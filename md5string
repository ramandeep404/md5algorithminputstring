import java.math.BigInteger;
import java.security.MessageDigest;
import java.security.NoSuchAlgorithmException;
import java.util.*;
// author raman
public class NewClass1 {
    public static String getMd5(String input)
    {
        String hashtext="Hash Text can't be generated";
        try {
  
            // Static getInstance method is called with hashing MD5
            MessageDigest md = MessageDigest.getInstance("MD5");
  
            // digest() method is called to calculate message digest
            //  of an input digest() return array of byte
            byte[] messageDigest = md.digest(input.getBytes());
  
            // Convert byte array into signum representation
            BigInteger no = new BigInteger(1, messageDigest);
  
            // Convert message digest into hex value
            hashtext = no.toString(16);
            while (hashtext.length() < 32) {
                hashtext = "0" + hashtext;
            }
            
        } 
  
       
        catch (Exception e) {
           System.out.println(e.toString());
        }
        return hashtext;
    }
  
 
    public static void main(String args[]) throws NoSuchAlgorithmException
    {
        Scanner sc=new Scanner(System.in);
        
        System.out.println("Enter a String to generate hash");
        String s = sc.next();
        System.out.println("Your HashCode Generated for " + s + " by MD5 is: " + getMd5(s));
    }
}
