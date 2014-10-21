# Install

### Using pip

```
pip install att
```

### From sources

```
python setup.py install
```

# Usage
```
Usage:
  att.py
  att.py --phone PHONE --code CODE
  att.py --from FROM
  att.py --from FROM --to TO
  att.py --phone PHONE --code CODE --from FROM
  att.py --phone PHONE --code CODE --from FROM --to TO
  att.py (-h | --help)
  att.py --version

Options:
  -h --help         Show this screen.
  -v --version      Show version.
  -p --phone        Phone number.
  -c --code         AT&T 4 digits code.
  -f --from         Date from (MM/DD/YYYY).
  -t --to           Date to (MM/DD/YYYY).
```

The `PHONE` and `CODE` can be retreived from your environment variables.
