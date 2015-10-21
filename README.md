# Lick
A simple tool for pulling a license into your software project.

Lick is written in Python and is compatible with both Python 2 and Python 3.

## Installation
Get the `lick` executable and put it on your path. You can run
```bash
(curl https://raw.githubusercontent.com/adamheins/lick/master/lick)> lick
```
in your terminal to get a copy of `lick`. Install Python dependencies by
running `pip install -r requirements.txt`.

## Usage
Specify a license type for lick to pull in. You must also provide the `--name`
option to fill in the license with your name. Example:
```bash
lick MIT --name "John Doe"
```

You can also list all available licenses. Just run:
```bash
lick --list
```

## Contributing
Pull requests are welcome! Especially PRs adding new licenses.

## License
MIT license. See the LICENSE file.
