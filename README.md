# Primos
Ingresa un numero para descomponerlos en los primos que puede ser multiplicado 
mi nombre es franco
Programa para ingresar y reducir matrices soy un programador nuevo sin experiencia que esta intentando aprender lo mas rapido que pueda revisar el codigo y cambiar o sugerir lo que te parezca, cualquier opinion ayuda mucho
package primosapp;

import clasesP.modulosPrimos;
import java.util.Scanner;


/**
 *
 * @author Franco
 */
public class PrimosApp {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        
        Scanner dato = new Scanner(System.in) ;
        
        int numeroVueltas , repetidor , anterior = 0 ;
        
        System.out.println( "ingresa la cantidad de numeros a analizar");
        
        repetidor = dato.nextInt() ;
        
        for ( int c = 0 ; c < repetidor ; c++ ){ 
        
            System.out.println( "Ingresa el numero a analizar");
        
            numeroVueltas = dato.nextInt() ;
            
            if ( anterior < numeroVueltas ){
                
                modulosPrimos.encontrarPrimos( numeroVueltas );
                
                anterior = numeroVueltas ;
                
            }
        
            modulosPrimos.buscarPrimos( numeroVueltas );
            
            modulosPrimos.mostrarResultado();
            
        }
    
    }
    
}
