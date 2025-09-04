# non-repeating-numbers-day17-of-my-gfg-challange
class Solution {
  public:
    char nonRepeatingChar(string s) {
     int freq[26] = {0};
      
      for(char c:s){
          freq[ c -'a']++;
      }
       for(int i = 0; i<s.size(); i++){
       if(freq[s[i]-'a']==1){
       return s[i];
             }
       }
          return '$';
          }
   };
