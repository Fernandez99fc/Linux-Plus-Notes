OBJECTIVES
--
INSTALL THE APACHE WEB SERVER ROLE IN CENTOS AND UBUNTU.
LOCATE APACHE CONFIGURATION FILES.

INSTALLING APACHE IN CENTOS
--
TO INSTALL APACHE, WE FIRSTLY HAVE TO INSTALL HTTP PACKAGE;
YUM INSTALL HTTPD.
YOU CAN USE;
rpm -ql httpd | less- TO VIEW FILES INSTALLED WITH HTTPD,Q TO QUERY AND L TO LIST.
HTTPD CONFIG FILE;
/ETC/HTTPD/CONF/HTTPD.CONF

INSTALLING APACHE IN DEBIAN/UBUNTU
--
THE PACKAGE IS CALLED APACHE2 IN DEBIAN BASED.
APT-GET INSTALL APACHE2
/ETC/APACHE2/APACHE2.CONF
THERE ARE OTHER FILES IN THE DIRECTORY;/ETC/APACHE2
/ETC/PORTS.CONF IS A DIFFERENT FILE FOR CONFIGURING LISTENING PORTS.
ADD TO FIREWALL
