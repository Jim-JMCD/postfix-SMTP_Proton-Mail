## Guide for installing, configuring and using Linux Postifix with Proton Mail secure SMTP. 
### Currently being edited and merged with Scaleway documentation

This guide describes how setup up Postfix to work with Proton secure SMTP providing system, security and application administrators use of system utilities that are mail enabled and software like sendmail, postfix, mailx and mutt to send reports, alerts and other material to people that presumably care.

The SMTP service can only send mail using a custom domain registered in a Proton Mail account. If the requirement includes receiving mails use mutt and the Proton Mail Bridge. 

There are other Linux command line mail services that can use SMTP credentials but they may have the limitation of not being able to be used with some Linux system utilities.

#### Summary
* How to test a SMTP TLS connection. 
* Getting the Proton Mail SMTP token.
* Installing and configuring postfix, the mail.cf file.
* Enabling SASL security, a TLS requirement.
* Enabling rewriting of local mails to the SMTP token user, this permits system and application accounts to use the SMTP mail service, useful for automation.  
* Section Notes & Mail Management covers:
  * The idiosyncrasies of using TLS/SASL enabled postfix;
  *	How setting up a SMTP mail-out service can cause catastrophic failure of a Linux box;
  *	Examples of Linux flavours having differing interpretations of what their command line mail facilities can do and some have replaced the old with utilities that are shinier.
  *	Plus, other interesting notes. 
*	Where to locate info for basic trouble shooting and security forensics.
*	An example using of using Ubuntu sendmail and mailx with a heredoc.  Heredocs demonstrate the versatility of the email clients. There is plenty on the internet how use Linux mail tools. 

Specific software installation instructions are not included in this guide because software package management varies between Linux flavours.  

[Postfix SMTP Proton Mail - Installation, Configuration and Usage Guide](https://github.com/Jim-JMCD/postfix-SMTP_Proton-Mail/blob/main/Postfix_SMTP_Proton-Mail_Guide.pdf)  
