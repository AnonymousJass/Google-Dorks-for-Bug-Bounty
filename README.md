# Google-Dorks-for-Bug-Bounty

Google Dorks for Bug Bounty
These are few Google Dorks which I have used in my Bug Hunting.


For Recon
If you are looking for new domains of any Target, take this text from footer of the websites and try this dork

intext:"© 2018 Sony Electronics Inc. All rights reserved"
For subdomains or different countries domains:-

site:"sony.com.*"
To find AWS S3 Buckets of any target:-

site:.s3.amazonaws.com "Sony"
For Login pages of any target

site:target.com intext:login intext:username intext:password

For Sensitive Information
Sensitive information like Classified documents, users credentials, API secrets, System information in metadata, etc. 


For passwords or any sensitive information's in documents with extension "ppt". You can change extension in "ext" to any extensions like "pdf", "docx".

site:*.com ext:ppt intext:password
site:*.com filetype:xls inurl:"email.xls"

Generated pdf, images, docx files have system information in their title or inside the document as a metadata. It might be System username, internal directory path.

c:\Users\ site:*.target.com filetype:pdf
c:\Users\ site:*.target.com

Other useful Dorks:-

allintext:username filetype:log
inurl:/proc/self/cwd
"index of" "database.sql.zip"
site:target.com inurl:admin "@gmail.com"
inurl:zoom.us/j and intext:scheduled for
allintitle: restricted filetype:doc site:gov
intitle:"Index of" wp-admin
inurl:Dashboard.jspa intext:"Atlassian Jira Project Management Software"

Useful Links:-
This is the complete database of google dorks where everyday new google dorks are disclosed, so keep an eye on this :- https://www.exploit-db.com/google-hacking-database 

Github Repository:- https://gist.github.com/stevenswafford/393c6ec7b5375d5e8cdc

Tool - https://github.com/BullsEye0/dorks-eye 

Learn how to create google dorks from here- https://medium.com/infosec/exploring-google-hacking-techniques-using-google-dork-6df5d79796cf 
