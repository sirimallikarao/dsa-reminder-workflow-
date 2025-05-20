# DSA Practice Reminder using n8n

This repository contains an automated workflow built with **n8n** that sends daily emails with Data Structures and Algorithms (DSA) practice problems.

## What it does

- Fetches problems from a Google Sheet  
- Selects two problems every day, prioritizing unsolved ones  
- Sends these problems via Gmail twice a day, at 4:00 AM and 6:00 PM  

## Google Sheet format

The Google Sheet should have these columns:  
- Topic  
- Problem description  
- Status (mark "Yes" if solved, "No" if unsolved)  

## Setup instructions

1. Import the workflow JSON file into your n8n instance  
2. Set up OAuth2 credentials for Google Sheets and Gmail  
3. Update the workflow with your Google Sheet ID and recipient email address  
4. Activate the workflow  

## How it works

- The workflow triggers automatically at 4 AM and 6 PM every day  
- It fetches problems from the Google Sheet  
- It selects two problems, favoring unsolved ones  
- It sends an email with the selected problems to the configured email address  

---

Feel free to customize the workflow and sheet to fit your practice needs!

