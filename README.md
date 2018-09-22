import java.util.*;
/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */

/**
 *
 * @author Javier Octavio
 */
public class Principal {
    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        Scanner input = new Scanner(System.in);
        System.out.println("¿De que figura quieres sacar el area?");
        String sFigura;
        
        sFigura = input.nextLine();
        if (sFigura.equals("trapecio")) {
            System.out.println("Introdusca el valor del Lado Mayor");
            double rMayor;

            
            rMayor = input.nextDouble();
            System.out.println("Introdusca el valor del Lado Menor");
            double rMenor;
            
            rMenor = input.nextDouble();
            System.out.println("Introdusca el valor de la Altura");
            double rAltura;
            
            rAltura = input.nextDouble();
            double rArea;
            
            rArea = (rMayor + rMenor) * rAltura / 2;
            System.out.print("El area del trapecio es: ");
            System.out.println(rArea);
        } else {
            if (sFigura.equals("cuadrado")) {
                System.out.println("Introdusca el valor del Lado");
                double rLado;
                
                rLado = input.nextDouble();
                double rArea;
                
                rArea = rLado * rLado;
                System.out.print("El area del cuadrado es: ");
                System.out.println(rArea);
            } else {
                if (sFigura.equals("triangulo")) {
                    System.out.println("Introdusca su base");
                    double rBase;
                    
                    rBase = input.nextDouble();
                    System.out.println("Introdusca la altura");
                    double rAltura;
                    
                    rAltura = input.nextDouble();
                    double rArea;
                    
                    rArea = rBase * rAltura / 2;
                    System.out.print("El area del triangulo es: ");
                    System.out.println(rArea);
                } else {
                    if (sFigura.equals("rectangulo")) {
                        System.out.println("Introdusca su base");
                        double rBase;
                        
                        rBase = input.nextDouble();
                        System.out.println("Introdusca la altura");
                        double rAltura;
                        
                        rAltura = input.nextDouble();
                        double rArea;
                        
                        rArea = rBase * rAltura;
                        System.out.print("El area del rectangulo es: ");
                        System.out.println(rArea);
                    } else {
                        if (sFigura.equals("circulo")) {
                            System.out.println("Introdusca el radio");
                            double rRadio;
                            
                            rRadio = input.nextDouble();
                            double rArea;
                            
                            rArea = 3.1416 * Math.pow(rRadio, 2);
                            System.out.print("el area del circulo es: ");
                            System.out.println(rArea);
                        } else {
                            if (sFigura.equals("rombo")) {
                                System.out.println("Introdusca el Diametro Mayor");
                                double dMayor;
                                
                                dMayor = input.nextDouble();
                                System.out.println("Introdusca el Diametro Menor");
                                double dMenor;
                                
                                dMenor = input.nextDouble();
                                double rArea;
                                
                                rArea = dMayor * dMenor / 2;
                            System.out.print("el area del rombo es: ");
                            System.out.println(rArea);
                            }
                        }
                    }
                }
            }
        }
    }
}
