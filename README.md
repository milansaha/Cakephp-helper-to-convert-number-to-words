Cakephp-helper-to-display-number-to-words
=================================================

In my last application, i was in need to show numbers in words. So while i was roaming arround in web got a php method 
here http://www.karlrixon.co.uk/writing/convert-numbers-to-words-with-php/ . Then using this method i made a cakephp
helper to solve my purpose. 

Step 1: 
   Download the number_to_word.php script and keep it in app/views/helpers/ 

Step 2: Load this helper in the desired controller or in appcontroller.

  <?php
  
    class BakeriesController extends AppController {
    
      var $helpers = array('NumberToWord'); 
      
    }
    
  ?>
  
Step 3: Now in the follwoing way you can use in your cakephp view

  <?php 
  
    echo $this->NumberToWord->convert_number_to_words(8769); 
    
    //eight thousand,seven hundred and sixty nine
    
  ?>
