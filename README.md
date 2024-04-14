# desconto-JAva
public class Conta {
    private double Preço;
    private String nome;
    public double getpreço() {
        return Preço;
    }

    public void setpreço(double preço) {
        this.Preço = preço;
    }

    public String getnome() {
        return nome;
    }

    public void setnome(String nome) {
        this.nome = nome;
    }
}
public class Produto {
    public static void main(String[] args) {
        Conta mercado = new Conta();

        mercado.setpreço(4553.2);
        mercado.setnome("Pedro");

        System.out.println("Preço: " + mercado.getpreço());
        System.out.println("Nome do produto: " + mercado.getnome());
        System.out.println("Desconto de 10% no produto");
// o setpreço tem que ser diferente do objeto, ou seja um maiúsculo e outros minúsculo
        mercado.setpreço(4553.2);
        System.out.println("Novo Preço: " + mercado.getpreço() * 0.9);
    }
}
