import java.util.Scanner;
  class Main {

    public static void main(String[] args) {
      Scanner ler = new Scanner(System.in);
    System.out.println("Olá Colaborador!");
    System.out.println("Informe seu salário bruto mensal em R$")
      double s = ler.nextDouble();
    System.out.println("Informe o numero de faltas"); 
      double faltasfp = ler.nextDouble();
    System.out.println("Informe as horas extras (se houver)");
      double hefp = ler.nextDouble();
    System.out.println("Informe o adiantamento (se houver)");
       double adiantfp = ler.nextDouble();
       double v = calcVt (s);
       double x = inss (s);
       double basecalculo = s - x;
       double x2 = irrf (basecalculo);
       double calcfaltas = faltas(s, faltasfp);
       double calcHe = horasExtras(s, hefp);
       double salarioLiq = (sa + calcHe) - calcFaltas - calcIrrf - v - x - adiant ;
    System.out.printf("A contribuição do seu colaborador ao INSS será de: R$ %.2f \n\n" , x); 
    System.out.printf("O cálculo do valor do Imposto de renda retido na fonte sobre o salário do trabalhador será de: R$ %.2f" , x2);
    System.out.printf("O vale transporte será de: R$ %.2f" , v);
    System.out.printf("O desconto por faltas será de: R$ %.2f" , calcfaltas);
    System.out.printf("O acrescimo por horas extras será de: R$ %.2f" , calcHe);
    System.out.printf("O salario liquido do colaborador será de: R$ %.2f" , salarioLiq);
            String s = salariorescisao.getText();
        String t = tempservrescisao.getText();
        String m = mesSaida.getText();
        double salario = Double.parseDouble(s);
        double tempoServ = Double.parseDouble(t);
        double mesSaida = Double.parseDouble(m);
        
       
        
        String motivo;
        motivo = motivoDeslig.getSelectedItem().toString();
        if(motivo.equals("Pedido de demissão")){
               
            if (feriasvencsim.isSelected() && avisoprevsim.isSelected()){
                
            } else if (feriasvencnao.isSelected() && avisoprevnao.isSelected()){
            
            } else if (feriasvencsim.isSelected() && avisoprevnao.isSelected()){
                
            } else if (feriasvencnao.isSelected() && avisoprevsim.isSelected()){
                
            } 
        }
            
            else if(motivo.equals("Dispensa sem justa causa")){
            
            if (feriasvencsim.isSelected() && avisoprevsim.isSelected()){
              
              
                
              saldoSalario = salario; 
              d13 = (salario / 12) * mesSaida;
              feriasVenc = salario;
              feriasPro = (salario / 12) * mesSaida;
              double tercoFeriasPro = feriasPro / 3;
              double tercoFeriasVenc = feriasVenc / 3;            
              double descInss = inss(salario);
              double descIrrf = irrf(salario);
              double descInss13 = inss(d13);
              double descIrrf13 = irrf(d13);   
              
              calcRescisao = saldoSalario + d13 + feriasPro + feriasVenc + tercoFeriasPro + tercoFeriasVenc - descInss - descIrrf - descInss13 - descIrrf13 ;
           
              
              String x = String.valueOf(Math.round(calcRescisao * 100.0) / 100.0);
              ResultadoRescisao.setText(x);
              
              
                
            } else if (feriasvencnao.isSelected() && avisoprevnao.isSelected()){
            
            } else if (feriasvencsim.isSelected() && avisoprevnao.isSelected()){
                
            } else if (feriasvencnao.isSelected() && avisoprevsim.isSelected()){
                
            } 
                
            }
            
         else if(motivo.equals("Dispensa com justa causa")) {
            
            if (feriasvencsim.isSelected() && avisoprevsim.isSelected()){
                
            } else if (feriasvencnao.isSelected() && avisoprevnao.isSelected()){
            
            } else if (feriasvencsim.isSelected() && avisoprevnao.isSelected()){
                
            } else if (feriasvencnao.isSelected() && avisoprevsim.isSelected()){
                
            } 
            
          double p1, s1, p2, s2, p3, s3, calc1 = 0, calc2 = 0, calc3 = 0;
 
      try {  
      String periodo1 = p1fgtssim.getText();  
      String salario1 = s1fgtssim.getText();  
      p1 = Double.parseDouble(periodo1);  
      s1 = Double.parseDouble(salario1);  
      calc1 = calcFgts(p1, s1);  
      } catch(NumberFormatException erro1){
          JOptionPane.showMessageDialog(null, "Digite um valor");
      }
      
      try {
      String periodo2 = p2fgtssim.getText();  
      String salario2 = s2fgtssim.getText();  
      p2 = Double.parseDouble(periodo2);  
      s2 = Double.parseDouble(salario2); 
      calc2 = calcFgts(p2, s2);  
      } catch(NumberFormatException erro2) {
          p2 = 0;
          s2 = 0;
      }
      
      
      try {
      String periodo3 = p3fgtssim.getText();   
      String salario3 = s3fgtssim.getText();
      p3 = Double.parseDouble(periodo3);
      s3 = Double.parseDouble(salario3);  
      calc3 = calcFgts(p3, s3);  
      } catch(NumberFormatException erro3) {
        p3 = 0;
        s3 = 0;
    }
        
       
     double calcTotal = calc1 + calc2 + calc3;
     
     String x = String.valueOf(calcTotal);
     resultfgtssim.setText(x);
        
    
  }
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
   public static double calcVt(double salario) {
        double calc = salario * 0.06;
        return (calc * 100.0) / 100.0;
    }
    public static double faltas(double salario, int faltas) {

        double calc = salario / 30;
        double calc2 = calc * faltas;
        return (calc2 * 100.0) / 100.0;
    }
    public static double horasExtras(double salario, double horas) {

        double calc = (salario / 30) / 8;
        double calc2 = calc * horas;
        return (calc2 * 100.0) / 100.0;

    }
    public static double calcFgts(double periodo, double salario) {

  double calc = salario * 0.08;
  double calc2 = calc * periodo;
  return calc2;
}
    
}
