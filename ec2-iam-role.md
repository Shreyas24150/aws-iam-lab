# EC2 IAM Role – Full S3 Access

## ✅ Objective
Allow EC2 to access S3 with full permissions using an IAM Role — **no keys required**.

## 🧭 Steps

1. IAM → Roles → Create role
   - Trusted entity: AWS service → EC2
   - Permissions: Attach `AmazonS3FullAccess`
   - Name: `EC2-S3-Access-Role`

2. Go to EC2 → Instances → Select your instance
   - Actions → Security → Modify IAM Role
   - Attach `EC2-S3-Access-Role`

3. Connect to EC2 instance:
   ```bash
   sudo apt update
   sudo apt install awscli -y
   aws s3 ls

🧪 Test
✅ S3 bucket list visible

✅ Able to upload/download/delete S3 files

