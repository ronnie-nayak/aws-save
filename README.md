# Save Up

Save-Up is a money management tracker that allows users to track their expenses and savings. It has a dashboard that shows updates, lots of tools for managing transactions, goals, billing reminders, and bank statement upload. It is built using modern web technologies and hosted on AWS cloud. The platform is made so that users can use it easily and connect with cloud services smoothly.

## Report Link

Check out the following project report on project features and screenshots of working.

**Link:** https://drive.google.com/file/d/1ZfJPFqq1lEBgtLRSXmqrCIr9fmhRAc5X/view?usp=sharing

## Steps to run code
### Prerequisite: 
- Add .env file with following details
  ```
  PORT='3000'
  
  # AWS IAM Role with S3, SES and RDS permissions
  AWS_KEY_ID=''
  AWS_SECRET_ACCESS_KEY=''
  AWS_REGION=''
  
  # AWS RDS details
  DATABASE_URL='postgresql://<username>:<password>@<URL>:<port>/<dbName>'
  
  # Next-Auth details
  AUTH_URL='http://localhost:3000'
  AUTH_INTERNAL_URL='http://localhost:3000'
  AUTH_SECRET=''
  
  # Discord and Github Auth details
  AUTH_DISCORD_ID=''
  AUTH_DISCORD_SECRET=''
  AUTH_GITHUB_ID=''
  AUTH_GITHUB_SECRET=''
  
  # AWS S3 details
  AWS_S3_BUCKET_NAME=''
  
  # GROQ API Key
  GROQ_API_KEY=''
  ```
- Install Docker CLI on your system
- Run Docker container
  ```
  docker compose up
  ```
- Deactivate Docker container
  ```
  docker compose down
  ```

## Features
- Extract and store transaction history from Bank Statements using OCR in PostgreSQL using RDS
- Distribute traffic using EC2 Load-Balancing and send notifications via SES
- S3 used to keep uploaded bank statement files and keep files safe and easily accessible
- Login using OAuth with Github/Discord
- Responsive Design
- Analytics of transaction history
- Filter History
- Set Recurring Bills
- Set Savings Targets

## Tech Stack

**Client:** React, TailwindCSS, Framer Motion

**Server:** NextJS, TypeScript, tRPC, DrizzleORM

**AWS Services:** EC2, RDS, S3, SES

## Members

Abhishek Nayak (E22CSEU1499)

Neha Nayak (E22CSEU1518)

Utkarsh Singh (E22CSEU0540)
