# cisco7
**cisco7** is simple class to encrypt or decrypt Cisco Type 7 passwords, implemented in native PHP. Licensed under GPLv3.

## Install
Simply copy cisco7.php where you want and include it in your code.
```
require_once("cisco7.php");
```

## Usage (Static)
```
require_once("cisco7.php");
$o="example";
echo "Original.: ".$o."\n";
echo "Encrypted: ".($e=Cisco7::encrypt($o))."\n"; // 02031C5A06160324
echo "Decrypted: ".($d=Cisco7::decrypt($e))."\n"; // example
```

## Usage (Dynamic)
```
require_once("cisco7.php");
$c=new Cisco7();
$o="example";
echo "Original.: ".$o."\n";
echo "Encrypted: ".($e=$c->encrypt($o))."\n"; // 02031C5A06160324
echo "Decrypted: ".($d=$c->decrypt($e))."\n"; // example
```
