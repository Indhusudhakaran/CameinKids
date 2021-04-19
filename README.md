# CameinKids
Main Project - CAMERINKIDS
{% load static %}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>MASTER TUTOR REGISTRATION FORM</title>
</head>
<body>
         <center><b><h2>MASTER TUTOR REGISTRATION FORM </h2></b></br>
         <form action="\mastertutorreg" method="post">
             {% csrf_token %}
             <h3> Enter Master Tutor Name:<input type="text" name="mtname"></br></h3>
            <h3> Gender:<input type="radio" name="gender" value="male"> Male
                    <input type="radio" name="gender" value="female"> Female
                    <input type="radio" name="gender" value="other"> Other</br></h3>
             <h3> Enter Address:<input type="text" name="address"></br></h3>
             <h3> Enter Phone Number:<input type="text" name="phoneno"></br></h3>
             <h3> Enter  Email:<input type="text" name="email"></br></h3>
             <h3>Enter User Name:<input type="text" name="username"></br></h3>
             <h3>Enter Password:<input type="text" name="passwd"></br></h3>
             <h3>Enter Department:<input type="text" name="dpt"></br></h3>
             <h3>Enter Designation:<input type="text" name="desi"></br></h3>
             <input type="submit" name="button" name="Register" value="Register">
    <h2>{{success}}</h2>
         </form>
         </center>
         <a href="/mastertutor"><center>View Registered</center></a>

</body>
</html>
