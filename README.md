# Gmail Automated Workflow (n8n)

## Description
This project automates the process of receiving emails with attachments (such as CVs or requests) using **n8n**. It organizes incoming attachments efficiently, uploads them to **Google Drive**, and can send automatic confirmation emails to the sender.

**Workflow Overview:**
1. **Gmail Trigger**: Detects new emails received in your Gmail account.
2. **Filter**: Checks if the email contains attachments.
3. **Get Message**: Retrieves the full email message and attachments.
4. **Set Fields & Split Out**: Prepares attachments and metadata for processing.
5. **Merge**: Combines attachment data with email metadata.
6. **Upload File (Google Drive)**: Saves each attachment to a designated folder in Google Drive.

Optional: You can extend the workflow to send customized responses based on the email content or type of attachment.

## Features
- Automatic processing of emails and attachments without manual intervention.
- Uploads attachments to Google Drive in a structured way.
- Optional automatic confirmation emails to senders.
- Supports multiple attachments and diverse file types.
- Easily extendable for advanced filtering or additional actions.

## Technologies Used
- **n8n** for workflow automation.
- **Gmail** for receiving emails.
- **Google Drive** for storing attachments.
- **Google Sheets** for optional metadata tracking.
- **Gmail** for sending confirmation emails.

## How to Use
1. Import the workflow JSON (`n8n_attachments.json`) into your n8n instance.
2. Connect your Gmail and Google Drive accounts via OAuth2 credentials.
3. Activate the workflow to start automatically processing incoming emails.

