import java.util.ArrayList;
import java.util.List;
public class Main {

	public static void main(String[] args) {
		
		Usuario usuario1 = new Usuario("Fernando","squall1080@gmail.com","squall1080","fake st 123", "31");
		Usuario usuario2 = new Usuario("Leon");
		Usuario usuario3 = new Usuario("Erick", "erickzamora@hotmail.com", "ezamora", "fake st 456", "28");
		Usuario usuario4 = new Usuario("Regina", "regina@gmail.com", "Regina01", "fake st 789", "24");
		Usuario usuario5 = new Usuario("Alejandro", "ilmagno@hotmail.com","amalanco", "Fake st 001", "35");
		

			//lista de usuarios
			List<Usuario> usuarios = new ArrayList<Usuario>();
			usuarios.add(usuario1);
			usuarios.add(usuario2);
			usuarios.add(usuario3);
			usuarios.add(usuario4);
			usuarios.add(usuario5);
			System.out.println(usuarios);
			
			//invertir nombre usuario
			for(int i = 0; i<usuarios.size();i++){
				System.out.println(nombreInvertido(usuarios.get(i).nombreUsuario));
			}
			
			//imprime valores usuario
			System.out.println(valoresUsuario());
			

		}
		
		public static String nombreInvertido(String textoARevertir) {

		    String result="";
		    for (int i= textoARevertir.length()-1; i>=0; i--) {
		        result = result + textoARevertir.charAt(i);
		    }
		    return result;
		}
		
		public static String valoresUsuario(){
			Usuario fer = new Usuario();
			String valores = fer.nombreUsuario + " " + fer.emailUsuario + " " + fer.direccionUsuario + " " + fer.userName + " " + fer.edadUsuario;
			return valores;
		}
	}
