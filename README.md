<?php 
$anzeige = false;
if(isset($_POST['rechnen'])){
    $height = $_POST["height"];
    $weight = $_POST["weight"];
    $erg = sqrt($height * $weight / 3600);
    $ergebnis = round($erg, 2);
    $anzeige = true;
    echo "<p>Your body surface is: $ergebnis m²</p>";
  }

?>


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Body Surface</title>
    <link rel="stylesheet" href="css/style.css">
    <link rel="stylesheet" href="css/mobil.css"> 
</head>
<body>
    <?php 
    if($anzeige == false) {

    ?>
    <form action="Köperoberfläche.php" method="POST">
    <h2>Body Surface</h2>   
        <label for="input1">Height</label> 
            <input type="number" class="hei" name="height" placeholder="h" value="<?php if(isset($height))  echo $height; ?>" required><br>
        <label for="input2">Weight</label>
            <input type="number" class="wei" name="weight" placeholder="w" value="<?php if(isset($weight))  echo $weight ?>" required><br>
    <input type="submit" name="rechnen" value="los!">
    
    </form>
    <?php 
    } ?>
    <?php 
    if($anzeige) {
        echo '<br><a href="Köperoberfläche.php"> another bill </a>';
    }
    
    ?>
    
</body>
</html>
<style>
form {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  background-color: #f9f3e6;
  padding: 20px;
  border-radius: 10px;
}
label {
  margin: 10px 0;
  font-weight: bold;
}
input[type=number] {
  padding: 10px;
  border: none;
  border-radius: 5px;
  background-color: #f2eee8;
  font-size: 16px;
  color: #333;
  text-align: center;
  width: 100%;
  max-width: 300px;
}
input[type=submit] {
  padding: 5px;
  border: none;
  border-radius: 5px;
  background-color: #ffcb9a;
  font-size: 16px;
  color: #fff;
  cursor: pointer;
  transition: all 0.3s ease-in-out;
  width: 100%;
  max-width: 300px;
}
input[type=submit]:hover {
  background-color: #ffbd4a;
}
</style>
