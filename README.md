# anagram
import java.util.*;
public class Main{
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        String str1=sc.next();
        String str2=sc.next();
        char ch[]=str1.toCharArray();
        char ch1[]=str2.toCharArray();
        Arrays.sort(ch);
        Arrays.sort(ch1);
        int temp=0;
        if(ch.length==ch1.length){
            for(int i=0;i<str1.length();i++){
                if(ch[i]!=ch1[i]){
                    temp++;
                    break;
                }
            }
        }
        else{
            temp++;
        }
        if(temp==0){
            System.out.println("anagram");
        }else{
            System.out.println("not anagram");
        }
        
    }
}
