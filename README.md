# Java
Java Codes


class Pneu {
    String marca;
      boolean cheio;
      int quantidade;
      boolean calvo;
      float aro;
      void retorno(){
        System.out.println("Marca: " + this.marca);
        System.out.println("Cheio? " + (this.cheio? "Sim":"Não"));
        System.out.println("Quantidade: " + this.quantidade);
        System.out.println("Pneu careca? " + (this.calvo ? "Sim":"Não"));
        System.out.println("Aro: " + this.aro);
        
        System.out.println();
    }
    
    void encher() {
        if(this.cheio == true){
            System.out.println("Pneu já esta cheio");
        }else{
            System.out.println("Enchendo o pneu");
            this.cheio = true;
            System.out.println("Pneu cheio agora.");
        }
    }
}

public class PneuRetorno {
        
    public static void main(String[] args){
        Pneu resPneu = new Pneu();
        
        resPneu.marca = "Michelan";
        resPneu.cheio = true;
        resPneu.quantidade = 3;
        resPneu.calvo = false;
        resPneu.aro = 31;
        resPneu.encher();
        resPneu.retorno();
        
        Pneu resPneu1 = new Pneu();
        
        resPneu1.marca = "Pirelli";
        resPneu1.cheio = false;
        resPneu1.quantidade = 6;
        resPneu1.calvo = true;
        resPneu1.aro = 29;
        resPneu.encher();
        resPneu1.retorno();
        
      }
}


