# Totally Random Mail Server Config Notes

* All mail is stored as user id 1002 and group id 1002
* Mail stored in maildir format
* Maildirs is in the path: `/home/mailbox/$DOMAIN/$USER`
  * eg. `user@mail-domain.com` is stored in `/home/mailbox/mail-domain.com/user`
* smtp with optional tls enabled in Postfix (smtp/port 25)
* imap over tls enabled in Dovecot (imaps/port 993)
* sasl over tls enabled in Postfix (submission/port 587)

