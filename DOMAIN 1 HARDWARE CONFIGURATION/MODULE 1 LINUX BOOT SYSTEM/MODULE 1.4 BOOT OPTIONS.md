# OBJECTIVES--------

1)Booting with ISO

2)Understandign the different Options for accessing an ISO

3)Understand how systems boot from NFS

An ISO Image is  a file holding the content of an optical disc,DVD/CD. Having the data in a file format rather than a physical cd/dvd which can distribute the data easily. We can also access the ISO file remotely to install an operating system on a computer.

# ISO REMOTE ACCESS METHODS

Remote access to the ISO Image can be made through the http or ftp. Using FTP allows data to be transferred bit-by-bit and can be secure using SFTP(SECURE FILE TRANSFER PROTOCOL)using the SSH 22 Port. HTTP Allows connection over port 80.

# (NFS).
It is a remote booting method that uses NETWORK FILE SYSTEM. A computer boots with a kernel image or gets one from the TFTFP server (like PXE). Next the system will connect to the NFS server on the network and access the root file system
