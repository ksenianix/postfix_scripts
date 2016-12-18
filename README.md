 Add new hosted domains to Postfix automaticaly 
Make it a cron job and it will add new domains to postfix automatically.

Add new hosted domains as new lines to domains.txt file in users home folder.
Change variable myuser to user name that will add new domains to domains.txt file
set variable main_domain to domain name of your Mail server.
Check Postfix's main.cf to have next lines:
virtual_mailbox_domains = hash:/etc/postfix/virtual_mailbox_domains
virtual_alias_maps = hash:/etc/postfix/virtual
