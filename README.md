# 🌐 Amazon S3 Static Website Hosting

Host a fast, serverless static website using Amazon S3 — no EC2, no backend, just pure cloud simplicity. This project walks through the setup, configuration, and deployment of a static HTML page using AWS S3 and bucket policies.

---

## 🔍 Overview

This project demonstrates how to:
- Host a static website using Amazon S3
- Configure public access through a bucket policy
- Use the AWS Console to deploy cloud resources without writing backend code

Live demo message:  
📸 "Hello from Ejike on AWS!"

---

## 📚 Key Concepts

- Amazon S3 static website hosting  
- IAM and access control via bucket policy  
- Cloud-based object storage for web apps  
- Deploying without a web server (EC2-free)  

---

## 🧠 Learning Objectives

By the end of this project, you'll be able to:

- Set up an S3 bucket for static website hosting  
- Upload and manage website files (HTML/CSS)  
- Configure public access through IAM policies  
- Understand when to use S3 for hosting lightweight apps or demos  

---

## 🧰 Prerequisites

- Basic knowledge of AWS services  
- An AWS account (free tier is enough)  
- HTML fundamentals (you can use any simple HTML page)  

---

## 🛠 Project Structure

```bash
.
├── index.html               # Static website homepage
├── README.md                # Project documentation
└── images/                  # Screenshots of setup and result
    ├── bucket-config.png
    ├── bucket-policy.png
    └── website-preview.png


---

🚀 Steps to Deploy on Amazon S3

1. Create an S3 Bucket
Bucket name must be globally unique
Disable “Block all public access”


2. Upload index.html
Enable static website hosting in bucket properties
Set index document to index.html


3. Set Bucket Policy
Add this JSON to allow public access:



{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "PublicReadGetObject",
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::ejike-site/*"
    }
  ]
}

4. Access Your Site
Visit the bucket’s website endpoint URL
You should see: "Hello from Ejike on AWS"




---

✅ Comprehensive Checklist

[x] Created unique S3 bucket

[x] Uploaded index.html

[x] Enabled static website hosting

[x] Applied public-read bucket policy

[x] Verified website via browser



---

💬 Where to Get Help

If you're stuck:

Use the AWS Documentation on S3 Hosting

Open an Issue in this repo

Tag me on LinkedIn: Ejike Gloria on LinkedIn



---

👩‍💻 Maintainer

Made with grit by:

Ejike Gloria
AWS Certified Solutions Architect – Associate
Cloud & Backend Dev Intern @ CodeAlpha
📍 Nigeria 🇳🇬
GitHub • LinkedIn
