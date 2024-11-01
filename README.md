# MCL Automatic Sign-In System

This Dockerized application automates the sign-in/sign-out process for MCL. You can securely provide your credentials at runtime without storing them in the Docker image.

## Quick Start

Run the container with the following command:

```bash
docker run wulukewu/mcl-sign-in-system:latest --inorout [signin/signout] --username [your_student_id] --password [your_password] --otpauth [otpauth_url]
```

### Parameters
- **`--inorout`**: Specify `"signin"` or `"signout"` for the desired action.
- **`--username`**: Your Student ID used for login.
- **`--password`**: Password for your portal login.
- **`--otpauth`** (optional): OTP URL to generate a one-time password (OTP) for two-factor authentication.

## Secrets Configuration (GitHub Actions)

If you're using GitHub Actions, add the following secrets under your repository settings:

- `username`: Your Student ID.
- `password`: Your portal login password.
- `otpauth` (optional): OTP URL for two-factor authentication.

## References

- [VS Code + Python + Selenium Automation Testing Part 1](https://medium.com/begonia-design/vs-code-python-selenium-%E8%87%AA%E5%8B%95%E5%8C%96%E6%B8%AC%E8%A9%A6-part-1-30d6c0ea92af)
- [Day 15: Dynamic Web Page Scraping 2 - Selenium Data Location Functions](https://ithelp.ithome.com.tw/articles/10300961)
- [【 Python 】利用 .env 與環境變數隱藏敏感資訊](https://learningsky.io/python-use-environmental-variables-to-hide-sensitive-information/)
