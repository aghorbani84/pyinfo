# PyInfo

A lightweight Python website-inspection script that retrieves a page, formats its HTML, and extracts text from an element with the `admin-plans` CSS class.

## What it does

The current script (`soucegather.py`):

1. Prompts for a website URL.
2. Downloads the page using `requests`.
3. Parses the response with Beautiful Soup.
4. Saves formatted HTML and the matching `.admin-plans` text to `information.txt`.

If the target element is absent, the report records that it was not found.

## Requirements

- Python 3
- `requests`
- `beautifulsoup4`

Install dependencies:

```bash
python -m pip install requests beautifulsoup4
```

## Run

```bash
git clone https://github.com/aghorbani84/pyinfo.git
cd pyinfo
python soucegather.py
```

Enter a URL when prompted. The output is written to `information.txt` in the current working directory.

## Limitations and responsible use

- The extractor currently targets the specific `.admin-plans` class; it is not a general-purpose crawler.
- It processes the HTML returned by the initial HTTP response and does not execute JavaScript.
- Use it only on websites you own or are authorized to inspect. Respect site terms, access controls, and rate limits.
- Review downloaded content before sharing it; page HTML may contain private or sensitive data.

## Contributing

Improvements should preserve the script's small scope and document any new dependencies or extraction rules.