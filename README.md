# Clase040516
package ejercicios0405;

public class Ejercicios0405 {

    public static void main(String[] args) {

        Solucionpff n = new Solucionpff();
        n.juegos();
        n.notas();
        n.notas_2();

    }

}

///////////////////////////
package ejercicios0405;

import java.util.Stack;

public class Solucionpff {

    Stack p = new Stack();

    public void juegos() {

        p.push("MU");
        p.push("Metin");
        p.push("Linage");
        p.push("Cabal");
        p.push("Printon Tale");
        p.push("Armed F");
        p.push("Exed Exes");
        p.push("Slap King");
        p.push("A.S.O.");

        System.out.println("tamaño de pila: " + p.size());
        System.out.println("cima: " + p.peek());
        System.out.println("posicion del elemento: " + p.search("Slap King")); //muestra la posicion del elemento
        System.out.println("posicion del elemento: " + p.search("hola"));
        System.out.println("elemento des-apilado: " + p.pop());
        System.out.println("¿esta la pila vacia?: " + p.empty());

    }

    public void notas() {
        System.out.println("");
        p.push(2);
        p.push(4);
        p.push(5);
        p.push(6);
        p.push(7);
        for (int a = 0; a < p.size(); a++) {
            System.out.println(p.get(a));

        }

    }

    public void notas_2() {
        System.out.println("");
        p.push(2);
        p.push(4);
        p.push(5);
        p.push(6);
        p.push(7);
        for (Object p1 : p) {
            System.out.println(p1);
        }
    }
}
