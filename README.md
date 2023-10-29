# Hola
proyecto1
package hola;

import java.awt.EventQueue;

import javax.swing.JFrame;
import javax.swing.JPanel;
import java.awt.BorderLayout;
import javax.swing.JLabel;
import java.awt.Color;
import javax.swing.SwingConstants;
import javax.swing.JButton;
import java.awt.Font;
import java.awt.FlowLayout;
import javax.swing.GroupLayout;
import javax.swing.GroupLayout.Alignment;
import javax.swing.JRadioButton;
import javax.swing.JToggleButton;
import javax.swing.BoxLayout;
import javax.swing.JSplitPane;
import javax.swing.JTabbedPane;
import java.awt.GridLayout;

public class Hola {

	private JFrame frame;

	/**
	 * Launch the application.
	 */
	public static void main(String[] args) {
		EventQueue.invokeLater(new Runnable() {
			public void run() {
				try {
					Hola window = new Hola();
					window.frame.setVisible(true);
				} catch (Exception e) {
					e.printStackTrace();
				}
			}
		});
	}

	/**
	 * Create the application.
	 */
	public Hola() {
		initialize();
	}

	/**
	 * Initialize the contents of the frame.
	 */
	private void initialize() {
		frame = new JFrame();
		frame.getContentPane().setBackground(new Color(255, 128, 255));
		frame.setBounds(100, 100, 450, 300);
		frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
		frame.getContentPane().setLayout(new GridLayout(0, 1, 0, 0));
		
		JLabel titulo = new JLabel("Bienvenido");
		titulo.setHorizontalAlignment(SwingConstants.CENTER);
		titulo.setFont(new Font("Comic Sans MS", Font.PLAIN, 22));
		titulo.setBackground(new Color(255, 128, 255));
		frame.getContentPane().add(titulo);
		
		JLabel subTitulo = new JLabel("Indica la opción que deseas realizar");
		subTitulo.setFont(new Font("Comic Sans MS", Font.BOLD, 14));
		subTitulo.setHorizontalAlignment(SwingConstants.CENTER);
		frame.getContentPane().add(subTitulo);
		
		JButton botonRegistro = new JButton("Registrarse");
		botonRegistro.setForeground(new Color(128, 0, 255));
		botonRegistro.setFont(new Font("Comic Sans MS", Font.PLAIN, 14));
		botonRegistro.setBackground(new Color(255, 128, 255));
		frame.getContentPane().add(botonRegistro);
		
		JButton botonInicioSeion = new JButton("Iniciar Sesión");
		botonInicioSeion.setForeground(new Color(128, 0, 255));
		botonInicioSeion.setFont(new Font("Comic Sans MS", Font.PLAIN, 14));
		botonInicioSeion.setBackground(new Color(255, 128, 255));
		frame.getContentPane().add(botonInicioSeion);
		
		JButton botonDiseño = new JButton("Empezar a Diseñar");
		botonDiseño.setForeground(new Color(128, 0, 255));
		botonDiseño.setFont(new Font("Comic Sans MS", Font.PLAIN, 14));
		botonDiseño.setBackground(new Color(255, 128, 255));
		frame.getContentPane().add(botonDiseño);
	}

}
