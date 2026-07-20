# Day 21 - Create an AWS EC2 RSA Key Pair

## 📌 Task

Create an EC2 Key Pair in the AWS **us-east-1** region with the following requirements:

- Key Pair Name: **xfusion-kp**
- Key Pair Type: **RSA**

---

## 🛠️ Solution

### 1. Retrieve AWS Console Credentials

On the `aws-client` host, run:

```bash
showcreds
```

This provides:

- AWS Console URL
- Username
- Password

---

### 2. Log in to AWS Console

- Open the AWS Console URL.
- Sign in using the provided credentials.
- Select the **N. Virginia (us-east-1)** region.

---

### 3. Navigate to EC2

```
AWS Console
   └── EC2
        └── Network & Security
             └── Key Pairs
```

---

### 4. Create a New Key Pair

Click **Create Key Pair** and provide:

| Field | Value |
|--------|-------|
| Name | `xfusion-kp` |
| Key Pair Type | `RSA` |
| Private Key Format | `.pem` |

Click **Create Key Pair**.

---

## ✅ Verification

Verify that the key pair appears in the EC2 Key Pairs list.

| Name | Type |
|------|------|
| xfusion-kp | RSA |

---

## 💡 Key Learnings

- Learned the purpose of an **EC2 Key Pair**.
- Understood the difference between **RSA** and **ED25519** key types.
- Learned how EC2 Key Pairs are used for secure SSH authentication.
- Practiced creating AWS resources in the correct region (**us-east-1**).
- Understood the importance of following exact naming conventions in cloud environments.

---

## 🚀 AWS Services Used

- Amazon EC2
- EC2 Key Pairs
- AWS Management Console

---

## 📚 Concepts Covered

- AWS EC2
- SSH Authentication
- RSA Key Pair
- AWS Region
- Cloud Resource Management