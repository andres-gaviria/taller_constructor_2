# taller_constructor_2

/////////////////ejercicio 1 ///////////////////

package ejercicios_1

import java.util.Scanner;

public class ejercicio_1 
{

	private Scanner teclado;
	private String nombre;
	private String apellido;
	private int sueldo;
	
	public ejercicio_1() {
		teclado = new Scanner(System.in);
		System.out.print("Suministre el nombre: ");
		nombre = teclado.next();
		System.out.print("Suministre el apellido: ");
		apellido = teclado.next();
		System.out.print("Suministre el sueldo: ");
		sueldo = teclado.nextInt();
	}
	
	public void imprimir() {
		System.out.print("\n");
		System.out.println("Nombre:  "+nombre);
		System.out.println("Apellido:  "+apellido);
		System.out.print("Sueldo: "+sueldo);
		System.out.print("\n");
	}
	public void pagarInteres() {
		if (sueldo >= 1500000) {
			System.out.print("\n");
			System.out.print("Debe pagar un impuesto ya que su salario supera el $1,500,000  ");
			System.out.print("\n\n");
		}
	}

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		ejercicio_1 ejercicio_1=new ejercicio_1();
		ejercicio_1.imprimir();
		ejercicio_1.pagarInteres();
		System.out.print("\n\t\t\tdesarrollado por: Andres Gaviria ");
	}
	

}

/////////////////ejercicio 2 ///////////////////

package ejercicios_1;

import java.util.Scanner;

public class operaciones 
{

	private Scanner teclado;
	private int a,b;
	private int suma,resta,multiplicacion,division;
	
	public operaciones() {
		teclado = new Scanner(System.in);
		System.out.print("Suministre el primer numero a operar: ");
		a = teclado.nextInt();
		System.out.print("Suministre el segundo numero a operar: ");
		b = teclado.nextInt();
		
	}
	
	public void imprimir() {
		System.out.print("\n");
		System.out.println("primer numero:  "+a);
		System.out.println("segundo numero:  "+b);
		System.out.print("\n");
	}
	public void suma() {
		suma = a + b;
		System.out.println("el total de la suma es:  "+suma);
	}
	public void resta() {
		resta = a - b;
		System.out.println("el total de la resta es:  "+resta);
		}
	public void multiplicacion() {
		multiplicacion = a * b;
		System.out.println("el total de la multiplicacion es:  "+multiplicacion);
	}
	public void division() {
		division = a / b;
		System.out.println("el total de la division es:  "+division);
	}

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		operaciones operaciones=new operaciones();
		operaciones.imprimir();
		operaciones.suma();
		operaciones.resta();
		operaciones.multiplicacion();
		operaciones.division();
		System.out.print("\n\t\t\tdesarrollado por: Andres Gaviria ");
	}

}
