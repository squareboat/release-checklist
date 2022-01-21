1. All API’s have backend validations as needed
1. All API’s are sending a response within 2000 ms.
1. Sitemap.xml is working and getting refreshed periodically. Sitemap index files may not list more than 50,000 Sitemaps and must be no larger than 50MB (Sitemap standards defined here: https://www.sitemaps.org/index.html)
1. Sneaker is installed and configured (For PHP Projects only)
1. Database backup script (Spatie) has been configured (For Laravel only)
1. Backups of database and user uploaded files is working
1. Backups restoration is working
1. .env.example and .env are in sync (For Laravel only)
1. Postman collection has been pushed to docs/ folder (if applicable)
1. Latest crontab backup is included in the docs/ folder (Take help from Devops if needed)
1. MySQL indexes have been added to all tables (Take help from Devops if needed)
1. No commented code is included in the codebase
1. User uploads
1. Images are being compressed
1. Original photos are being maintained
1. All third party API and webhook interactions (SMS services, CRM’s etc.) are being logged for both request and response
1. Basic page audits have been done in Laravel DebugBar (For Laravel only)
1. Persistent XSS is not occuring and tested across all application inputs, such as forms, URL parameters, hidden fields and cookie values
1. X-Frame-Options, X-XSS-Protection and X-Content-Type-Options headers have been set (Test using Chrome Developer Console or securityheaders.io)
1. Passwords have been hashed in the database, using bcrypt etc. (Do NOT use MD5, SHA1 etc.)
1. Queues have been configured on SQS
1. Basic SQL injection checks have been performed
1. Basic CSRF checks have been performed
1. Email is being sent to the user incase of password change
1. The system does not allow any .php or any executable file to be uploaded
1. All failed login attempts have been logged
1. Cookies are secure and httponly and encrypted
1. Admin cannot login via the standard login page
1. Admin login has a captcha
1. Changing a user’s email requires him to re-enter his password
1. Strong password policy of minimum 6 characters
1. File uploads are not being stored in a publicly accessible directory on the server
1. Reset password link expires after 1 hour
1. Resend OTP should not work within 1 minute of previous OTP send
1. The re-sent OTP should be same as previous OTP for 10 minutes
1. There should be a limit on the number of times the OTP can be requested.
1. Signup emails should not be from temporary email providers.
1. Bounce handling URL has been provided
