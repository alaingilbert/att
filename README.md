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

The `PHONE` and `CODE` can be retreived from your environment variables.

### Commande line
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

### Code

```python
>>> from att import Att
>>> att = Att(PHONE, CODE)
>>> print att.getAllEvents(DATE_FROM, DATE_TO)
```

### Response

```python
[{'units_charged': u 'NA',
  'duration': u '0min 32sec',
  'call_location': u '-,-,USA',
  'date': '2014-10-16 10:24:08+00:00',
  'timezone': u 'US/Mountain',
  'total_amount': 0,
  'number_called': u '14155559161',
  'calling_number': u '16505557827',
  'service_used': u '$40 Monthly',
  'nature_of_call': u 'Local',
  'type': u 'Outgoing Call'
},...]
```