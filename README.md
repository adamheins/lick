# Lick
A simple tool for pulling a license into your software project.

Lick is written in Python and is compatible with both Python 2 and Python 3.

## Installation
Get the `lick` executable and put it on your `$PATH`. You can run
```bash
(curl https://raw.githubusercontent.com/adamheins/lick/master/lick)> lick
```
in your terminal to get a copy of lick.

Install Python dependencies by running
```bash
pip install -r requirements.txt
```

## Usage
Specify a license type for lick to pull in. Example:
```bash
lick MIT
```

Lick will fill out fields required in the license (name, year, etc.). Lick
first looks for fields in a JSON file pointed to be the environment variable
`$LICK_FIELD_FILE_PATH`. If that file does not exist, lick will use
`~/.lick.json` if it exists. Lick will ask you to enter any unfilled fields in
the terminal. It should be noted that the `<year>` field will automatically be
filled with the current year if not given in a file.

Lick field files are simple JSON files containing name-value pairs. For
example, here is a really simple lick field file just specifying a name:
```json
{
  "name": "John Doe"
}
```

You can also list all available licenses. Just run:
```bash
lick --list
```

## Contributing
Pull requests are welcome! Especially ones adding new licenses. Fields that
need to be filled out in the license should be placed between angled brackets
(`< >`). The field names should not contain whitespace. The name of the
license's file name must all be added to `LICENSES` list in the `lick` source
file.

## License
MIT license. See the LICENSE file.
