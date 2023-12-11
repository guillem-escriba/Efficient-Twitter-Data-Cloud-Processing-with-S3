Twitter Data Processing and Benchmarking Tool
Contributors
David Pérez Carrasco (u188332)
Guillem Escriba Molto (u188331)
Pau Folch (u188246)
Overview
This project involves creating a tool for processing Twitter data, including features like tweet simplification, language filtering, cloud uploading, and performance benchmarking.

SimplifiedTweet:
Constructs an object using 6 features described in the assignment.
Implements Optional<SimplifiedTweet> to convert a string into a JSON object with these features, returning an empty object if the string lacks any.
Includes a getLanguage method to return the tweet's language.

FileLanguageFilter:
Filters tweets by language.
Reads input files line by line, creating SimplifiedTweet objects and writing complete tweets of the filtered language to the output file.
Appends to the output file without overwriting.

S3Uploader:
Manages file uploads to an Amazon S3 bucket.
Checks for bucket existence and creates it if not found.
Handles file uploading, overwriting existing files or creating new ones as needed.

Benchmarking:
Measures the execution time for filtering and uploading processes.
Reports the number of filtered tweets and the processing time for each folder.
Identifies challenges in calculating total tweets and execution time.

Execution:
Provides a command for executing the program with specific datasets.
Requires the dataset to be downloaded and decompressed in the specified folder for successful execution.

Extensions:
Implements suggested tests for verifying parsing correctness and handling exceptions.
Considers additional tests for the upload process.
