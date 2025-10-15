# Sales_Agent
Our first Agentic Framework project!!  Prepare yourself for something ridiculously easy.  We're going to build a simple Agent system for generating cold sales outreach emails: 1. Agent workflow 2. Use of tools to call functions 3. Agent collaboration via Tools and Handoffs
## Before we start - some setup:


Please visit Sendgrid at: https://sendgrid.com/

(Sendgrid is a Twilio company for sending emails.)

If SendGrid gives you problems, see the alternative implementation using "Resend Email" in community_contributions/2_lab2_with_resend_email

Please set up an account - it's free! (at least, for me, right now).

Once you've created an account, click on:

Settings (left sidebar) >> API Keys >> Create API Key (button on top right)

Copy the key to the clipboard, then add a new line to your .env file:

`SENDGRID_API_KEY=xxxx`

And also, within SendGrid, go to:

Settings (left sidebar) >> Sender Authentication >> "Verify a Single Sender"  
and verify that your own email address is a real email address, so that SendGrid can send emails for you.
