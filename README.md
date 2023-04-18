# k-peroberflache
Meine erstes projekt


<?php
echo "Das ist Aufgabe 1:";
echo "<br>";  
for($f=0;$f<=100;$f++){
    echo $f ."<\n>" ;
    
}



echo "<br>";echo "<br>";echo "<br>"; 
echo "Das ist Aufgabe 2:";
echo "<br>";
$Letters = array("Aa", "Bb", "Cc", "Dd","Ee", "Fe", "Gg", "Hh", "Ii", "Jj", "Kk", "Ll", "Mm", "Nn", "Oo", "Pp", "Qq", "Rr", "Ss", "Tt", "Uu", "Vv", "Ww", "Xx", "Yy", "Zz");
$conunt = count($Letters);
$x= 0;
while($x < $conunt){
    echo $Letters[$x] . ' ';
    $x++;
    
}
    
echo "<br>";echo "<br>";echo "<br>"; 
echo "Das ist Aufgabe 3:";
echo "<br>";
$wert=11;
do {
    echo $wert . "PHP macht Spaß <br>";
    $wert--;
}while($wert > 5);
echo "<br>";echo "<br>";echo "<br>"; 
echo "Das ist Aufgabe 4:";
echo "<br>";
$cars = [
    "BMW" => "7er",
    "Mercedes" => "A-Klass",
    "Nissan" => "X-Trail"
];
foreach($cars as $key=>$pairs) {
    echo " Die beste Auto von $key ist $pairs . <br> ";
    
}

echo "<br>";echo "<br>";echo "<br>"; 
echo "Das ist Aufgabe 5: <br> •	1.Die große untershid ist, dass unser geschikte data mit Get im browser sichbar sind.
 <br> •	2.Per Post kann große menge als Get geschickt werden.";
echo "<br>";

echo "<br>";echo "<br>";echo "<br>"; 
echo "Das ist Aufgabe 6:";
echo "<br>";



?>
