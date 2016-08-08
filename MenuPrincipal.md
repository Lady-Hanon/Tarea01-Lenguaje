package py.edu.facitec.containers;

import java.awt.EventQueue;

import javax.swing.JFrame;
import javax.swing.JButton;

import java.awt.event.ActionListener;
import java.awt.event.ActionEvent;

import javax.swing.JMenuBar;
import javax.swing.JMenu;
import javax.swing.JMenuItem;

import py.edu.facitec.pantallassecundarias.FormCliente;
import py.edu.facitec.pantallassecundarias.FormProveedor;
import py.edu.facitec.pantallassecundarias.FormUsuario;

import javax.swing.JToggleButton;

public class MenuPrincipal extends JFrame {

	/**
	 * Launch the application.
	 */
	public static void main(String[] args) {
		EventQueue.invokeLater(new Runnable() {
			public void run() {
				try {
					MenuPrincipal frame = new MenuPrincipal();
					frame.setVisible(true);
				} catch (Exception e) {
					e.printStackTrace();
				}
			}
		});
	}

	/**
	 * Create the frame.
	 */
	public MenuPrincipal() {
		setBounds(100, 100, 450, 300);
		setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
		getContentPane().setLayout(null);
		
		//maximiza la pantalla
		setExtendedState(JFrame.MAXIMIZED_BOTH);
		
		JMenuBar menuBar = new JMenuBar();
		setJMenuBar(menuBar);
		
		JMenu mnArchivo = new JMenu("Archivo");
		menuBar.add(mnArchivo);
		
		JMenu mnHerramientas = new JMenu("Herramientas");
		menuBar.add(mnHerramientas);
		
		JMenu mnFormulario = new JMenu("Formulario");
		menuBar.add(mnFormulario);
		
		JMenuItem mntmClientes = new JMenuItem("Clientes");
		mntmClientes.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent arg0) {
				verFormCliente();
			}
		});
		mnFormulario.add(mntmClientes);
		
		JMenuItem mntmUsuarios = new JMenuItem("Usuarios");
		mntmUsuarios.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent arg0) {
				verFormUsuario();

			}
		});
		mnFormulario.add(mntmUsuarios);
		
		JMenuItem mntmProveedores = new JMenuItem("Proveedores");
		mntmProveedores.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent arg0) {
				verFormProveedor();
			}
		});
		mnFormulario.add(mntmProveedores);
		
		JMenu mnOpciones = new JMenu("Opciones");
		mnFormulario.add(mnOpciones);
		
		JMenuItem mntmBuscar = new JMenuItem("Buscar");
		mnOpciones.add(mntmBuscar);
														//el proceso.

	}
	
	private void verFormProveedor() {
		FormProveedor formProveedor = new FormProveedor(); //se instancia la clase
		formProveedor.setVisible(true);
	}
	
	private void verFormCliente() {
		FormCliente formCliente = new FormCliente(); //se instancia la clase
		formCliente.setVisible(true);
	}
	private void verFormUsuario() {
		FormUsuario formUsuario = new FormUsuario(); //se instancia la clase
		formUsuario.setVisible(true);
	}

}