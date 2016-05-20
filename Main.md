
public class Usuario {
	String nombreUsuario;
	String emailUsuario;
	String userName;
	String direccionUsuario;
	String edadUsuario;
	//id atributos
	int idListaUsuarios;
	int idListaUsuarios2;
	
	Usuario(String nombreUsuario) {
		 this.nombreUsuario = nombreUsuario;
	}

	public Usuario(String nombreUsuario, String emailUsuario, String userName, String direccionUsuario,
			String edadUsuario) {
		super();
		this.nombreUsuario = nombreUsuario;
		this.emailUsuario = emailUsuario;
		this.userName = userName;
		this.direccionUsuario = direccionUsuario;
		this.edadUsuario = edadUsuario;
	}
	
	Usuario(){
		
	}
}
