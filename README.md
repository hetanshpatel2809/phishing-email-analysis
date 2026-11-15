# Phishing Email Analysis

## About the Project

This project focuses on analyzing a suspicious email sample to identify possible phishing indicators. It involves examining email headers, sender information, authentication results, message content, and embedded URLs to understand potential email-based threats.

The analysis is performed using a publicly available `.eml` email sample.

## Objectives

- Identify suspicious sender addresses and domains.
- Examine email headers for authentication issues.
- Analyze SPF, DKIM, and DMARC results.
- Identify suspicious links and possible URL manipulation.
- Detect social engineering and phishing indicators.
- Prepare a structured phishing analysis report.

## Tools and Technologies

- **Email Client / Text Editor:** To inspect the `.eml` file.
- **Email Header Analysis:** To examine sender information and authentication results.
- **URL Inspection:** To identify suspicious URL characteristics.
- **Manual Investigation:** To identify phishing indicators in the email content.

## Project Structure

```text
Phishing-Email-Analysis/
│
├── README.md
│
├── sample-email/
│   └── sample-10.eml
│
├── analysis/
│   └── phishing_analysis_report.txt

```

## Analysis Performed

The following areas were examined:

### 1. Sender Analysis
- Display name and actual sender address.
- Sender-domain mismatch.
- Return-Path information.

### 2. Email Header Analysis
- SPF authentication result.
- DKIM authentication result.
- DMARC authentication result.
- Reply-To information.
- Received headers.

### 3. Email Content Analysis
- Promotional claims.
- Requests to install a browser extension.
- Wallet-related instructions.
- Potential social engineering techniques.

### 4. URL Analysis
- Embedded links.
- Suspicious URL characteristics.
- Possible Unicode lookalike characters.
- Destination verification requirements.

## Key Findings

The analyzed email promoted an OKX Web3 browser extension.

Some suspicious characteristics identified were:

- The displayed brand name did not clearly match the sender's domain.
- SPF authentication result was `none`.
- DKIM authentication result was `fail`.
- DMARC authentication result was `none`.
- The embedded extension link contained potentially deceptive Unicode characters.
- The email encouraged users to install an extension and create or import a wallet.

**Note:** These findings indicate suspicious characteristics but do not independently prove that the email or extension is malicious.

## Results

The email was classified as **Suspicious – Further Verification Required**.

The analysis demonstrated how email headers, authentication results, sender information, message content, and URLs can help identify potential phishing attempts.

For detailed findings, refer to:

`analysis/phishing_analysis_report.txt`

## How to Use

1. Clone or download this repository.
2. Open the `sample-email` folder.
3. Inspect the `sample-10.eml` file using a text editor or email analysis tool.
4. Examine the email headers and message content.
5. Compare your observations with the report in the `analysis` folder.

## Security Precautions

- Never click suspicious email links.
- Do not install browser extensions from unverified sources.
- Never share passwords, private keys, or wallet recovery phrases.
- Verify the sender through official communication channels.
- Perform suspicious-link analysis in a safe environment.

## Limitations

- The analysis is based on the supplied email sample.
- No live interaction with the embedded link was performed.
- The browser extension's actual behavior was not tested.
- The findings do not establish that the email caused a successful compromise.

## Disclaimer

This project is intended strictly for educational and cybersecurity awareness purposes. The sample email is analyzed for learning and research. Do not use suspicious links or attachments on personal or production systems.

## Author

**Hetansh Patel**

Cyber Security Student | Cybersecurity Intern
