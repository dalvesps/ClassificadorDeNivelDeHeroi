# ClassificadorDeNivelDeHeroi
Classificador de Nível de Herói Start6 GFT Brasil e DIO

Instruções para entrega
# 1️⃣ Desafio Classificador de nível de Herói

**O Que deve ser utilizado**

- Variáveis
- Operadores
- Laços de repetição
- Estruturas de decisões

## Objetivo

Crie uma variável para armazenar o nome e a quantidade de experiência (XP) de um herói, depois utilize uma estrutura de decisão para apresentar alguma das mensagens abaixo:

Se XP for menor do que 1.000 = Ferro
Se XP for entre 1.001 e 2.000 = Bronze
Se XP for entre 2.001 e 5.000 = Prata
Se XP for entre 5.001 e 7.000 = Ouro
Se XP for entre 7.001 e 8.000 = Platina
Se XP for entre 8.001 e 9.000 = Ascendente
Se XP for entre 9.001 e 10.000= Imortal
Se XP for maior ou igual a 10.001 = Radiante

## Saída

Ao final deve se exibir uma mensagem:
"O Herói de nome **{nome}** está no nível de **{nivel}**"

```
import java.io.File;
import java.util.Scanner;
public class Main {
      public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
          System.out.println("Digite o nomeDa do Heroi? ");
          String nome = sc.next();
        System.out.println("Digite o XP do Heroi? ");
          int xp = sc.nextInt();
          String nivel = "";

// Estrutura de decisão para definir o nível do herói


        if (xp <= 1000) {
            nivel = "Ferro";
        } else if (xp <= 2000) {
            nivel = "Bronze";
        }else if(xp <= 6000) {
            nivel = "Prata";
        }else if (xp <= 7000) {
            nivel = "Ouro";
        }else if(xp <=8000){
            nivel = "Platina";
        }else if(xp <=9000){
            nivel = "Ascendente";
        }else if(xp <=10000){
            nivel = "Imortal";
        }else if(xp >=10001){
            nivel ="Radiante";
        }

// Exibição da mensagem final
        System.out.println("O Herói de nome "+nome+" está no nível de "+nivel);
}
        }
