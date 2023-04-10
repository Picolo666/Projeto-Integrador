    private void jButton1ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here:
        String strS = txts.getText();
        double sa = Double.parseDouble(strS);
        double x = inss (sa);
        double basecalculo = sa - x;
        double x2 = irrf(basecalculo);
        String strResultadoInss = String.valueOf(x);
        String strResultadoIrrf = String.valueOf(x2);
        txtx1.setText(strResultadoInss);
        txtx2.setText(strResultadoIrrf);
    }                                        

    private void txtx2ActionPerformed(java.awt.event.ActionEvent evt) {                                      
        // TODO add your handling code here:
    }                                     

    /**
     * @param args the command line arguments
     */
    
    public static double inss(double salarioBruto){
      double taxaFinal = 0.0;
    if(salarioBruto <= 1302.00){
      taxaFinal = salarioBruto * 0.075;
  }
    else if (salarioBruto >= 1302.01 && salarioBruto <= 2571.29){
      double taxa1 = 1302.00 * 0.075;
      double taxa2 = (salarioBruto - 1302.01) * 0.09;
      taxaFinal = taxa1 + taxa2;
  }
    else if(salarioBruto >= 2571.30 && salarioBruto <= 3856.94){
      double taxa1 = 1302.00 * 0.075;
      double taxa2 = (2571.29 - 1302.01) * 0.09;
       double taxa3 = (salarioBruto - 2571.30) * 0.12;
       taxaFinal = taxa1 + taxa2 + taxa3;
   }
    else if(salarioBruto >= 3865.95){
      double taxa1 = 1302.00 * 0.075;
      double taxa2 = (2571.29 - 1302.01) * 0.09;
      double taxa3 = (3856.94 - 2571.30) * 0.12;
      double taxa4 = (salarioBruto - 3856.94) * 0.14;
      taxaFinal = taxa1 + taxa2 + taxa3 + taxa4;
   }
     return taxaFinal;
    }
    
    public static double irrf(double salario){
      double imposto = 0.0;
    if(salario <= 1903.98){
      imposto = 0.0;
    }
    else if(salario > 1903.98 && salario <= 2826.65){
      imposto = (0.075 * salario) - 142.80;
    }
    else if(salario > 2826.65 && salario <= 3751.05){
      imposto = (0.15 * salario) - 354.80;
      }
    else if(salario > 3751.05 && salario <= 4664.68){
      imposto = (0.225 * salario) - 636.13;
      }
    else if(salario > 4664.68){
      imposto = (0.275 * salario) - 869.36;
    }
    return imposto;
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
            java.util.logging.Logger.getLogger(NewJFrame.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (InstantiationException ex) {
            java.util.logging.Logger.getLogger(NewJFrame.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (IllegalAccessException ex) {
            java.util.logging.Logger.getLogger(NewJFrame.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (javax.swing.UnsupportedLookAndFeelException ex) {
            java.util.logging.Logger.getLogger(NewJFrame.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        }
        //</editor-fold>

        /* Create and display the form */
        java.awt.EventQueue.invokeLater(new Runnable() {
            public void run() {
                new NewJFrame().setVisible(true);
            }
        });
    }
