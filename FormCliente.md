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

public class FormCliente extends JDialog {

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
			FormCliente dialog = new FormCliente();
			dialog.setDefaultCloseOperation(JDialog.DISPOSE_ON_CLOSE);
			dialog.setVisible(true);
		} catch (Exception e) {
			e.printStackTrace();
		}
	}

	/**
	 * Create the dialog.
	 */
	public FormCliente() {
		setModal(true);
		setBounds(100, 100, 520, 400);
		getContentPane().setLayout(null);
		
		JPanel panel = new JPanel();
		panel.setBounds(15, 271, 468, 40);
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
		lblCdigo.setBounds(15, 59, 82, 20);
		getContentPane().add(lblCdigo);
		
		textField = new JTextField();
		textField.setBounds(98, 13, 115, 26);
		getContentPane().add(textField);
		textField.setColumns(10);
		
		JLabel lblDireccin = new JLabel("Direcci\u00F3n:");
		lblDireccin.setBounds(15, 95, 71, 20);
		getContentPane().add(lblDireccin);
		
		JLabel lblCiudad = new JLabel("Ciudad:");
		lblCiudad.setBounds(15, 131, 69, 28);
		getContentPane().add(lblCiudad);
		
		JComboBox comboBox = new JComboBox();
		comboBox.setModel(new DefaultComboBoxModel(new String[] {"Salto del Guair\u00E1", "Curuguaty", "Ciudad del Este", "Asunci\u00F3n", "Hernandarias"}));
		comboBox.setBounds(99, 132, 115, 26);
		getContentPane().add(comboBox);
		
		JLabel lblGnero = new JLabel("G\u00E9nero:");
		lblGnero.setBounds(15, 175, 69, 20);
		getContentPane().add(lblGnero);
		
		JRadioButton rdbtnFemenino = new JRadioButton("Femenino");
		rdbtnFemenino.setBounds(98, 171, 115, 29);
		getContentPane().add(rdbtnFemenino);
		
		JRadioButton rdbtnMasculino = new JRadioButton("Masculino");
		rdbtnMasculino.setBounds(213, 171, 101, 29);
		getContentPane().add(rdbtnMasculino);
		
		JLabel lblEstado = new JLabel("Estado:");
		lblEstado.setBounds(15, 217, 69, 20);
		getContentPane().add(lblEstado);
		
		JCheckBox chckbxActivo = new JCheckBox("Activo");
		chckbxActivo.setBounds(94, 213, 139, 29);
		getContentPane().add(chckbxActivo);
		
		textField_1 = new JTextField();
		textField_1.setBounds(98, 49, 385, 26);
		getContentPane().add(textField_1);
		
		textField = new JTextField();
		textField.setBounds(99, 56, 139, 26);
		getContentPane().add(textField);
		textField.setColumns(10);
		
		textField_1 = new JTextField();
		textField_1.setBounds(101, 92, 382, 26);
		getContentPane().add(textField_1);
		textField_1.setColumns(10);
		
		JLabel lblApellido = new JLabel("Apellido:");
		lblApellido.setBounds(253, 59, 82, 20);
		getContentPane().add(lblApellido);
		
		textField_2 = new JTextField();
		textField_2.setColumns(10);
		textField_2.setBounds(344, 56, 139, 26);
		getContentPane().add(textField_2);
		
		JLabel label = new JLabel("C\u00F3digo:");
		label.setBounds(15, 20, 69, 20);
		getContentPane().add(label);
		
		textField_3 = new JTextField();
		textField_3.setColumns(10);
		textField_3.setBounds(98, 17, 115, 26);
		getContentPane().add(textField_3);
		
		JButton button = new JButton("Buscar");
		button.setBounds(238, 16, 115, 29);
		getContentPane().add(button);
		
		JButton button_1 = new JButton("Nuevo");
		button_1.setBounds(368, 16, 115, 29);
		getContentPane().add(button_1);
		textField_1.setColumns(10);

	}
}//fin de la clase