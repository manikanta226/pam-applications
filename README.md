# pam-applications
configuring su command using pam libraries.

sample configuration file to add /etc/pam.d/ directory.

For Normal su : /etc/pam.d/su

  auth  sufficient   pam_rootok.so

  auth  required     pam_unix.so 

  account required pam_unix.so 

  session required        pam_env.so readenv=1 

  session optional        pam_mail.so nopen


compile and check for any platform.
