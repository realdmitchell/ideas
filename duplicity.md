Duplicity
======
Backup:
```
$ duplicity --no-encryption --ssh-askpass DIRECTORY sftp://username@server
```
Backup with GPG encryption:
```
$ duplicity --ssh-askpass --encrypt-key "GPG-KEY" DIRECTORY sftp://username@server
```
Restore (it automatically detects encryption and asks for GPG passphrase):
```
$ duplicity --ssh-askpass restore sftp://username@server . 
$ duplicity               restore file:///destination-dir-with-duplicity-files/ .
```
List files (if encrypted by GPG it asks for that passphrase):
```
$ duplicity --ssh-askpass list-current-files sftp://username@server
$ duplicity               file:///destination-dir-with-duplicity-files/ .
```
## Version 
* Version X.Y

## Contact
#### Developer/Company
* Homepage:  http://www.nongnu.org/duplicity/duplicity.1.html
* e-mail: 
* Twitter: [@twitterhandle](https://twitter.com/twitterhandle "twitterhandle on twitter")
* other communication/social media
