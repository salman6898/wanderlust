To install and configure the Email Extension Plugin in Jenkins, follow these steps:

Installing the Email Extension Plugin
Log in to Jenkins:

Open your Jenkins dashboard in your web browser.

Navigate to Plugin Manager:
Go to Manage Jenkins from the sidebar.

Click on Manage Plugins.

Install the Email Extension Plugin:
In the Available tab, use the search box to find the "Email Extension Plugin".

Check the checkbox next to the "Email Extension Plugin".

Click the Install without restart button at the bottom of the page, or if you prefer, Download now and install after restart.
Configuring the Email Extension Plugin

Global Configuration:
After the plugin is installed, go back to the Manage Jenkins page.

Click on Configure System.

Configure SMTP Server:
Scroll down to the Extended E-mail Notification section.
Fill in the SMTP server details:

SMTP server: The address of your SMTP server (e.g., smtp.example.com).

Default user E-mail suffix: The default domain for email addresses (e.g., @example.com).

SMTP Port: The port your SMTP server uses (commonly 25, 465, or 587).

Use SMTP Authentication: 
Check this if your SMTP server requires authentication.

User Name: Your SMTP username

Password: Your SMTP password.

Use SSL: Check this if your SMTP server uses SSL.

Use TLS: Check this if your SMTP server uses TLS.

Default Content:
You can set default email content for all jobs here, such as subject and body templates.
Test Configuration:

Use the Test configuration by sending test e-mail section to send a test email to verify that your settings are correct.
Save the Configuration:

Click Save at the bottom of the page to apply your changes.
Using Email Extension Plugin in Pipelines
With the plugin installed and configured, you can use the emailext step in your pipeline scripts. Here's a sample script that includes the usage of emailext:

Summary:
Install the Email Extension Plugin through the Jenkins Plugin Manager.

Configure SMTP Server Settings in Jenkins global configuration to enable email notifications..

Use the emailext step in your pipeline script to send emails on build success or failure, attaching relevant reports.
