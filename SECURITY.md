# Security Policy

## Reporting a vulnerability

Please report potential security issues privately through GitHub's private
vulnerability reporting feature when available. Do not open a public issue
containing credentials, tokens, personal data, or exploit details.

## Credentials

Example notebooks must not contain live credentials. Use environment variables
or local configuration excluded by `.gitignore`, restrict every API key to the
minimum required APIs and origins, and revoke any credential that is committed
accidentally.
