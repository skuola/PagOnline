# PagOnline
Igfs payment gateway sdk


#Install

`composer require skuola/pagonline`

#Usage

###Verify transaction
```
<?php

include ('vendor/autoload.php');

//Verify transaction

use PagOnline\init\IgfsCgVerify;

$verify = new IgfsCgVerify();

$verify->serverURL = "server url";
$verify->tid = "terminal id";
$verify->kSig = "signature";
$verify->timeout = "timeout";

$verify->shopID    = "ShopID";
$verify->paymentID = "PaymentID";

var_dump("Result", $verify->execute());

```
