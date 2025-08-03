# URL Shortener

A simple command-line URL shortening service implemented in Python. This program allows users to shorten long URLs and retrieve the original URLs using their shortened versions.

## Features

- Generate shortened URLs using MD5 hashing
- Store and retrieve URL mappings
- In-memory storage using Python dictionary
- Simple command-line interface

## How to Use

1. Run the program:

```python
python main.py
```

2. Choose from the following options:
   - Option 1: Shorten a URL
   - Option 2: Retrieve Original URL
   - Option 3: Exit

### Shorten a URL

- Enter a long URL when prompted
- Get a shortened version in the format: `http://short.ly/{6-character-code}`
- Duplicate URLs will return existing short URLs

### Retrieve Original URL

- Enter the shortened URL
- Get back the original long URL
- Returns an error message if URL not found

## Technical Details

- Uses `hashlib.md5` for URL hashing
- Generates 6-character unique codes
- Stores URL mappings in an in-memory dictionary
- Written in Python 3

## Limitations

- Data is not persistent (lost when program exits)
- Uses in-memory storage (not suitable for large-scale use)
- No validation for URL format

## Author

Shivam Ramola

## License

This project is open source and available under the
