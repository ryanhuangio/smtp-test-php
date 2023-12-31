# SMTP Test PHP

## Purpose

This simply script allows testing multiple SMTP connections. It is quicker than using Thunderbird and easier than using Telnet, and scales well when you have to bulk test SMTP.

## How to Use

1. Clone repo `git clone https://github.com/ryanhuangio/smtp-test-php.git`
2. Change directory `cd smtp-test-php`
3. Install dependencies `composer install`
4. Configure `env.php` and replace with your SMTP connection details.
5. Run `php smtp.php` and it will loop through each SMTP connection to check if it works by sending a test email.

If it sends successfully, you will see a message like:

```
$ php smtp.php
✅ Email sent from user@domain.com successfully!
❌ Email failed to send from user@gmail.com.
```
