<?php
	$a=array(1,2,3,4,5);
  $number=6;
  
  
  function clock_wise($a,$n)
  {
      $count=$n;
      $remain=(count($a)-1)-$n;
	    $i=count($a)-1;
	    $temp=array();
	    while($count>0){
	      array_push($temp,$a[$i]);
	      $i=$i-1;
	      $count=$count-1;
	    }
	    
	    $j=0;
	    while($remain>=0)
	    {
	      array_push($temp,$a[$j]);
	      $j=$j+1;
	      $remain=$remain-1;
	    }
	    
	    return $temp;
    
  }
  print_r(clock_wise($a,$number));
	    

?>
