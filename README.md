# get-data-frome-user-form

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>

<?php

if(isset($_POST['submit'])){
        $name=$_POST['name'];
        $gender=$_POST['gender'];
        $department=$_POST['department'];
        $coder=$_POST['coder'];
}
if(empty($_POST['submit'])){
    $field = "please fullfill this user form";
    
}
if(empty($_POST['name'])){
    $field = "please fullfill this user form";
    
}
if(empty($_POST['gender'])){
    $field = "please fullfill this user form";
    
}
if(empty($_POST['department'])){
    $field = "please fullfill this user form";
    
}
if(empty($_POST['coder'])){
    $field = "please fullfill this user form";
    
}
if(isset($_POST['name'])){
    echo "User Name Is: ".$name;
}
echo "<br/>";
if(isset($_POST['gender'])){
    echo "User Is: ".$gender;
}
echo "<br/>";
if(isset($_POST['department'])){
    echo "User Department is: ".$department;
}
echo "<br/>";
if(isset($_POST['coder'])){
    echo "User Expert this language: ".$coder;
}






?>

    


<form action="" method="post">
<table>

<tr>
<td>User Name:</td>
<td>
<input type="text" name="name"  placeholder="USER NAME"/>
</td>
</tr>

<tr>
<td>Gender:</td>
<td>
        <input type="radio" name="gender"  value="Male">Male
        <input type="radio" name="gender"  value="Female">Female
</td>
</tr>

<tr>
<td>Department:</td>
<td>
        <input type="checkbox" name="department"  value="CSE">CSE
        <input type="checkbox" name="department"  value="Math">Math
        <input type="checkbox" name="department"  value="English">English
        <input type="checkbox" name="department"  value="EEE">EEE

</td>
</tr>

<tr>
<td>Expert Language:</td>
<td>
       <select name="coder" require="1">

            <option value=" ">Select One</option>
            <option value="PHP">PHP</option>
            <option value="JAVA">JAVA</option>
            <option value="C#">C#</option>
            <option value="C++">C++</option>

     </select>

</td>
</tr>
<tr>
<td></td>
<td>
<input type="submit" name="submit" value="submit">
<input type="reset" name="reset" value="clear">

</td>
</tr>

</table>
</form>
</body>
</html>
