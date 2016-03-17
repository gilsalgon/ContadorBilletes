# ContadorBilletes
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package contadorbilletes;

import java.io.InputStream;

/**
 *
 * @author Gsalazar
 */
public class ContadorBilletes {

    /**
     * @param monto
     * @param args the command line arguments
     */
    public static void contador(int monto) {
        int Diezmilcolon=0, Cincomilcolon=0, Dosmilcolon=0, Milcolon=0, Quinientoscolon=0, 
                Ciencolon=0, Cincuentacolon=0, Veinticincocolon=0, Diezcolon=0, Cincocolon=0; 
        // TODO code application logic here
        //calculo billettes de 10000
        Diezmilcolon=monto/10000;
        monto=monto-(Diezmilcolon * 10000);
        //calculo billetes de 5000
        Cincomilcolon=monto/5000;
        monto=monto-(Cincomilcolon * 5000);
        //calculo billetes de 2000
        Dosmilcolon=monto/2000;
        monto=monto-(Dosmilcolon * 2000);
        //calculo billetes de 1000
        Milcolon=monto/1000;
        monto=monto-(Milcolon * 1000);
        //calculo monedas de 500
        Quinientoscolon=monto/500;
        monto=monto-(Diezmilcolon * 500);
        // calculo moneda de 100
        Ciencolon=monto/100;
        monto=monto-(Ciencolon * 100);
        // calculo moneda de 50
        Cincuentacolon=monto/50;
        monto=monto-(Cincuentacolon * 50);
        //calculo de moneda de 25
        Veinticincocolon=monto/25;
        monto=monto-(Veinticincocolon * 25);
        //calculo de moneda de 10
        Diezcolon=monto/10;
        monto=monto-(Cincuentacolon * 10);
        //calculo de moneda de 5
        Cincocolon=monto/5;
        monto=monto-(Cincocolon * 5);
        System.out.println();
        if(Diezmilcolon >0);{
        System.out.println("Billetes de 10000 colones:"+Diezmilcolon);//imprime la cantidad de billetes de 10000
        }if(Cincomilcolon >0);{
        System.out.println("Billetes de 5000 colones:"+Cincomilcolon);//imprime la cantidad de billetes de 5000
        }if(Dosmilcolon >0);{
        System.out.println("Billetes de 2000 colones:"+Dosmilcolon);//imprime la cantidad de billetes de 2000
        }if(Milcolon >0);{
        System.out.println("Billetes de 1000 colones:"+Milcolon);//imprime la cantidad de billetes de 1000
        }if(Quinientoscolon >0);{
        System.out.println("Monedas de 500 colones:"+Quinientoscolon);//imprime la cantidad de monedas de 500
        }if(Ciencolon >0);{
        System.out.println("Monedas de 100 colones:"+Ciencolon);// imprime la cantidad de monedas de 100
        }if(Cincuentacolon >0);{
        System.out.println("Monedas de 50 colones:"+Cincuentacolon);// imprime la cantidad de monedas de 50
        }if(Veinticincocolon >0);{
        System.out.println("Monedas de 25 colones:"+Veinticincocolon); //imprime la cantidad de monedas de 25
        }if(Diezcolon >0);{
        System.out.println("Monedas de 10 colones:"+Diezcolon); // imprime la cantidad de monedas de 10
        }if(Cincocolon >0);{
        System.out.println("Monedas de 5 colones:"+Cincocolon); //imprime la cantidad de monedas de 5
    }


    }

    ContadorBilletes(int numero) {
        throw new UnsupportedOperationException("Not supported yet."); //To change body of generated methods, choose Tools | Templates.
    }

    ContadorBilletes(InputStream in) {
        throw new UnsupportedOperationException("Not supported yet."); //To change body of generated methods, choose Tools | Templates.
    }

 }




-------------------------------------------------------------------------------------------------------------------------------------------------

/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package contadorbilletes;
import java.util.Scanner;


/**
 *
 * @author Gsalazar
 */
public class Main {
/**
 *
 * static ContadorBilletes contador = new ContadorBilletes(System.in);
    
 * @author Gsalazar
 */
    static Scanner ingreso = new Scanner(System.in);
    /**
     *
     * @param args
     */
    public static void main(String[] args){
        System.out.print("ingrese monto a procesar:  ");
        int numero = ingreso.nextInt();
    ContadorBilletes.contador(numero);
    /**     contador.ContadorBilletes(numero); */

    }
}

