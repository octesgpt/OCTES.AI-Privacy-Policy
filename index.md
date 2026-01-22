Privacy Policy — OCTES GPT Report Generator

Last updated: 2026-01-22

This Privacy Policy explains how data is handled when you use the OCTES GPT Report Generator (“the Service”). The Service generates DOCX/PDF reports (and related charts/tables) based on the information you provide.

1) What data we process

When you use the Service, we may process:

Report content you provide (text sections, tables, chart inputs, formulas, metadata like title/date/client name).

Generated output files (DOCX/PDF reports).

Basic technical data required to operate the Service (e.g., request timestamps, error logs, and performance/debug logs).

2) How your data is used

Your data is used only to:

Generate the requested report output (DOCX/PDF)

Render charts and formulas into the report

Return the output to you (either as a direct file response or via a download link)

Troubleshoot failures and improve reliability (via limited logging)

3) Where data is sent

To generate a report, the content you submit may be sent to:

Our backend API hosted on Microsoft Azure (Azure Functions)

Storage on Microsoft Azure Blob Storage (only when a download link is requested/returned)

4) Storage and retention

Depending on the response mode:

Raw/binary response (“return=raw”): the file is returned directly.
We do not intentionally store the generated file in Blob Storage in this mode.

URL response (“return=url”): the generated file is uploaded to Azure Blob Storage and a time-limited SAS link is returned.

Retention:

Files stored in Azure Blob Storage may remain until they are deleted or a retention policy is applied.

SAS download links are time-limited (typically ~60 minutes, depending on configuration).

If your organization requires a strict retention schedule (e.g., auto-delete after X days), please contact us to enable it.

5) Sharing and access

If a file is uploaded to Azure Blob Storage and returned via a SAS link, anyone who has the link may be able to download the file until the link expires.

We recommend treating download links as confidential and sharing them only with trusted recipients.

6) Security

We take reasonable steps to protect data, including:

Use of HTTPS for API access

Restricted access to Azure resources

Time-limited SAS URLs for file downloads (when enabled)

No method of transmission or storage is 100% secure, but we aim to use industry-standard protections.

7) Third-party services

This Service relies on:

OpenAI / ChatGPT (for the GPT experience)

Microsoft Azure (hosting and storage)

Your use of ChatGPT is also governed by OpenAI’s privacy and platform policies. Your use of Azure services is governed by Microsoft’s terms when applicable.

8) Children’s privacy

This Service is not intended for children under 13 and we do not knowingly collect personal information from children.

9) Your choices

You should avoid submitting:

passwords

private keys

highly sensitive personal data

If you believe sensitive data was submitted unintentionally, contact us to help remove stored outputs (if any exist).

10) Contact

If you have questions or requests regarding this policy, contact:

Email: parag@octes.com.au
