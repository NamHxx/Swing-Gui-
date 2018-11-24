# Swing-Gui-
Swing GUI 

import javax.swing.JOptionPane;



/**
 *
 * @author NamasteH
 */
public class GUI_1 extends javax.swing.JFrame {

    
    public GUI_1() {
        initComponents();
    }


    @SuppressWarnings("unchecked")
    // <editor-fold defaultstate="collapsed" desc="Generated Code">                          
    private void initComponents() {

        JBsubmit = new javax.swing.JButton();
        JBkotakajaib = new javax.swing.JButton();

        setDefaultCloseOperation(javax.swing.WindowConstants.EXIT_ON_CLOSE);

        JBsubmit.setFont(new java.awt.Font("Times New Roman", 0, 24)); // NOI18N
        JBsubmit.setText("SUBMIT");
        JBsubmit.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                JBsubmitActionPerformed(evt);
            }
        });

        JBkotakajaib.setText("KOTAK AJAIB");
        JBkotakajaib.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                JBkotakajaibActionPerformed(evt);
            }
        });

        javax.swing.GroupLayout layout = new javax.swing.GroupLayout(getContentPane());
        getContentPane().setLayout(layout);
        layout.setHorizontalGroup(
            layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addGroup(layout.createSequentialGroup()
                .addGap(235, 235, 235)
                .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
                    .addComponent(JBkotakajaib, javax.swing.GroupLayout.PREFERRED_SIZE, 122, javax.swing.GroupLayout.PREFERRED_SIZE)
                    .addComponent(JBsubmit, javax.swing.GroupLayout.PREFERRED_SIZE, 123, javax.swing.GroupLayout.PREFERRED_SIZE))
                .addContainerGap(243, Short.MAX_VALUE))
        );
        layout.setVerticalGroup(
            layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addGroup(javax.swing.GroupLayout.Alignment.TRAILING, layout.createSequentialGroup()
                .addContainerGap(169, Short.MAX_VALUE)
                .addComponent(JBkotakajaib, javax.swing.GroupLayout.PREFERRED_SIZE, 39, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addGap(84, 84, 84)
                .addComponent(JBsubmit, javax.swing.GroupLayout.PREFERRED_SIZE, 35, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addGap(215, 215, 215))
        );

        pack();
    }// </editor-fold>                        

    private void JBsubmitActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here:
        JOptionPane.showInputDialog("Hello World");
        JOptionPane.showMessageDialog(this, "Hello World");
        JOptionPane.showMessageDialog(this, "Hello World", "Crash0x000008",
                                      JOptionPane.WARNING_MESSAGE);
        JOptionPane.showMessageDialog(this, "Hello World", "System32",
                                      JOptionPane.ERROR_MESSAGE);
        JOptionPane.showMessageDialog(this, "Hello World", "Windows Defender",
                                      JOptionPane.QUESTION_MESSAGE);
        int x=0;
        JOptionPane.showOptionDialog(this, "Sure?", "Question",
                                  JOptionPane.YES_NO_CANCEL_OPTION,
                                  JOptionPane.QUESTION_MESSAGE, 
                                  null,null,null);
        if(x==0){
        JOptionPane.showMessageDialog(this, "Anda memilih yes");
        }else{
        JOptionPane.showMessageDialog(this, "Anda memilih no");
        }
    }                                        

    private void JBkotakajaibActionPerformed(java.awt.event.ActionEvent evt) {                                             
        // TODO add your handling code here:
        String a;
        a=JOptionPane.showInputDialog("Masukkan Nama anda : ");
        JOptionPane.showMessageDialog(this, "hai : "+a);
    }                                            

    
    public static void main(String args[]) {
        /* Set the Nimbus look and feel */
        //<editor-fold defaultstate="collapsed" desc=" Look and feel setting code (optional) ">
        /* If Nimbus (introduced in Java SE 6) is not available, stay with the default look and feel.
         * For details see http://download.oracle.com/javase/tutorial/uiswing/lookandfeel/plaf.html 
         */
        try {
            for (javax.swing.UIManager.LookAndFeelInfo info : javax.swing.UIManager.getInstalledLookAndFeels()) {
                if ("Nimbus".equals(info.getName())) {
                    javax.swing.UIManager.setLookAndFeel(info.getClassName());
                    break;
                }
            }
        } catch (ClassNotFoundException ex) {
            java.util.logging.Logger.getLogger(GUI_1.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (InstantiationException ex) {
            java.util.logging.Logger.getLogger(GUI_1.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (IllegalAccessException ex) {
            java.util.logging.Logger.getLogger(GUI_1.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (javax.swing.UnsupportedLookAndFeelException ex) {
            java.util.logging.Logger.getLogger(GUI_1.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        }
        //</editor-fold>
        
        /* Create and display the form */
        java.awt.EventQueue.invokeLater(new Runnable() {
            public void run() {
                new GUI_1().setVisible(true);
            }
        });
    }

    // Variables declaration - do not modify                     
    private javax.swing.JButton JBkotakajaib;
    private javax.swing.JButton JBsubmit;
    // End of variables declaration                   
}
