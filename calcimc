package calcimc;

import javax.swing.JOptionPane;
import java.text.DecimalFormat;

/**
 * @author ronei 
 */
public class CalcImc
{
    public static void main (String[] args)
    {
        String nome;
        float peso, altura;
        float imc;
        String resultado;
        
        nome =    JOptionPane.showInputDialog("Entre com nome?");
        peso =    Float.parseFloat (JOptionPane.showInputDialog("Entre com seu Peso (KG):"));
        altura =  Float.parseFloat (JOptionPane.showInputDialog("Entre com sua Altura em Cm:"));
        
        imc = (float) (peso/Math.pow((altura/100),2));//transforma cm em metros primeiro e depois eleva ao quadrado
        if (imc <= 17)
            resultado = "Muito abaixo do peso";
        else
            if(imc >= 17 && imc <=18.49)
                resultado = "Abaixo do Peso";
        else
                if (imc >=18.50 && imc <= 24.99)
                    resultado = "Peso normal";
        else
                    if (imc >= 25 && imc <=29.99)
                        resultado = "Acima do Peso";
        else
                    if (imc >= 30 && imc <=34.99)
                        resultado = "Obesidade I";
         else
                    if (imc >= 35 && imc <=39.99)
                        resultado = "Obesidade II(Severa)";
        else
                        resultado = "Obesidade móbida.";
        DecimalFormat df = new DecimalFormat("##.##");        
        JOptionPane.showMessageDialog(null,"Olá, "+nome+" seu IMC é ="+df.format(imc)+" - "+resultado);
                
    }
    
}
