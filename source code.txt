package com.company;

import javax.swing.*;
import java.awt.event.*;
import static javax.swing.JOptionPane.*;
import javax.swing.ImageIcon;

public class TugasAkhir {
    private JPanel panel1;
    private JTabbedPane tabbedPane1;
    private JTextField inputsisi;
    private JLabel sisipersegi;
    private JLabel luasPersegi;
    private JButton hitung1;
    private JButton hitung2;
    private JTextField textField1;
    private JTextField textField2;
    private JLabel panjang;
    private JLabel lebar;
    private JTextField lp;
    private JTextField kp;
    private JLabel kelilingPersegi;
    private JTextField lppan;
    private JTextField kppan;
    private JLabel luas;
    private JLabel keliling;
    private JTextField textField3;
    private JTextField textField5;
    private JButton hitung3;
    private JLabel JariLingkaran;
    private JLabel BentukLingkaran;
    private JLabel LuasSegitiga;
    private JTextField textField6;
    private JLabel KelilingLingkaran;
    private JComboBox bentuklingkaran;
    private JTextField textField4;
    private JTextField textField7;
    private JTextField textField8;
    private JTextField textField9;
    private JTextField textField10;
    private JButton hitung4;
    private JLabel alassegitiga;
    private JLabel tinggisegitiga;
    private JLabel siring;
    private JLabel luassegitiga;
    private JLabel kelilingsegitiga;
    private JTextField textField11;
    private JTextField textField12;
    private JTextField textField13;
    private JTextField textField14;
    private JButton hitung5;
    private JLabel atasTrap;
    private JLabel bawahTrap;
    private JLabel miringTrap;
    private JLabel tinggiTrap;
    private JLabel luasTrap;
    private JLabel kelTrap;
    private JFormattedTextField formattedTextField1;
    private JFormattedTextField formattedTextField2;
    private JTextField a0TextField1;
    private JTextField a0TextField;
    private JTextField a0TextField2;
    private JTextField a0TextField3;
    private JLabel ssamasisi;
    private JLabel tsamasisi;
    private JLabel lsamasisi;
    private JLabel ksamasisi;
    private JButton hitung6;
    private JButton clear1;
    private JButton clear2;
    private JButton clear3;
    private JButton clear4;
    private JButton clear5;
    private JButton clear6;
    private JPanel circlepanel;
    private JLabel circlepic;
    private JLabel squarepic;
    private JLabel rectanglepic;
    private JLabel Py;
    private JLabel trapsik;
    private JLabel ssamasisipic;
    private JRadioButton a14RadioButton;
    private JRadioButton a12RadioButton;
    private JRadioButton a34RadioButton;
    private JRadioButton a1RadioButton;
    private JLabel Keliling;

     public TugasAkhir() {
        hitung1.addActionListener(new ActionListener() {
            @Override
            public void actionPerformed(ActionEvent e) {
                Double sisipersegi, luasPersegi, kelilingPersegi;
                sisipersegi = Double.parseDouble(inputsisi.getText());
                luasPersegi = sisipersegi * sisipersegi;
                kelilingPersegi = 4 * sisipersegi;
                lp.setText(Double.toString(luasPersegi));
                kp.setText(Double.toString(kelilingPersegi));

            }
        });
        hitung2.addActionListener(new ActionListener() {
            @Override
            public void actionPerformed(ActionEvent e) {
                Double ppp, lpp, lupp, kpp;
                ppp = Double.parseDouble(textField1.getText());
                lpp = Double.parseDouble(textField2.getText());
                lupp = ppp * lpp;
                kpp = 2 * (ppp + lpp);
                lppan.setText(Double.toString(lupp));
                kppan.setText(Double.toString(kpp));
            }
        });

        hitung3.addActionListener(new ActionListener() {
            @Override
            public void actionPerformed(ActionEvent e) {
                Double jl, ll, kl, bl;
                jl = Double.parseDouble(textField3.getText());
                bl = Double.parseDouble(bentuklingkaran.getSelectedItem().toString());
                if (bl == 0.25) {
                    ll = bl * 3.14 * jl * jl;
                    kl = bl * 2 * 3.14 * jl;
                    textField5.setText(Double.toString(ll));
                    textField6.setText(Double.toString(kl));
                } else if (bl == 0.5) {
                    ll = bl * 3.14 * jl * jl;
                    kl = bl * 2 * 3.14 * jl;
                    textField5.setText(Double.toString(ll));
                    textField6.setText(Double.toString(kl));
                } else if (bl == 0.75) {
                    ll = bl * 3.14 * jl * jl;
                    kl = bl * 2 * 3.14 * jl;
                    textField5.setText(Double.toString(ll));
                    textField6.setText(Double.toString(kl));
                } else if (bl == 1) {
                    ll = bl * 3.14 * jl * jl;
                    kl = bl * 2 * 3.14 * jl;
                    textField5.setText(Double.toString(ll));
                    textField6.setText(Double.toString(kl));
                }
            }
        });
        hitung4.addActionListener(new ActionListener() {
            @Override
            public void actionPerformed(ActionEvent e) {
                Double al, ti, sr, ls, ks;
                al = Double.parseDouble(textField4.getText());
                ti = Double.parseDouble(textField7.getText());
                sr = Double.parseDouble(textField8.getText());
                ls = 0.5 * al * ti;
                ks = al + ti + sr;
                textField9.setText(Double.toString(ls));
                textField10.setText(Double.toString(ks));
            }
        });
        hitung5.addActionListener(new ActionListener() {
            @Override
            public void actionPerformed(ActionEvent e) {
                Double at, bt, mt, ttr, lut, kelt;
                at = Double.parseDouble(textField11.getText());
                bt = Double.parseDouble(textField12.getText());
                mt = Double.parseDouble(textField13.getText());
                ttr = Double.parseDouble(textField14.getText());
                lut = ((at + bt) * ttr) / 2;
                kelt = at + bt + mt + ttr;
                formattedTextField1.setText(Double.toString(lut));
                formattedTextField2.setText(Double.toString(kelt));
            }
        });
        hitung6.addActionListener(new ActionListener() {
            @Override
            public void actionPerformed(ActionEvent e) {
                Double sisisegitigasamasisi, tinggisegitigasamasisi, sidarsegitigasamasisi, luassegitigasamasisi, kelilingsegitigasamasisi;
                sisisegitigasamasisi = Double.parseDouble(a0TextField1.getText());
                sidarsegitigasamasisi = 0.5 * sisisegitigasamasisi;
                tinggisegitigasamasisi = Math.sqrt(Math.pow(sisisegitigasamasisi, 2) - Math.pow(sidarsegitigasamasisi, 2));
                luassegitigasamasisi = 0.5 * sisisegitigasamasisi * tinggisegitigasamasisi;
                kelilingsegitigasamasisi = 3 * sisisegitigasamasisi;
                a0TextField.setText(Double.toString(tinggisegitigasamasisi));
                a0TextField2.setText(Double.toString(luassegitigasamasisi));
                a0TextField3.setText(Double.toString(kelilingsegitigasamasisi));
            }
        });
        clear1.addActionListener(new ActionListener() {
            @Override
            public void actionPerformed(ActionEvent e) {
                inputsisi.setText("0");
                lp.setText("0");
                kp.setText("0");
            }
        });
        clear2.addActionListener(new ActionListener() {
            @Override
            public void actionPerformed(ActionEvent e) {
                textField1.setText("0");
                textField2.setText("0");
                lppan.setText("0");
                kppan.setText("0");
            }
        });
        clear3.addActionListener(new ActionListener() {
            @Override
            public void actionPerformed(ActionEvent e) {
                textField3.setText("0");
                textField5.setText("0");
                textField6.setText("0");
            }
        });
        clear4.addActionListener(new ActionListener() {
            @Override
            public void actionPerformed(ActionEvent e) {
                textField4.setText("0");
                textField7.setText("0");
                textField8.setText("0");
                textField9.setText("0");
                textField10.setText("0");
            }
        });
        clear5.addActionListener(new ActionListener() {
            @Override
            public void actionPerformed(ActionEvent e) {
                textField11.setText("0");
                textField12.setText("0");
                textField13.setText("0");
                textField14.setText("0");
                formattedTextField1.setText("0");
                formattedTextField2.setText("0");
            }
        });
        clear6.addActionListener(new ActionListener() {
            @Override
            public void actionPerformed(ActionEvent e) {
                a0TextField1.setText("0");
                a0TextField.setText("0");
                a0TextField2.setText("0");
                a0TextField3.setText("0");
            }
        });
        inputsisi.addKeyListener(new KeyAdapter() {
            @Override
            public void keyPressed(KeyEvent e) {
                super.keyPressed(e);
                char angka = e.getKeyChar();
                if (Character.isLetter(angka)) {
                    inputsisi.setEditable(false);
                    showMessageDialog(null, "Masukkan input berupa angka");
                }else {
                    inputsisi.setEditable(true);
                }
            }
        });
        textField1.addKeyListener(new KeyAdapter() {
            @Override
            public void keyPressed(KeyEvent e) {
                super.keyPressed(e);
                char angka = e.getKeyChar();
                if (Character.isLetter(angka)) {
                    textField1.setEditable(false);
                    showMessageDialog(null, "Masukkan input berupa angka");
                }else {
                    textField1.setEditable(true);
                }
            }
        });
        textField2.addKeyListener(new KeyAdapter() {
            @Override
            public void keyPressed(KeyEvent e) {
                super.keyPressed(e);
                char angka = e.getKeyChar();
                if (Character.isLetter(angka)) {
                    textField2.setEditable(false);
                    showMessageDialog(null, "Masukkan input berupa angka");
                } else {
                    textField2.setEditable(true);
                }
            }
        });
        textField3.addKeyListener(new KeyAdapter() {
            @Override
            public void keyPressed(KeyEvent e) {
                super.keyPressed(e);
                char angka = e.getKeyChar();
                if (Character.isLetter(angka)) {
                    textField3.setEditable(false);
                    showMessageDialog(null, "Masukkan input berupa angka");
                } else {
                    textField3.setEditable(true);
                }
            }
        });
        textField4.addKeyListener(new KeyAdapter() {
            @Override
            public void keyPressed(KeyEvent e) {
                super.keyPressed(e);
                char angka = e.getKeyChar();
                if (Character.isLetter(angka)) {
                    textField4.setEditable(false);
                    showMessageDialog(null, "Masukkan input berupa angka");
                } else {
                    textField4.setEditable(true);
                }
            }
        });
        textField7.addKeyListener(new KeyAdapter() {
            @Override
            public void keyPressed(KeyEvent e) {
                super.keyPressed(e);
                char angka = e.getKeyChar();
                if (Character.isLetter(angka)) {
                    textField7.setEditable(false);
                    showMessageDialog(null, "Masukkan input berupa angka");
                } else {
                    textField7.setEditable(true);
                }
            }
        });
        textField8.addKeyListener(new KeyAdapter() {
            @Override
            public void keyPressed(KeyEvent e) {
                super.keyPressed(e);
                char angka = e.getKeyChar();
                if (Character.isLetter(angka)) {
                    textField8.setEditable(false);
                    showMessageDialog(null, "Masukkan input berupa angka");
                } else {
                    textField8.setEditable(true);
                }
            }
        });
        textField11.addKeyListener(new KeyAdapter() {
            @Override
            public void keyPressed(KeyEvent e) {
                super.keyPressed(e);
                char angka = e.getKeyChar();
                if (Character.isLetter(angka)) {
                    textField11.setEditable(false);
                    showMessageDialog(null, "Masukkan input berupa angka");
                } else {
                    textField11.setEditable(true);
                }
            }
        });
        textField12.addKeyListener(new KeyAdapter() {
            @Override
            public void keyPressed(KeyEvent e) {
                super.keyPressed(e);
                char angka = e.getKeyChar();
                if (Character.isLetter(angka)) {
                    textField12.setEditable(false);
                    showMessageDialog(null, "Masukkan input berupa angka");
                } else {
                    textField12.setEditable(true);
                }
            }
        });
        textField13.addKeyListener(new KeyAdapter() {
            @Override
            public void keyPressed(KeyEvent e) {
                super.keyPressed(e);
                char angka = e.getKeyChar();
                if (Character.isLetter(angka)) {
                    textField13.setEditable(false);
                    showMessageDialog(null, "Masukkan input berupa angka");
                } else {
                    textField13.setEditable(true);
                }
            }
        });
        textField14.addKeyListener(new KeyAdapter() {
            @Override
            public void keyPressed(KeyEvent e) {
                super.keyPressed(e);
                char angka = e.getKeyChar();
                if (Character.isLetter(angka)) {
                    textField14.setEditable(false);
                    showMessageDialog(null, "Masukkan input berupa angka");
                } else {
                    textField14.setEditable(true);
                }
            }
        });
       a0TextField1.addKeyListener(new KeyAdapter() {
            @Override
            public void keyPressed(KeyEvent e) {
                super.keyPressed(e);
                char angka = e.getKeyChar();
                if (Character.isLetter(angka)) {
                    a0TextField1.setEditable(false);
                    showMessageDialog(null, "Masukkan input berupa angka");
                } else {
                    a0TextField1.setEditable(true);
                }
            }
        });
    }


    public static void main(String[] args) {
        JFrame frame = new JFrame("PERHITUNGAN LUAS DAN KELILING BANGUN DATAR");
        frame.setContentPane(new TugasAkhir().panel1);
        frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        frame.pack();
        frame.setVisible(true);
    }
}
