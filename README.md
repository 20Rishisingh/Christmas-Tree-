/* WAP to print Christmas tree of 08 lines as given below :-
                               * 
                              * * 
                             * * * 
                            * * * * 
                           * * * * * 
                          * * * * * * 
                         * * * * * * * 
                        * * * * * * * * 
                              * *
                              * *
                              * *
                              * *
*/



import java.util.*;
import java.io.*;

public class Main {
    public static void main(String[] args) {
        Scanner asd = new Scanner(System.in);
            int n = 8;
            int nsp = n-1, nc = 1;
            
            for (int row = 1; row <= 8; row++){
                    for (int sp = 1; sp <= nsp; sp++){
                            System.out.print(" ");
                    }
                    for (int col = 1; col <= nc; col++){
                            System.out.print("*"+" ");
                    }
                    nsp--; nc++;
                    System.out.println();
            }
            for (int i = 1;i<=(n/2);i++){
                    for (int j = 0;j<=n/2;j++){
                           System.out.print(" ");
                    }
                    for (int k = n/2; k <= (n/2)+1;k++){
                           System.out.print(" "+"*");
                    }
                    System.out.println();
            }
    }
}
