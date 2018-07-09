# Interview

I am posting popular interview question's solution which are paid in nature(sometimes)

interview question on interviewcake.com: "I like parentheticals (a lot). "Sometimes (when I nest them (my parentheticals) too much (like this (and this))) they get confusing." Write a function

<?php
$str = 'Sometimes (when I nest them (my parentheticals) too much (like this (and this))) they get confusing.';
findparenthesis($str,'(',')',10);

function findparenthesis($str,$character,$find,$place){
    $i=0;
    $new_str= '';
    $str_length = strlen($str);
    
    for($str_length;$str_lengh>$place;$place++){
        $new_str += $str[$place];
        if($str[$place] == $character){
          $i++;
        }elseif($str[$place] == $find){
          $i--;
        }
    
      if($i ==0){
        return $place
      }
    
    }

}

