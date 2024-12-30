---
Title: '.strptime()' 
Description: 'Returns a datetime object that represents the parsed date and time from the given string, based on the specified format.'
Subjects:
- 'Python'
- 'Computer Science'
Tags:
- 'Date'
- 'Time'
- 'Strings'
CatalogContent:
- 'learn-python-3'
- 'paths/computer-science'
---

The **`.strptime()`** is a method included in the [`datetime`](https://www.codecademy.com/resources/docs/python/dates) module. It is used to parse a string representing a date and/or time and convert it into a `datetime` object using a specified format.

## Syntax

```pseudo
from datetime import datetime

datetime.strptime(date_string, format)
```

### Parameters:

- `date_string` (str): The string representing the date and/or time to be parsed..
- `format` (str): A string that defines the structure of `date_string` using format codes from the `datetime` module (e.g., `%Y` for a four-digit year, `%m` for a two-digit month).

It returns a `datetime` object, which represents the parsed date and time from the provided `date_string` according to the specified `format`.

## Example

```python
from datetime import datetime

# Define the date-time string and format
datetime_string = "27/12/2024 15:30:00"
datetime_format = "%d/%m/%Y %H:%M:%S"

# Parse the string into a datetime object
dt_object = datetime.strptime(datetime_string, datetime_format)

print(dt_object) #Output: 2024-12-27 15:30:00
```

## Codebyte Example

```codebyte/python
from datetime import datetime

# Define the date-time string and format
datetime_string = "27/12/2024 15:30:00"
datetime_format = "%d/%m/%Y %H:%M:%S"

# Parse the string into a datetime object
dt_object = datetime.strptime(datetime_string, datetime_format)

print(dt_object)  # Output: 2024-12-27 15:30:00
```