# Security

/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */

package security12;
import java.util.*;
/**
 *
 * @author STUDENT
 */
public class Security12 {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        Scanner sc = new Scanner (System.in);

        //System.out.println(p);
        //key matrix declaration
        String[][] playfair = new String[5][5];
        
        //the user input and build of the matrix
        String key = sc.next();
        
        for (int i = 0; i < key.length(); i++){
            for (int j = 0; j < key.length(); j++){
                StringBuilder temp = new StringBuilder();
                temp.append(key.charAt(i));
                playfair[i][j] = temp.toString();
            }
        }
        
        //completing the matrix
        for (int i = 0; i < 5; i++){
           for(int j = 0; j < 5; j++){
               if(playfair[i][j] == null && playfair[i][j].length() > 0){
                   playfair[i][j] = "a";
               }
           }
        }
        
        //printing the matrix
        for (int i = 0; i < 5; i++){
           for(int j = 0; j < 5; j++){
               System.out.println(playfair[i][j]);
           }
        }
        
//        //splitting the P
//        ArrayList<String> split = new ArrayList<String>();
//        
//        //Plain text input
//        String p = sc.nextLine();
//        p = p.toLowerCase();
//        
//        int count = 0;
//        for (int j = 0; j < p.length()-1; j++){
//            StringBuilder temp = new StringBuilder();
////                    if((p.length() % 2 == 1) && (i == p.indexOf(p.charAt(p.length() - 1)))){
////                        temp.append(p.charAt(i+1));
////                    }else{
////                        
////                    }
//            temp.append(p.charAt(j));
//            temp.append(p.charAt(j+1));
//                    
//                    
//            if (count == 2){
//                count = 0;
//                split.add(temp.toString());
//            }else{
//                count ++;
//            }
//                    
//        }
//
//        
//        for(int i = 0; i < split.size(); i++){
//            System.out.println(split.get(i));
//        }
//        
////        for(int i = 0; i < 5; i++){
////            for(int j = 0; j < 5; j++){
////                
////            }
////        }
        
        
    }
    
}
