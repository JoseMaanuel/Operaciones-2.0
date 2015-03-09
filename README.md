# Operaciones-2.0

package operaciones;

import java.util.*;
public class Operaciones {

   
    public static void main(String[] args) {
       int a,b,op, s;
        Scanner lec=new Scanner(System.in);
       
        System.out.println("Escribe un numero");
        a=lec.nextInt();
        
        System.out.println("Escribe otro numero");
        b=lec.nextInt();
        do{
        System.out.println("seleccione la operacion a realizar");
        System.out.println("1)Suma \n 2)Resta \n 3)Multiplicacion \n 4)Division \n 5)Modular \n");
        op=lec.nextInt();
       
        switch(op){
            case 1:
                System.out.println("Suma");
                System.out.println(a+b);
                break;
            case 2:
                System.out.println("Resta");
                System.out.println(a-b);
                break;
            case 3:
                System.out.println("Multiplicacion");
                System.out.println(a*b);
                break;
            case 4:
                System.out.println("Division");
                System.out.println(a/b);
                break;
            case 5:
                System.out.println("Modular");
                System.out.println(a%b);
                break;
            default:
                System.out.println("La opcion es incorrecta");
                break;
        }
        System.out.println("¿Desea Salir?");
        System.out.println("1= Si   2= No");
        System.out.println("Ejiga una opcion");
        s=lec.nextInt();
        if(s==2){
           System.out.println("Este bien quedate dentro del programa");  
        }else {
            System.exit(0);
        }
    }while(op>5);
        
    }
}
