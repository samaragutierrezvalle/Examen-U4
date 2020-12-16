# Examen-U4
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner leer = new Scanner(System.in);
         ArbolBinario arbolito =new ArbolBinario();
         ArbolEspejo arbolito2=new ArbolEspejo();
         int elemento,opc;
         System.out.println("*************************************");
         System.out.println("          Examen de Unidad");
         System.out.println("**************************************");
         do{
         
         System.out.println("ingresa el numero del nodo");
         elemento=leer.nextInt();
         arbolito.agregarNodo(elemento);
         arbolito2.agregarNodo(elemento);
         
         System.out.println("¿Deseas agregar otro nodo?\n1->SI\n2->no");
         opc=leer.nextInt();
         
         }while(opc==1);
         if(opc >1){
             System.out.println("Recorrido InOrden");
             if(!arbolito.estaVacio()){
                    
                    arbolito.inOrden(arbolito.raiz);
                }
                else {
                    System.out.println("El Arbol esta vacio");
                }
             System.out.println("\nRecorrido en PreOrden");
             if(!arbolito.estaVacio()){
                  
                    arbolito.preOrden(arbolito.raiz);
                }
                else {
                    System.out.println("El Arbol esta vacio");
                }
             System.out.println("\nRecorrido en PostOrden");
              if(!arbolito.estaVacio()){
               
                    arbolito.postOrden(arbolito.raiz);
                }
                else {
                    System.out.println("El Arbol esta vacio");
                }
              
              
              System.out.println("\n*****************Arbol espejo****************************** ");
               System.out.println("Recorrido InOrden");
             if(!arbolito2.estaVacio()){
                    
                    arbolito2.inOrden(arbolito2.raiz);
                }
                else {
                    System.out.println("El Arbol esta vacio");
                }
             System.out.println("\nRecorrido en PreOrden");
             if(!arbolito2.estaVacio()){
                  
                    arbolito2.preOrden(arbolito2.raiz);
                }
                else {
                    System.out.println("El Arbol esta vacio");
                }
             System.out.println("\nRecorrido en PostOrden");
              if(!arbolito2.estaVacio()){
               
                    arbolito2.postOrden(arbolito2.raiz);
                }
                else {
                    System.out.println("El Arbol esta vacio");
                }
         }
         
         
    }
}
