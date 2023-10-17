⁸# Qwe0 сейчас я расскажу о PHP туда можно вписать программированные коды по типу <form method="post" action="<?php echo $_SERVER['PHP_SELF'];?>"> 
        Name: <input type="text" name="fname"> 
        <input type="submit"> 
    </form> 
  
    <?php 
        if ($_SERVER["REQUEST_METHOD"] == "POST") 
        { 
            $str = $_POST['fname']; 
              
            if (empty($str))  
            { 
              echo "String is empty"; 
            }  
            else 
            { 
    ?> 
               <h1> 
                 <?php echo $str ?> 
               </h1> 
    <?php 
            } 
        } 
    ?> 
</body> 
</html>
 типо такого
