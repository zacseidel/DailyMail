# DailyMail
A project to automate email based on customized data sets.

*** work in progress - still being updated ***

### Background
This project created a script to send me an email each day with reminders about upcoming holidays and birthdays.  After doing that, I started including some reading along with recent market information.

This project was inspired by Willem Hoek's [Birthday Reminder](https://whoek.com/b/birthday-reminder-with-github-actions-and-python) project.  You can find his [Github repository here](https://github.com/whoek/birthday-reminder).

## Tools
- [Sendgrid API](https://sendgrid.com) for automating the email -- free for less than 100 emails per day.
- Github Actions for running the python script.  Note - [Azure Pipelines](https://learn.microsoft.com/en-us/dotnet/architecture/devops-for-aspnet-developers/actions-vs-pipelines) is an alternative for Github Actions.
- I wanted to include bible verses for reading each day.  I used the Revised Lectionary [resource from Vanderbilt University](https://lectionary.library.vanderbilt.edu/daily.php?year=A) to create a .csv file for a reading plan, and the ESV API to provide HTML code for each day's reading.
- While there are several free tools for downloading financial information, I found the easiest option to be creating a google sheet with the relevant information through the [GoogleFinance() function](https://support.google.com/docs/answer/3093281?hl=en), then downloading the data from the GoogleSheet to my email with the [gspread package](https://docs.gspread.org/en/latest/).

I found Chat GPT helpful in creating the python and html code.  

## Github Repository

Files used are:  
- `daily_mail.py` - python program which creates the html and sends the email
- `.env` - environment variables for the python program
- `birthdays.csv` - list of dates
- `verses.csv` - list of verses
- `github/workflows/pythonapp.yaml` - Github Actions setup file


## Content

### Reading


### Markets

### Recurring Reminders

### Occasions 

## Setup

### HTML

### Email

### Github Actions





