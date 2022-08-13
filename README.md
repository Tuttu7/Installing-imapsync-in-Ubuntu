#### Here is  the command to install imapsync dependencies, you need root privilege to run them.


```
apt-get install  \
libauthen-ntlm-perl     \
libclass-load-perl      \
libcrypt-openssl-rsa-perl \
libcrypt-ssleay-perl    \
libdata-uniqid-perl     \
libdigest-hmac-perl     \
libdist-checkconflicts-perl \
libencode-imaputf7-perl     \
libfile-copy-recursive-perl \
libfile-tail-perl       \
libio-compress-perl     \
libio-socket-inet6-perl \
libio-socket-ssl-perl   \
libio-tee-perl          \
libjson-webtoken-perl   \
libmail-imapclient-perl \
libmodule-scandeps-perl \
libnet-dbus-perl        \
libnet-ssleay-perl      \
libpar-packer-perl      \
libproc-processtable-perl \
libreadonly-perl        \
libregexp-common-perl   \
libsys-meminfo-perl     \
libterm-readkey-perl    \
libtest-fatal-perl      \
libtest-mock-guard-perl \
libtest-mockobject-perl \
libtest-pod-perl        \
libtest-requires-perl   \
libtest-simple-perl     \
libunicode-string-perl  \
liburi-perl             \
libtest-nowarnings-perl \
libtest-deep-perl       \
libtest-warn-perl       \
make                    \
time                    \
cpanminus
```


#### Install required Python modules using CPAN on your system

```

cpanm Crypt::OpenSSL::RSA Crypt::OpenSSL::Random --force
cpanm Mail::IMAPClient JSON::WebToken Test::MockObject 
cpanm Unicode::String Data::Uniqid
cpanm File::Tail CGI Crypt::OpenSSL::RSA JSON::WebToken::Crypt::RSA Regexp::Common Test::Deep

```



#### After completing the installation of required packages. Download latest imapsync code from its official Github repository on your local system.

```

git clone https://github.com/imapsync/imapsync.git

```

#### Navigate to newly cloned repository and install it with the following commands on your system.

```
cd imapsync
mkdir -p dist
make install

```

```
root@Tuttu:~/imapsync/imapsync# imapsync -version
2.200
```
