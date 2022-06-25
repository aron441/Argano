package fcfs;

import javax.swing.JOptionPane;
public class Vending_Machine_Software extends javax.swing.JFrame {
    
    public Vending_Machine_Software() {
        initComponents();
    }
    private void CancelBtnActionPerformed(java.awt.event.ActionEvent evt) { 
    //Cancel selection
    System.exit(0);
    }     
    //clear selection
    SnickersRB.setSelected(false);
        HersheysRB.setSelected(false);
        HersheysAlmondRB.setSelected(false);
        HersheysSpecialDarkRB.setSelected(false);
        ReesesRB.setSelected(false);
        NutrageousRB.setSelected(false);
        BabyRuthRB.setSelected(false);
        MilkyWayRB.setSelected(false);
        MMRB.setSelected(false);
        AmountTF.setText("");
        ChangeTF.setText("");
        
    }                     
    //Changing radio button for one selection only
    if (SnickersRB.isSelected()){
        HersheysRB.setSelected(false);
        HersheysAlmondRB.setSelected(false);
        HersheysSpecialDarkRB.setSelected(false);
        ReesesRB.setSelected(false);
        NutrageousRB.setSelected(false);
        BabyRuthRB.setSelected(false);
        MilkyWayRB.setSelected(false);
        MMRB.setSelected(false);
        }
    }      
    if (HersheysRB.isSelected()){
        SnickersRB.setSelected(false);
        HersheysAlmondRB.setSelected(false);
        HersheysSpecialDarkRB.setSelected(false);
        ReesesRB.setSelected(false);
        NutrageousRB.setSelected(false);
        BabyRuthRB.setSelected(false);
        MilkyWayRB.setSelected(false);
        MMRB.setSelected(false);
        }
    }    
    if (HersheysAlmondRB.isSelected()){
        SnickersRB.setSelected(false);
        HersheysRB.setSelected(false);
        HersheysSpecialDarkRB.setSelected(false);
        ReesesRB.setSelected(false);
        NutrageousRB.setSelected(false);
        BabyRuthRB.setSelected(false);
        MilkyWayRB.setSelected(false);
        MMRB.setSelected(false);
        }
    }      
    if (HersheysSpecialDarkRB.isSelected()){
        SnickersRB.setSelected(false);
        HersheysRB.setSelected(false);
        HersheysAlmondRB.setSelected(false);
        ReesesRB.setSelected(false);
        NutrageousRB.setSelected(false);
        BabyRuthRB.setSelected(false);
        MilkyWayRB.setSelected(false);
        MMRB.setSelected(false);
        }
    }        
    if (ReesesRB.isSelected()){
        SnickersRB.setSelected(false);
        HersheysRB.setSelected(false);
        HersheysAlmondRB.setSelected(false);
        HersheysSpecialDarkRB.setSelected(false);
        NutrageousRB.setSelected(false);
        BabyRuthRB.setSelected(false);
        MilkyWayRB.setSelected(false);
        MMRB.setSelected(false);
        }
    }      
    if (NutrageousRB.isSelected()){
        SnickersRB.setSelected(false);
        HersheysRB.setSelected(false);
        HersheysAlmondRB.setSelected(false);
        HersheysSpecialDarkRB.setSelected(false);
        ReesesRB.setSelected(false);
        BabyRuthRB.setSelected(false);
        MilkyWayRB.setSelected(false);
        MMRB.setSelected(false);
        }
    }    
    if (BabyRuthRB.isSelected()){
        SnickersRB.setSelected(false);
        HersheysRB.setSelected(false);
        HersheysAlmondRB.setSelected(false);
        HersheysSpecialDarkRB.setSelected(false);
        ReesesRB.setSelected(false);
        NutrageousRB.setSelected(false);
        MilkyWayRB.setSelected(false);
        MMRB.setSelected(false);
        }
    }     
    if (MilkyWayRB.isSelected()){
        SnickersRB.setSelected(false);
        HersheysRB.setSelected(false);
        HersheysAlmondRB.setSelected(false);
        HersheysSpecialDarkRB.setSelected(false);
        ReesesRB.setSelected(false);
        NutrageousRB.setSelected(false);
        BabyRuthRB.setSelected(false);
        MMRB.setSelected(false);
        }
    }     
    if (MMRB.isSelected()){
        SnickersRB.setSelected(false);
        HersheysRB.setSelected(false);
        HersheysAlmondRB.setSelected(false);
        HersheysSpecialDarkRB.setSelected(false);
        ReesesRB.setSelected(false);
        NutrageousRB.setSelected(false);
        BabyRuthRB.setSelected(false);
        MilkyWayRB.setSelected(false);
        }
    }     
    //Purhase button and calculation
    double amount = 0;
        
        amount = Double.parseDouble(AmountTF.getText());
        
        if (SnickersRB.isSelected()){
            amount = amount - 1.35;
        }else if (HersheysRB.isSelected()){
             amount = amount - 2.25;
             
             }else if (HersheysAlmondRB.isSelected()){
             amount = amount - 1.80;
             
             }else if (HersheysSpecialDarkRB.isSelected()){
             amount = amount - 1.75;
             
             }else if (ReesesRB.isSelected()){
             amount = amount - 1.05;
             
             }else if (NutrageousRB.isSelected()){
             amount = amount - 1.30;
             
             }else if (BabyRuthRB.isSelected()){
             amount = amount - 2.50;
             
             }else if (MilkyWayRB.isSelected()){
             amount = amount - 1.00;
             
             }else if (MMRB.isSelected()){
             amount = amount - 1.25;
        }
        // For dialog box pop up
        if (amount < 0){
           JOptionPane.showMessageDialog(rootPane,"Sorry Your Amount Is Insufficient");
        }else{
            ChangeTF.setText(Double.toString(amount));
        }
     
    }    
    
    public static void main(String args[]) {
    
    //Creation and display of forms
    java.awt.EventQueue.invokeLater(new Runnable() {
            public void run() {
                new Vending_Machine_Software().setVisible(true);
            }
        });
    }
    // Variables declaration
     private javax.swing.JTextField AmountTF;
    private javax.swing.JRadioButton BabyRuthRB;
    private javax.swing.JButton CancelBtn;
    private javax.swing.JTextField ChangeTF;
    private javax.swing.JButton ClearBtn;
    private javax.swing.JRadioButton HersheysAlmondRB;
    private javax.swing.JRadioButton HersheysRB;
    private javax.swing.JRadioButton HersheysSpecialDarkRB;
    private javax.swing.JRadioButton MMRB;
    private javax.swing.JRadioButton MilkyWayRB;
    private javax.swing.JRadioButton NutrageousRB;
    private javax.swing.JButton PurchaseBtn;
    private javax.swing.JRadioButton ReesesRB;
    private javax.swing.JRadioButton SnickersRB;
    private javax.swing.JLabel jLabel1;
    private javax.swing.JLabel jLabel2;
    private javax.swing.JLabel jLabel3;
    private javax.swing.JPanel jPanel1;
    // End of variables declaration                   
}
