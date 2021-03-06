# Password Manager

## About

A password manager that can be used to store your usernames and passwords for different services, using google sheets via a python script.

While this isn't really the most *"secure"* password manager in the universe and I don't recommend that you use it, I was just really curious about the gspread library and had never written more than 10 lines in Python before so I challenged myself to make this project in less than 12 hours overall.

I learned a lot during this mini project so it was well worth it!

## Dependancies

This project uses the following:
+ Python3 or later
+ gspread python library
+ oauth2client python library

### Install the dependancies

#### Ubuntu and its derivatives
```
  $ sudo apt update
  $ sudo apt install python3-pip build-essential
  $ sudo pip3 install gspread oauth2client
  $ sudo pip3 install --upgrade google-auth-oauthlib
```

#### Arch and its derivatives
```
  $ sudo pacman -Sy python-pip
  $ sudo pip install gspread oauth2client
  $ sudo pip install --upgrade google-auth-oauthlib
```

## How to run

Clone this repo and make sure that the "PasswordManager.py" and "PasswordManagerAuth.json" files are in the same folder.

This WILL make you access the SAME Google sheet as anyone who has tried this project, the Google sheet contains some dummy usernames and password. DO NOT enter any real usernames or passwords there, they will be visible to everyone else.

If you wish to use this project, fork it and add your OWN Google sheet using this tutorial: https://youtu.be/vISRn5qFrkM


To run from a Linux shell: 
``` 
clear && python3 PasswordManager.py
```

After that you will see the master password printed on the first line of your terminal, use that to edit the _database_ of usernames and passwords and play around! 

Please don't mess up the google sheet too much(Preferably just add your name as a username and add any dummy password!) as that will ruin the demonstration of this project for anyone else who is curious about it.
