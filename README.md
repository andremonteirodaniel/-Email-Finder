Email-Finder

Email Finder (Web Crawler)

A simple Python tool that crawls a starting URL, recursively follows internal and external links, and extracts valid email addresses found on HTML pages. Useful for intelligence gathering (OSINT) and security testing.

Features

Recursive Crawling: Starts at a URL and follows all found links that have not been crawled previously.
Email Extraction: Uses regular expressions to identify emails in standard format.
Visitor Control: Keeps a record of already crawled URLs to avoid unnecessary loops and repetitions.

Prerequisites

Make sure you have Python installed. The following libraries are required:

 `requests`
 `beautifulsoup4`

Installation

1. Clone the repository:

``bash
git clone https://github.com/andremonteirodaniel/-Email-Finder.git

cd -Email-Finder

``
2. Install the dependencies:

``bash
pip install -r requirements.txt

```

Usage

Run the script providing the starting URL as a command-line argument.

``bash
python email_finder.py <STARTING_URL>

    Important Technical Details

  Uses the `requests` library to make HTTP requests.

 Uses `BeautifulSoup` to parse HTML and extract * link tags (`<a>`).

The regular expression used for emails is: `r"\w[\w\.]+\w@\w[\w\.]+\w"`.
