OBJECTIVES
--
UNDERSTAND THE IMPORTANCE OF CERTIFICATE FOR ESTABLISHING TRUST.
EXPLAIN HOW A CETIFICATE AUTHORITY HELPS ESTABLISH TRUST.
NAME THE PORTS USED BY A CERTIFICATE AUTHORITY.

CERTIIFCATE AUTHORITY(CA) AND TRUST
--
THE CERTIFICATE AUTHORITY ROLE SERVES A MAJOR ISSUE WITH SECURITY: HOW CAN YOU TRUST THAT A WEBSITE YOU REACH IS THE REAL WEBSITE?
THE ANSWER IS DIGITAL CERTIFICATES THAT VALIDATES THE IDENTITY OF THE SERVER. DIGITAL CERTIFICATES ARE EITHER ISSUED OR SIGNED BY A CA AND THEREFORE THE CA CAN VERIFY THE CERTIFICATE

CERTIFICATES AND ENCRYPTION KEYS
--
A CERTIFICATE IS AN ENCRYPTED KEY ;WE LARGELY FOCUS ON ASSYMETRIC ENCRYPTION, WHICH USES TWO KEYS:
A PUBLIC KEY IS KNOWN BY EVERYONE; CAN ONLY BE DECRYPTED WITH THE PRIVATE KEY.
A PRIVATE KEY IS ALSO KNOWN BY THE OWNER; CAN ONLY BE DECRYPTED BY PUBLIC KEY.
     BY COMPARISON,A SYMMETRIC KEY IS A SINGLE KEY KNOWN TO BOTH PARTIES.
     GENERALLY, ASSYMETRIC ENCRYPTION IS USED TO ESTABLISH TRUSTED CONNECTION; CONNECTION CAN THEN BE USED TO EXCHANGE A SYMMETRIC KEY. 

CA IN DETAIL
--
THE CA CAN ISSUE CERTIFICATES TO A WEB SERVER OWNER.
ALTERNATIVELY, THE OWNER SENDS A CERTIFICATE SIGNING REQUEST(CSR) TO THE CA.
THE CA SIGNS THE CERTIFICATES WITH ITS OWN PRIVATE KEY.

REMEMBER:PRIVATE KEY CAN ONLY BE DECRYPTED BY A PUBLIC KEY.
REMEMBER: EVERYONE CAN ACCESS THE PUBLIC KEY.
THEREFORE, ANYONE CAN DECRYPT THE SIGNATURE OF THE CERTIFICATE AND VERIFY.

CA AND PORTS
--
A CA CAN BE USED FOR CERTIFICATES BEYOND SSL/TLS (WEB) CERTIFICATES.
- DIFFERENT PORTS CAN BE USED ON A CERTIFICATE AUTHORITY BASED ON THE CERTIFICATES IT ISSUES.

WE'VE COVERED SSL/TLS WEB SERVERS, WHICH COULD COMMUNICATE WITH A CA VIA PORT 443: HOWEVER:
- FOR LDAP THE CA MIGHT USE PORT 389 OR 636.
- IMPORTANT TO LOOK AT THE PORTS REQUIRED TO COMMUNICATE WITH THE CA FOR EACH APPLICATION.

SYMMETRIC ENCRYPTION VS ASSYMETRIC ECNRYPTION-
--
FOR TWO COMPUTERS TO EXCHANGE MESSAGE OVER THE INTERNET SECURELY, THE MESSAGE HAS TO BE ENCRYPTED BECAUSE THE INTERET IS PUBLIC. SO TO ACHIEVE THIS, WE USE EITHER SYMMETRIC  OR ASSYMETRIC ENCRYPTION.
SYMETTRIC ENCRYPTION IS WHEN A SECRET KEY IS USED TO ENCRYPT THE DATA BY THE SENDER AND ALSO USED TO DECRYPT THE DATA BY THE RECEIVER. WHICH MEANS, THE SECRET KEY IS KNOWN BY THE TWO COMPUTERS. HUMANS CAN MEET IN A PRIVATE PLACE TO AGREE ON A SECRET KEY TO BE USED, BUT COMPUTERS CAN'T BECAUSE IT IS DONE OVER THE INTERNET WHICH IS PUBLIC, SO COMPUTERS CANT AGREE ON A SECRET KEY TO USE OVER THE INTERNET, THAT IS WHY THERE IS ASSYMETRIC ENCRYPTION.
AS FOR ASSYMETRIC ENCRYPTION, TWO COMPUTERS DON'T HAVE TO MEET TO EXCHANGE A SECRET KEY, THE SENDER USES A PUBLIC KEY TO ENCRYPT THE MESSAGE AND THE RECEIVER USES A PRIVATE KEY TO DECRYPT THE MESSAGE. HERE, THE PUBLIC CAN BE KNOWN TO ANYONE OVER THE INTERNET AND THEY CAN USE IT TO ENCRYPT A MESSAGE, BUT ONLY THE RECEIVER HAS A KEY TO DECRYPT THE MESSAGE. THINK OF IT LIKE SENDING A MESSAGE TO MAIL BOX, EVERY PERSON HAS THE KEY TO SEND A MESSAGE TO THAT MAIL BOX, BUT ONLY THE RECEIVER HAS THE KEY TO READ THE MESSAGE INTENDED FOR HIM.