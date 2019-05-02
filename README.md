# php-codeacedmy
World Traveler
Hello there, friend! We’re exhausted having just returned to New York City from a whirlwind of world travel. We’re bringing all our international currency to the bank to be exchanged for USD. Our travels have made us wise and weary, and we want to ensure we’re being treated fairly. Can you help?

Write a program to calculate exactly how much cash in USD we should end up with after it has all been exchanged



<?php
  
$riel = 2103942;
$kyat = 19092;
$krones = 109;
$lek = 9094;

echo "At the start of transaction we had $riel riel, $kyat kyat, $krones krones, and $lek lek.";

$Riel_to_USD= 0.00026*$riel;
$Kyat_to_USD= 0.00066*$kyat;
$Krones_to_USD= 0.11*$krones;
$Lek_to_USD= 0.0090*$lek;

echo "\n
remaining ${riel} riel are:$Riel_to_USD usd. 
\n
remaining ${kyat} riel are:$Kyat_to_USD usd.
\n
remaining ${krones} krones are:$Krones_to_USD usd.
\n
remaining ${lek} lek are $Lek_to_USD usd.";

$final_amount = $Riel_to_USD + $Kyat_to_USD + $Krones_to_USD + $Lek_to_USD-4;

echo "\n\nAfter deducting the transactions fees, you'll be recieving $final_amount usd.";

