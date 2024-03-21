# analyzes_emails
Python script that analyzes emails from either a local PST file or a remote email server inbox

# Check up & analyze emails on PST/server; add automatic actions (analyzes_emails)
<a href="https://github.com/FernandoTorresL/analyzes_emails/commits/main" target="_blank">![GitHub last commit](https://img.shields.io/github/last-commit/FernandoTorresL/analyzes_emails)</a>

<a href="https://github.com/FernandoTorresL/analyzes_emails" target="_blank">![GitHub repo size](https://img.shields.io/github/repo-size/FernandoTorresL/analyzes_emails)</a>

Validate XML files structure and data for use with SIE (IMSS) system.
## Objective

The goal is to develop a Python script that analyzes emails from either a local PST file or a remote email server inbox. The script will search for specific keywords within the emails and, when a keyword is found, send a notification email to the sender. Additionally, the script will save metadata from the emails to a MongoDB database.

## Description

The script takes a configuration file (secrets.ini) as input, containing parameters such as the path to the PST file, email server connection details, keywords to search for, and MongoDB connection settings. Based on the configuration, the script connects to either a local PST file or a remote email server inbox using libpff or exchangelib, respectively.

For each email, the script extracts metadata including sender email address, subject, and received time, saving this information to a MongoDB database. It also checks the email content for specified keywords. If any keyword is found in the email subject or body, the script sends a notification email to the original sender.

The script reduces the manual effort required to search and notify email senders based on specific criteria, enhancing efficiency in email management workflows. Additionally, by storing email metadata in MongoDB, it enables further analysis and retrieval of email data for various purposes.

## Technology used

This project was build with the use of: 

- Python v3.??
- Python v3.?? (W10)

## Installation

### Clone repo

```sh
git clone git@github.com:FernandoTorresL/analyzes_emails.git
```
> Optional: You can change *<my_folder>* on the next instruction to create a new folder

```sh
git clone git@github.com:FernandoTorresL/analyzes_emails.git <my_folder>
```

### Create / copy initial files (only placeholder_file.txt on GitHub)

You must create o paste some files on place:

- A **secrets.ini** file based on secrets.example.ini (Update values on file)

### Change to working directory and create a Python virtual environment

OS X & Linux:

```sh
$ cd analyzes_emails
$ python -m venv ./venv
$ source ./venv/bin/activate
$ pip install --upgrade pip
$ pip3 install -r requirements.txt
(venv) $
```

Windows:
```sh
$ cd analyzes_emails
$ python -m venv venv
$ .\venv\Scripts\activate
$ pip3 install -r requirements.txt
(venv) $
```

Windows 10 with Git bash terminal:
```sh
$ cd analyzes_emails
$ python -m venv venv
$ source ./venv/Scripts/activate
$ pip3 install -r requirements.txt
(venv) $
```

Windows 10 with powershell terminal:
```sh
PS> cd analyzes_emails
PS> python -m venv venv
PS> .\.venv\Scripts\Activate.ps1
PS> pip3 install -r requirements.txt
(.venv) PS>
```

Windows 10 with WSL shell:
```sh
user@pc_name: cd analyzes_emails
user@pc_name: python3 -m venv venv
user@pc_name: source venv/bin/activate
user@pc_name: pip install --upgrade pip
user@pc_name: pip3 install -r requirements.txt
(venv) user@pc_name:
```

> This prompt may vary if you use another shell configuration, like pk10 or git bash

Later, to deactivate the virtual environment
OS X & Linux & Windows:

```sh
(venv) $ deactivate
$
```

### View help and arguments

```sh
python3 analyzes_emails.py --help
```

```sh
usage: analyzes_emails.py [-h]
```
> If using another Python version try: python analyzes_emails.py --help

## Run the project

Before run this project, edit or copy the following files:

* secrets.ini

Then, you can execute the program:

```sh
python analyzes_emails.py
```

### Example

```sh
python analyzes_emails.py
```

### Example output

```sh

```

## Output files

---

## Contributing to this repo

1. Fork it (<https://github.com/FernandoTorresL/analyzes_emails/fork>)
2. Create your feature branch (`git checkout -b feature/fooBar`)
3. Commit your changes (`git commit -am 'Add some fooBar'`)
4. Push to the branch (`git push origin feature/fooBar`)
5. Create a new Pull Request

---

<div align="center">
    <a href="https://fertorresmx.dev/">
      <img height="150em" src="https://raw.githubusercontent.com/FernandoTorresL/FernandoTorresL/main/media/FerTorres-dev1.png">
  </a>
</div>



## Follow me 
[fertorresmx.dev](https://fertorresmx.dev/)

#### :globe_with_meridians: [Twitter](https://twitter.com/FerTorresMx), [Instagram](https://www.instagram.com/fertorresmx/): @fertorresmx
