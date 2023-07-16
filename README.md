# Facebook Post Backup Tool

## Motivation

With the current Facebook policies in place, there's a risk that significant posts may be removed due to malicious reports. To safeguard against this, I write a simple script to back up posts shared on Facebook.

## Prerequisites

Before running the script, make sure that the required dependencies are properly installed. There are two methods to do this:

1. **Using `poetry`**: Install `poetry` and run the script as described under the 'Usage' section.

2. **Using `pip`**: Directly install the dependencies using `pip` with the command provided below:
   
   ```shell
   pip install -r requirements.txt
   ```

## Usage

To use the tool, run the following command with `poetry`:

```shell
poetry run python src/main.py --url [url] --filename [filename]
```

Replace `[url]` with the URL of the Facebook post you want to back up, and replace `[filename]` with the desired name of the output file.

The script will store the backed-up post in a directory named after the post time (e.g., "2023-07-15"), and the file name will be the one you provided (e.g., "a.md").
