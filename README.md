# MCL Automatic Sign-In System - GitHub Runner

A runner that automates the sign-in/sign-out process for NCU HumanSys. You can securely provide your credentials at runtime without storing them in the Docker image.

## Hub

**GitHub**: [wulukewu/mcl-sign-in-system](https://github.com/wulukewu/mcl-sign-in-system)

**Docker Hub**: [wulukewu/mcl-sign-in-system](https://hub.docker.com/r/wulukewu/mcl-sign-in-system)

## Quick Start

Run the container with the following command:

```bash
docker run wulukewu/mcl-sign-in-system:latest --inorout <signin|signout> --username <your_username> --password <your_password> --otpauth <[optional] otpauth_url>
```

## Secrets Configuration (GitHub Actions)

If you're using GitHub Actions, add the following secrets under your repository settings:

- **`--username`**: Your Student ID used for login.
- **`--password`**: Password for your portal login.
- **`--otpauth`** [optional]: OTP URL to generate a one-time password (OTP) for two-factor authentication.
