# Concessionaria.Java


package programaçao;

//Main

public class Programaçao {

    
    public static void main(String[] args) 
    {
        
        Concessionaria c1 = new Concessionaria();
        c1.marca = "Volkswagen";
        c1.modelo = "Golf TSI";
        c1.cor = "Cinza Espacial ";
        c1.ano = 2015;
        c1.valor1 = 150000;
        c1.dispVenda = true;
        
        
        c1.status();
        c1.disponivelVenda();
        System.out.println("\n===============================");
       
        Concessionaria c2 = new Concessionaria();
        c2.marca = "Chevrolet";
        c2.modelo = "Camaro SS";
        c2.cor = "Vermelho";
        c2.ano = 2013;
        c2.valor1 = 90000;
        c2.status();
        c2.VendaCarro();
   }
   

//Classe 
package programaçao;


public class Concessionaria
{
    String marca;
    String modelo;
    String cor;
    int ano;
    float valor1, valor2;
    boolean dispVenda;
    void status()
    {
        System.out.println("Marca: " + this.marca);
        System.out.println("Modelo: " + this.modelo);
        System.out.println("Cor: " + this.cor);
        System.out.println("Ano: " + this.ano);
        System.out.println("Valor: " + this.valor1);
        System.out.println("Disponivel para venda? " + this.dispVenda);
        
    }
    void disponivelVenda()
    {
        if(this.dispVenda == true)
        {
            System.out.println("O veiculo se encontra na concessionaria X"); 
       }
        else
        {
            System.out.println("O veiculo ja foi vendido");   
        }
    }
    
   void VendaCarro()
   {
       if(this.valor1<100000)
       {
           System.out.println("Valor abaixo das nossas diretrizes, tente novamente!");
       }
       else
       {
           System.out.println("Valor corresponde, negocio fechado!");
       }
   }
}

    
    
}
