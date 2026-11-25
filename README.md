<h1 align="center">pyinfo</h1>

<p align="center">
  <em>A minimal Python 3 script that fetches a web page and saves its HTML (and one target element's text) to a file.</em>
</p>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-GPLv3-blue.svg" alt="License: GPL v3" /></a>
  <img src="https://img.shields.io/badge/Python-3-3776AB?logo=python&logoColor=white" alt="Python 3" />
</p>

---

## Overview

`soucegather.py` is a small learning script for basic web information gathering. It asks for a URL, downloads the page with `requests`, parses it with BeautifulSoup, and writes the results to `information.txt`.

## Features

- Prompts for a target URL
- Saves the full, prettified HTML source of the page
- Extracts the text of a specific element — by default `<div class="admin-plans">` (edit the selector in the script to target something else)
- Reports network/HTTP errors instead of crashing

## Tech Stack

- Python 3
- [requests](https://requests.readthedocs.io/)
- [Beautiful Soup 4](https://www.crummy.com/software/BeautifulSoup/)

## Getting Started

```bash
git clone https://github.com/aghorbani84/pyinfo.git
cd pyinfo
pip install requests beautifulsoup4
python3 soucegather.py
# Enter the URL of the site: https://example.com
```

Output is written to `information.txt` in the current directory.

> [!IMPORTANT]
> Only gather information from websites you own or are permitted to access, and respect each site's terms of service and `robots.txt`.

## Project Structure

```
.
├── soucegather.py   # The script
├── LICENSE          # GPL-3.0
└── README.md
```

## License

Licensed under the [GNU General Public License v3.0](LICENSE).

## Author

**Abolfazl Ghorbani** — [@aghorbani84](https://github.com/aghorbani84)
