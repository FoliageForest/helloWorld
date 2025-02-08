## ssh

ssh -i /root/.ssh/id_rsa root@192.168.8.1

     -i identity_file
             Selects a file from which the identity (private key) for public key authentication is read.
             The default is ~/.ssh/id_dsa, ~/.ssh/id_ecdsa, ~/.ssh/id_ed25519 and ~/.ssh/id_rsa.  Iden‐
             tity files may also be specified on a per-host basis in the configuration file.  It is pos‐
             sible to have multiple -i options (and multiple identities specified in configuration
             files).  If no certificates have been explicitly specified by the CertificateFile directive,
             ssh will also try to load certificate information from the filename obtained by appending
             -cert.pub to identity filenames.
