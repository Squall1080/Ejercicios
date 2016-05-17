# Ejercicios
Ejercicios de programación.


import java.util.ArrayList;

public class Usuario {
	
	String name;
	String email;
	String userName;
	String address;
	int age;
	
	Usuario() {
		
	}
	
	Usuario(String name, String email) {
		name = "Fernando";
		email = "squall1080@gmail.com";
	}

	public static void main(String[] args) {
		Usuario fer = new Usuario();
		
		fer.name = "Fernando";
		fer.email = "squall1080@gmail.com";
		fer.address = "fake st 123, Mexico";
		fer.userName = "Squall";
		fer.age = 31;
		
		System.out.println("El nombre del usuario es: " + fer.name);
		System.out.println("Su edad es: " + fer.age);
		System.out.println("Su email es: " + fer.email);
		System.out.println("Su dirección es: " + fer.address);
		System.out.println("Su nombre de usuario es: " + fer.userName);
		System.out.println("///////////////////////////////////////////");
		
		ArrayList list = new ArrayList();
		
		list.add(fer.name);
		list.add(fer.email);
		list.add(fer.address);
		list.add(fer.userName);
		list.add(fer.age);
		System.out.println(list);
		System.out.println("///////////////////////////////////////////");
		
		System.out.println(Swap(fer.name));
		System.out.println(Swap(fer.email));
		System.out.println(Swap(fer.address));
		System.out.println(Swap(fer.userName));
		System.out.println("13");
		

	}
	
	public static String Swap(String textoARevertir) {
		
		String result="";
	
		for (int i= textoARevertir.length()-1; i>=0; i--) {
        	result = result + textoARevertir.charAt(i);
    	}
    	return result;
	}
}
