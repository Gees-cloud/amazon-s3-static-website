 # 🌐 Amazon S3 Static Website Hosting

This project demonstrates how to host a simple static website using *Amazon S3*, one of AWS’s most powerful storage services.

## 📸 Preview

> *Live Message:* "Hello from Ejike on AWS"  
![S3 Website Screec:c:c:\Users\Ejike\OneDrive\Pictures\website-preview.png\Users\Ejike\OneDrive\Pictures\bucket-policy.png\Users\Ejike\OneDrive\Pictures\bucket-config.png.jpgnshot](c./images/website-preview.png)

---

## 🧰 Tools & Services Used

- *Amazon S3*
- *AWS Console*
- *IAM (for access control)*
- *Bucket Policies*

---

## ✅ What I Did

- Created a new S3 bucket with a unique name
- Uploaded a basic index.html file
- Enabled *static website hosting* in the bucket properties
- Wrote a *bucket policy* to allow public access to the files
- Visited the *S3 website endpoint* and saw the site live!

---

## 🔐 Bucket Policy Sample

```json
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
