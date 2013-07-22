Reverse-Integer
===============

public class Solution {
    public int reverse(int x) {
        // Start typing your Java solution below
        // DO NOT write main() function
        
   boolean flag = false;
   
   if(x <0) flag = true;
   
   x = Math.abs(x);
   
   StringBuffer sb = new StringBuffer();
   int sum = 0;
   
   while(x>0){
      int last = x % 10;
       sum = sum * 10 + last;
       x = x / 10;
       
   }
   
   if(flag) return -sum;
   else return sum;
    }
}
