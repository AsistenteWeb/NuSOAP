AsistenteWeb - nuSOAP
=====================

AsistenteWeb/nuSOAP based in NuSphere NuSOAP.

This is a set of PHP classes.  
No PHP extensions required!!!

Create and consume web services based on:
- SOAP 1.1
- WSDL 1.1 
- HTTP 1.0/1.1. and more

Installation
------------
``` json
{
    "require": {
        "asistenteweb/nusoap": "dev-master"    

    }
}
```
To actually install AsistenteWeb/nuSOAP in your project, download the composer binary and run it:

``` bash
wget http://getcomposer.org/composer.phar
# or
curl -O http://getcomposer.org/composer.phar

php composer.phar install
```

Use it
------
``` php
use Aw\Nusoap\NusoapClient;

       $client = new NusoapClient("https://yourserver.org?wsdl", true);
       $result = $client->call('method', $variables);
``` 


Important!
----------
If you want to read the documentation, keep in mind all clases were rewritten with CamelCase, for example:  
previously: nusoap_client
now became: NusoapClient
 

Documentation
--------------
http://sourceforge.net/projects/nusoap/files/nusoap-docs/0.9.5/nusoap-docs-0.9.5.zip/download

TODO
----
- Rewrite Documentation
- Rewrite Samples
- Test
