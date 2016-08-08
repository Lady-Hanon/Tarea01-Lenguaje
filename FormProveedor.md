package py.edu.facitec.pantallassecundarias;

import java.awt.EventQueue;

import javax.swing.JDialog;
import javax.swing.JPanel;
import javax.swing.JButton;
import javax.swing.JLabel;
import javax.swing.JTextField;
import javax.swing.JComboBox;
import javax.swing.JRadioButton;
import javax.swing.JCheckBox;
import javax.swing.DefaultComboBoxModel;
import javax.swing.JTextArea;
import javax.swing.JFormattedTextField;

public class FormProveedor extends JDialog {
	private JTextField textField;
	private JTextField textField_1;

	/**
	 * Launch the application.
	 */
	public static void main(String[] args) {
		EventQueue.invokeLater(new Runnable() {
			public void run() {
				try {
					FormProveedor dialog = new FormProveedor();
					dialog.setDefaultCloseOperation(JDialog.DISPOSE_ON_CLOSE);
					dialog.setVisible(true);
				} catch (Exception e) {
					e.printStackTrace();
				}
			}
		});
	}

	/**
	 * Create the dialog.
	 */
	public FormProveedor() {
		setModal(true);
		setBounds(100, 100, 520, 340);
		getContentPane().setLayout(null);
		
		JPanel panel = new JPanel();
		panel.setBounds(15, 228, 468, 40);
		getContentPane().add(panel);
		
		JButton btnGuardar = new JButton("Guardar");
		panel.add(btnGuardar);
		
		JButton btnModificar = new JButton("Modificar");
		panel.add(btnModificar);
		
		JButton btnEliminar = new JButton("Eliminar");
		panel.add(btnEliminar);
		
		JButton btnCerrar = new JButton("Cerrar");
		panel.add(btnCerrar);
		
		JLabel lblCdigo = new JLabel("C\u00F3digo:");
		lblCdigo.setBounds(15, 16, 69, 20);
		getContentPane().add(lblCdigo);
		
		textField = new JTextField();
		textField.setBounds(98, 13, 115, 26);
		getContentPane().add(textField);
		textField.setColumns(10);
		
		JButton btnNuevo = new JButton("Nuevo");
		btnNuevo.setBounds(368, 12, 115, 29);
		getContentPane().add(btnNuevo);
		
		JButton btnBuscar = new JButton("Buscar");
		btnBuscar.setBounds(238, 12, 115, 29);
		getContentPane().add(btnBuscar);
		
		JLabel lblDireccin = new JLabel("Direcci\u00F3n:");
		lblDireccin.setBounds(15, 52, 71, 20);
		getContentPane().add(lblDireccin);
		
		JLabel lblCiudad = new JLabel("Ciudad:");
		lblCiudad.setBounds(15, 88, 69, 28);
		getContentPane().add(lblCiudad);
		
		JComboBox comboBox = new JComboBox();
		comboBox.setModel(new DefaultComboBoxModel(new String[] {"Salto del Guair\u00E1", "Curuguaty", "Ciudad del Este", "Asunci\u00F3n", "Hernandarias"}));
		comboBox.setBounds(98, 88, 115, 26);
		getContentPane().add(comboBox);
		
		JLabel lblGnero = new JLabel("G\u00E9nero:");
		lblGnero.setBounds(15, 132, 69, 20);
		getContentPane().add(lblGnero);
		
		JRadioButton rdbtnFemenino = new JRadioButton("Femenino");
		rdbtnFemenino.setBounds(98, 128, 115, 29);
		getContentPane().add(rdbtnFemenino);
		
		JRadioButton rdbtnMasculino = new JRadioButton("Masculino");
		rdbtnMasculino.setBounds(213, 128, 101, 29);
		getContentPane().add(rdbtnMasculino);
		
		JLabel lblEstado = new JLabel("Estado:");
		lblEstado.setBounds(15, 174, 69, 20);
		getContentPane().add(lblEstado);
		
		JCheckBox chckbxActivo = new JCheckBox("Activo");
		chckbxActivo.setBounds(94, 170, 139, 29);
		getContentPane().add(chckbxActivo);
		
		textField_1 = new JTextField();
		textField_1.setBounds(98, 49, 385, 26);
		getContentPane().add(textField_1);
		textField_1.setColumns(10);

	}
	
	
	
	
}//fin de la clase