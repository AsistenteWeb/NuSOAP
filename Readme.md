Esyst - NuSOAP
=====================

Esyst/nusoap based on NuSphere NuSOAP.

This is a fork of AsistenteWeb/NuSOAP with some bugs fixed, unfortunately my pull requests were not responded to.

See also: https://github.com/Esyst/PHP-Soap for a library that makes NuSoap compatible with the native Soapclient API (drop in replacement).

Create and consume web services based on:
- SOAP 1.1
- WSDL 1.1 
- HTTP 1.0/1.1. and more

Instalation
-----------
``` json
{
    "require": {
				"esyst/nusoap": "0.1.1"    
    }
}
```
To actually install Esyst/nusoap  in your project, download the composer binary and run it:

``` bash
wget http://getcomposer.org/composer.phar
# or
curl -O http://getcomposer.org/composer.phar

php composer.phar install
```

Use it
------
``` php
use Esyst\Nusoap\NusoapClient;

       $client = new NusoapClient("https://yourserver.org?wsdl", true);
       $result = $client->call('method', $variables);
``` 


Important!
----------
If you want to read the documentation, take in mind all clases were rewrited with CamelCase, for example:  
after: nusoap_client
now: NusoapClient
 

Documentation
--------------
http://sourceforge.net/projects/nusoap/files/nusoap-docs/0.9.5/nusoap-docs-0.9.5.zip/download

TODO
----
- Rewrite Documentation
- Rewrite Samples
- Test
