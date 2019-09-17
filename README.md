# Server-Certificate


<img src="https://github.com/kabir55/Server-Certificate/blob/master/Install%20server%20certificate.PNG"> 


we'll show how to create the Server Certificate, get it signed and
install signed Server Certificate with a private key
in the location specified by the where is server configuration file.
We use tools provided by AWS MI image instance,
and then, also the Apache web server, as an example.
Create a server certificate directly first.
And then, we cd, changing to the directory.
We run the /etc/pki/tls/misc/CA scripts,
with option new request.
To generate the private and public key pair,
the script will then ask us to enter the subject name field.
We will try to hit Enter for all the default values or
enter your own site information, as required.
Common name subfield should be used
with a server domain name or the *.,
followed by the domain name of the organizations.
Here * is the wildcard character.
It is critical to be exact here, since the browser
will match the common name presented by the server
in the certificate with the DNS reverse lookup of
the IP address used by the server in the HTTP response.
Using wildcard * followed by the domain name allow us,
the webmaster, to use different server domain name,
without having to matching it exactly.
It can be anyone with a domain name in the subnet.
We only send the generated newreq.pem file,
which contains the certificate request for CA to sign. 
