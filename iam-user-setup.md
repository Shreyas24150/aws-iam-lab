# IAM User Setup – Read-Only S3 Access

## ✅ Objective
Create a limited-permission IAM user that can only **read** from S3 (no write/upload allowed).

## 🧭 Steps

1. Go to IAM Console → Users → Add user
2. Username: `dev-user`
3. Access type: ✅ Programmatic access, ✅ AWS Management Console
4. Set a custom password
5. Permissions: Attach policy `AmazonS3ReadOnlyAccess`
6. Create user → Save access keys

## 🔐 Sign-in
Use the AWS account sign-in URL:
