*Intuz — Your automation partner, one workflow at a time.*

<p align="center">
  <picture>
    <img alt="Banner Image" src="https://github.com/user-attachments/assets/210f97fc-0fce-404a-b647-7dfe1302cd37" />
  </picture>
</p>

[Intuz](https://www.intuz.com) helps organizations orchestrate AI, automation, and enterprise systems through scalable workflows. Our repository showcases proven implementations across healthcare, operations, customer support, document processing, sales, and back-office functions, enabling teams to accelerate automation initiatives without starting from scratch.

[N8N Creator](https://n8n.io/creators/intuz/) · [AI Agent Development](https://www.intuz.com/ai-agents-for-business-automation/) · [AI Automation Services](https://www.intuz.com/ai-automation-services/) · [For Custom Workflow Automation](https://www.intuz.com/get-started/)

# Hyper-personalize email outreach with AI, Gmail, and Google Sheets

Intuz provides a complete and automated solution for hyper-personalized email outreach.

It powerfully combines AI with Gmail and Google Sheets, using specific keywords and prospect data to automatically craft unique, compelling email content that boosts engagement and secures more replies.

Instead of manually replying to every lead or inquiry, this template does the heavy lifting for you, ensuring every response is relevant, thoughtful, and timely.

It reads each person’s unique inquiry, uses OpenAI to craft a perfectly tailored and human-like response, and sends it directly from your Gmail account. Ideal for sales, marketing, and customer support teams looking to boost engagement and save hours of manual work.

## Use Cases

- **Sales Teams:** Instantly follow up with new leads from your website’s contact form with a personalized touch.
- **Customer Support:** Provide initial, intelligent responses to support tickets, answering common questions or acknowledging receipt of a complex issue.
- **Marketing Automation:** Nurture leads by responding to content downloads or webinar sign-ups with relevant, non-generic information.
- **Founders & Solopreneurs:** Manage all incoming business inquiries, including partnerships, media, and other requests, efficiently without sacrificing quality.

## How It Works

### 1. Trigger the Flow (Manual)

Start the automation whenever you’re ready to process a new batch of inquiries from your sheet.

### 2. Fetch Inquiries from Google Sheets

The workflow connects to your specified Google Sheet and reads each row. It pulls the contact’s First Name, Email ID, Inquiry Intent (e.g., “Demo Request,” “Pricing Inquiry”), and the full text of their Original Inquiry.

### 3. Sync Your Signature

Before writing the email, an HTTP Request node dynamically fetches your display name from your Gmail account settings. This ensures the signature in the generated email (`Thanks, {{Your Name}}`) is always accurate.

### 4. Craft a Hyper-Personalized Reply with AI

It uses this context to generate a high-quality, professional, and friendly email reply in HTML format.

For example:

- If the intent is **“Technical Support,”** the AI will generate a helpful, empathetic response addressing the technical issue.
- If the intent is **“Partnership Proposal,”** it will draft a professional reply acknowledging the proposal and outlining the next steps.

### 5. Send via Gmail

The final node takes the AI-generated message, adds a relevant subject line (e.g., “Re: Your Demo Request”), and sends it directly to the contact’s email address from your connected Gmail account.

This process loops for every single row in your Google Sheet, turning a list of names into a series of meaningful conversations.

## Setup Instructions

To get this workflow running, you’ll need to configure a few things:

### 1. Credentials

- **Google:** Connect your Google account via OAuth2 and ensure you have enabled access for Google Sheets, Google Drive, and Gmail.
- **OpenAI:** Add your OpenAI API key as a credential.

### 2. Google Sheet Setup

Create a Google Sheet with the following exact column headers:

- `First Name`
- `Email ID`
- `Inquiry Intent` — A short category like “Demo Request”, “Billing Issue”, etc.
- `Original Inquiry` — The full text of the email or message you received.

### 3. Node Configuration

- **Get row(s) in sheet:** Select your Google Sheet document and the specific sheet name.
- **Message a model (OpenAI):** Choose your preferred OpenAI model, such as `gpt-4-turbo` or `gpt-3.5-turbo`.

### 4. HTTP Request & Send Personalized Emails

These nodes should automatically use your configured Gmail credentials. No changes are typically needed.

## FAQ

**Is this template free to use?**
Yes. It's an open-source n8n workflow published by Intuz — copy the workflow JSON from this repo and import it into your own n8n instance at no cost.

**Do I need a paid n8n plan to run this?**
No. It runs on n8n's free self-hosted Community Edition or on n8n Cloud. You'll need your own credentials for the services this workflow connects to, not a specific n8n pricing tier.

**Does it send the email automatically, or draft it for review?**
It sends automatically — the workflow drafts a personalized reply with AI and sends it directly from your connected Gmail account with no manual approval step. Review the AI prompt carefully before activating in production.

## Related n8n templates from Intuz

- [Automate cold outreach with email personalization using Gemini and Google Sheets](https://github.com/Intuz-production/Personalized-Sales-Outreach-Automation-with-AI)
- [Automate AI Upwork proposal generation with Apify, Google Gemini & Sheets](https://github.com/Intuz-production/Upwork-proposal-generation-automation)
- [Route Gmail Emails to Slack Channels Using AI](https://github.com/Intuz-production/AI-Powered-Gmail-to-Slack-Email-Routing)

See all of Intuz's free n8n templates: https://www.intuz.com/n8n-workflow-automation-templates/

## Connect with us

Intuz is a USA-based AI & workflow automation company with 16+ years of experience building custom AI-enabled workflow automations for SMBs and Enterprises, specializing in agentic AI, LLM integrations, and CRM/ERP sync across Healthcare, FinTech, eCommerce, Manufacturing, and Real Estate. Explore 30+ free templates at intuz.com/n8n-workflow-automation-templates or get a custom workflow built at intuz.com/get-started.

* **Website:** https://www.intuz.com/n8n-workflow-automation-templates/
* **Email:** [getstarted@intuz.com](mailto:getstarted@intuz.com)
* **LinkedIn:** https://www.linkedin.com/company/intuz/
* **Get Started:** https://n8n.partnerlinks.io/intuz

## For Custom Workflow Automation

[Click here - Get Started](https://www.intuz.com/get-started/)
