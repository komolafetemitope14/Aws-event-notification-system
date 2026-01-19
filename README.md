Event Announcement Website (Serverless AWS Project)

Overview

This is a serverless event announcement website built with AWS services.  
Users can view upcoming events, subscribe to email notifications, and create new events using a simple web form.

The frontend is hosted on Amazon S3, while AWS Lambda, API Gateway, and SNS handle the backend logic.

---

## Features

- Email subscription for event updates  
- Event listing from a JSON file  
- Create new events  
- Automatic email notifications  
- Fully serverless architecture  

---

## AWS Services Used 🛠

- **Amazon S3** – Frontend hosting & event data storage  
- **Amazon SNS** – Email notifications  
- **AWS Lambda** – Backend processing  
- **API Gateway** – API endpoints  
- **IAM** – Secure permissions  

---

## How It Works

1. Users access the website via S3  
2. Requests go through API Gateway  
3. Lambda processes the request  
4. Data is stored in S3 or sent via SNS  
5. Subscribers receive email alerts  

---

## System Design

You can describe:
- Architecture decisions  
- Security setup  
- Data flow  
- Scalability  

### Architecture Diagram

<img width="1324" height="710" alt="Event announcement 1" src="https://github.com/user-attachments/assets/cf6b78f8-7551-4293-83fe-c5fedacc5532" />

---

## API Endpoints

| Endpoint | Method | Description |
|----------|--------|-------------|
| /subscribe | POST | Subscribe user to email notifications |
| /create-event | POST | Create a new event and notify users |

---

## Project Files

index.html
styles.css
events.json
README.md


---

## Setup & Deployment

1. Upload files to S3  
2. Enable static website hosting  
3. Create SNS topic  
4. Create Lambda functions  
5. Configure API Gateway  
6. Test the application  

---

## Clean Up

Remember to delete AWS resources to avoid charges:
- S3 bucket  
- Lambda functions  
- API Gateway  
- SNS topic  
- IAM roles  

---

## 👨‍💻 Author

Komolafe Temitope
