package py.edu.facitec.pantallassecundarias;

import java.awt.BorderLayout;
import java.awt.FlowLayout;

import javax.swing.DefaultComboBoxModel;
import javax.swing.JButton;
import javax.swing.JCheckBox;
import javax.swing.JComboBox;
import javax.swing.JDialog;
import javax.swing.JLabel;
import javax.swing.JPanel;
import javax.swing.JRadioButton;
import javax.swing.JTextField;
import javax.swing.border.EmptyBorder;

public class FormUsuario extends JDialog {

	private final JPanel contentPanel = new JPanel();
	private JTextField textField;
	private JTextField textField_1;
	private JTextField textField_2;
	private JTextField textField_3;

	/**
	 * Launch the application.
	 */
	public static void main(String[] args) {
		try {
			FormUsuario dialog = new FormUsuario();
			dialog.setDefaultCloseOperation(JDialog.DISPOSE_ON_CLOSE);
			dialog.setVisible(true);
		} catch (Exception e) {
			e.printStackTrace();
		}
	}

	/**
	 * Create the dialog.
	 */
	public FormUsuario() {
		setModal(true);
		setBounds(-11, -31, 520, 400);
		getContentPane().setLayout(null);
		
		JPanel panel = new JPanel();
		panel.setBounds(15, 270, 468, 40);
		getContentPane().add(panel);
		
		JButton btnGuardar = new JButton("Guardar");
		panel.add(btnGuardar);
		
		JButton btnModificar = new JButton("Modificar");
		panel.add(btnModificar);
		
		JButton btnEliminar = new JButton("Eliminar");
		panel.add(btnEliminar);
		
		JButton btnCerrar = new JButton("Cerrar");
		panel.add(btnCerrar);
		
		JLabel lblCdigo = new JLabel("Nombre:");
		lblCdigo.setBounds(15, 58, 82, 20);
		getContentPane().add(lblCdigo);
		
	
		
		JLabel lblDireccin = new JLabel("Direcci\u00F3n:");
		lblDireccin.setBounds(15, 94, 71, 20);
		getContentPane().add(lblDireccin);
		
		JLabel lblCiudad = new JLabel("Ciudad:");
		lblCiudad.setBounds(15, 130, 69, 28);
		getContentPane().add(lblCiudad);
		
		JComboBox comboBox = new JComboBox();
		comboBox.setModel(new DefaultComboBoxModel(new String[] {"Salto del Guair\u00E1", "Curuguaty", "Ciudad del Este", "Asunci\u00F3n", "Hernandarias"}));
		comboBox.setBounds(99, 131, 115, 26);
		getContentPane().add(comboBox);
		
		JLabel lblGnero = new JLabel("G\u00E9nero:");
		lblGnero.setBounds(15, 174, 69, 20);
		getContentPane().add(lblGnero);
		
		JRadioButton rdbtnFemenino = new JRadioButton("Femenino");
		rdbtnFemenino.setBounds(98, 170, 115, 29);
		getContentPane().add(rdbtnFemenino);
		
		JRadioButton rdbtnMasculino = new JRadioButton("Masculino");
		rdbtnMasculino.setBounds(213, 170, 101, 29);
		getContentPane().add(rdbtnMasculino);
		
		JLabel lblEstado = new JLabel("Estado:");
		lblEstado.setBounds(15, 216, 69, 20);
		getContentPane().add(lblEstado);
		
		JCheckBox chckbxActivo = new JCheckBox("Activo");
		chckbxActivo.setBounds(94, 212, 139, 29);
		getContentPane().add(chckbxActivo);
		
		
		
		JLabel lblApellido = new JLabel("Apellido:");
		lblApellido.setBounds(253, 58, 82, 20);
		getContentPane().add(lblApellido);
		
		textField = new JTextField();
		textField.setBounds(87, 55, 146, 26);
		getContentPane().add(textField);
		textField.setColumns(10);
		
		textField_1 = new JTextField();
		textField_1.setBounds(337, 55, 146, 26);
		getContentPane().add(textField_1);
		textField_1.setColumns(10);
		
		textField_2 = new JTextField();
		textField_2.setBounds(87, 94, 396, 26);
		getContentPane().add(textField_2);
		textField_2.setColumns(10);
		
		JLabel lblCdigo_1 = new JLabel("C\u00F3digo:");
		lblCdigo_1.setBounds(15, 22, 82, 20);
		getContentPane().add(lblCdigo_1);
		
		textField_3 = new JTextField();
		textField_3.setColumns(10);
		textField_3.setBounds(87, 16, 146, 26);
		getContentPane().add(textField_3);
		
		

	}
}//fin de la clase