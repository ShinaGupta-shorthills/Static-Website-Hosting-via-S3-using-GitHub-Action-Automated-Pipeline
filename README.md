# Static-Website-Hosting-via-S3-using-GitHub-Action-Automated-Pipeline
Use S3 to host a static HTML website with public access.

🧠 What We’re Trying to Do
We want to:
Write and commit some static web files (HTML, CSS, JS) into a GitHub repo.
Use GitHub Actions to automatically:
Upload these files to an S3 bucket.
Host them as a static website from that S3 bucket.

🧰 Prerequisites
Before writing the pipeline, make sure:
You have an AWS account.
You created an S3 bucket, e.g., my-static-site-bucket.
You enabled static website hosting for the S3 bucket.
You created an IAM user with programmatic access and permissions for S3:
AmazonS3FullAccess or custom permissions.
You store the IAM credentials in your GitHub repository secrets:
AWS_ACCESS_KEY_ID
AWS_SECRET_ACCESS_KEY
AWS_REGION (like us-east-1)

## 📦 Deployment Steps (AWS S3)

1. Create an S3 bucket with public access.
2. Enable static website hosting in the bucket settings.
3. Upload the `index.html` file.
4. Set `index.html` as the default document.
5. Access your site using the provided S3 website URL.

---

Made by Shina
