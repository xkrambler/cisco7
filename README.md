# cisco7
**cisco7** is simple class to encrypt or decrypt Cisco Type 7 passwords, implemented in native PHP. Licensed under GPLv3.

## Install
Simply copy cisco7.php where you want and include it in your code.
```
require_once("cisco7.php");
```

## Usage
```
require_once("cisco7.php");
$c=new Cisco7();
$o="example";
echo "Original.: ".$o."\n";
echo "Encrypted: ".($e=$c->encrypt($o))."\n"; // 02031C5A06160324
echo "Decrypted: ".($d=$c->decrypt($e))."\n"; // example
```
