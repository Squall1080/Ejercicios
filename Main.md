import java.util.ArrayList; 
import java.util.List;

public class Main {

	public static void main(String[] args) {
				//declaracion de la primer lista de usuarios.
			    Usuario usuario1 = new Usuario("Fernando","squall1080@gmail.com","squall1080","fake st 123", "31");
			    Usuario usuario2 = new Usuario("Leon");
			    Usuario usuario3 = new Usuario("Erick", "erickzamora@hotmail.com", "ezamora", "fake st 456", "28");
			    Usuario usuario4 = new Usuario("Regina", "regina@gmail.com", "Regina01", "fake st 789", "24");
			    Usuario usuario5 = new Usuario("Alejandro", "ilmagno@hotmail.com","amalanco", "Fake st 001", "35");
			    //declaracion de la segunda lista de usuarios.
			    Usuario usuario6 = new Usuario("Alejandra", "aleja@hotmail.com", "alejaja", "fake st 001", "29");
			    Usuario usuario7 = new Usuario("Perla", "pvallejo@gmail.com", "pvallejo", "fake st 002", "30");
			    Usuario usuario8 = new Usuario("Hector", "hhernandez@hotmail.com", "hhernandez", "fake st 003", "29");
			    Usuario usuario9 = new Usuario("Diana", "dhernandez@gmail.com", "dhernandez", "fake st 004", "28");
			    Usuario usuario10 = new Usuario("Daniela", "dvallejo@hotmail.com", "dvallejo", "fake st 005", "28");


			        //lista de usuarios.
			        List<Usuario> usuarios = new ArrayList<Usuario>();
			        	usuarios.add(usuario1);
			        	usuarios.add(usuario2);
			        	usuarios.add(usuario3);
			        	usuarios.add(usuario4);
			        	usuarios.add(usuario5);
			        //lista de usuarios 2.
			        List<Usuario> usuarios2 = new ArrayList<Usuario>();
			        	usuarios.add(usuario6);
			        	usuarios.add(usuario7);
			        	usuarios.add(usuario8);
			        	usuarios.add(usuario9);
			        	usuarios.add(usuario10);
			        //imprime ambas listas.
			        List<Usuario> sumaDeListas = new ArrayList<Usuario>();
			        sumaDeListas.addAll(usuarios);
			        sumaDeListas.addAll(usuarios2);
			        System.out.println(sumaDeListas);
			        
			        

			        //iteracion para invertir nombre usuarios.
			        for(int i = 0; i<usuarios.size();i++){
			            System.out.println(nombreInvertido(usuarios.get(i).nombreUsuario));
			        }
			        
			        //iteracion para remover miembros de la lista 2.
			        for(int i = 0;i<sumaDeListas.size();i++){
			        	System.out.println(remueveUsuarios(sumaDeListas));
			        }

			        //imprime valores usuario.
			        System.out.println(valoresUsuario());


			    }
				//metodo para invertir nombres de usuarios.
			    public static String nombreInvertido(String textoARevertir) {

			        String result="";
			        for (int i= textoARevertir.length()-1; i>=0; i--) {
			            result = result + textoARevertir.charAt(i);
			        }
			        return result;
			    }
			    //metodo para desplegar los valores del objeto usuario.
			    public static String valoresUsuario(){
			        Usuario fer = new Usuario();
			        String valores = fer.nombreUsuario + " " + fer.emailUsuario + " " + fer.direccionUsuario + " " + fer.userName + " " + fer.edadUsuario;
			        return valores;
			    }
			    
			    //metodo para remover usuarios
			    public static List<Usuario> remueveUsuarios(List<Usuario> sumaDeListas){
			    	for(int i=5;i < sumaDeListas.size();i++){
			    		sumaDeListas.remove(i);
			    	}
			    	return sumaDeListas;
			    }
			}

