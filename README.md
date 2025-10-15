# Sales_Agent
Our first Agentic Framework project!!  Prepare yourself for something ridiculously easy.  We're going to build a simple Agent system for generating cold sales outreach emails: 
1. Agent workflow
2. Use of tools to call functions
3. Agent collaboration via Tools and Handoffs
   
## Before we start - some setup:

Please visit Sendgrid at: https://sendgrid.com/

(Sendgrid is a Twilio company for sending emails.)

Please set up an account - it's free! (at least, for me, right now).

Once you've created an account, click on:

Settings (left sidebar) >> API Keys >> Create API Key (button on top right)

Copy the key to the clipboard, then add a new line to your .env file:

`SENDGRID_API_KEY=xxxx`

And also, within SendGrid, go to:

Settings (left sidebar) >> Sender Authentication >> "Verify a Single Sender"  
and verify that your own email address is a real email address, so that SendGrid can send emails for you.

#### Certificate error

If you get an error SSL: CERTIFICATE_VERIFY_FAILED then  
First run this: `!uv pip install --upgrade certifi`  
Next, run this:
```python
import certifi
import os
os.environ['SSL_CERT_FILE'] = certifi.where()
```

#### Other errors or no email

If there are other problems, you'll need to check your API key and your verified sender email address in the SendGrid dashboard

(Or - you could always replace the email sending code below with a Pushover call, or something to simply write to a flat file)

## Remember to check the trace

https://platform.openai.com/traces

And then check your email!!

### Handoffs represent a way an agent can delegate to an agent, passing control to it

Handoffs and Agents-as-tools are similar:

In both cases, an Agent can collaborate with another Agent

With tools, control passes back

With handoffs, control passes across

### Remember to check the trace

https://platform.openai.com/traces

And then check your email!!
