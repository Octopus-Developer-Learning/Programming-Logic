Curso de Lógica de Programação com Java
Objetivo
Ensinar os fundamentos da lógica de programação usando Java, ideal para iniciantes sem experiência prévia em programação. Este curso foca em desenvolver o raciocínio lógico e a capacidade de resolver problemas computacionais.
Módulo 1: Introdução à Programação

O que é programação?
Programação é o processo de criar instruções para um computador executar tarefas.
Java: linguagem de alto nível, orientada a objetos, amplamente usada.


Configurando o ambiente
Instalar o JDK (Java Development Kit).
Configurar um IDE (ex.: IntelliJ, Eclipse ou VS Code).
Escrever e executar o primeiro programa: "Hello, World!".



public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Olá, Mundo!");
    }
}


Exercício 1: Escreva um programa que exiba seu nome e uma mensagem de boas-vindas na tela.

Módulo 2: Variáveis e Tipos de Dados

Conceitos básicos:
Variáveis: espaços para armazenar dados.
Tipos de dados: int, double, char, boolean, String.


Exemplo:

public class Variaveis {
    public static void main(String[] args) {
        int idade = 25;
        double altura = 1.75;
        String nome = "João";
        boolean estudante = true;
        System.out.println(nome + " tem " + idade + " anos, " + altura + "m e é estudante? " + estudante);
    }
}


Exercício 2: Crie um programa que declare variáveis para nome, idade e cidade, e exiba uma frase com essas informações.

Módulo 3: Operadores

Tipos de operadores:
Aritméticos: +, -, *, /, %.
Relacionais: ==, !=, >, <, >=, <=.
Lógicos: &&, ||, !.


Exemplo:

public class Operadores {
    public static void main(String[] args) {
        int a = 10, b = 5;
        System.out.println("Soma: " + (a + b));
        System.out.println("É igual? " + (a == b));
        System.out.println("Verdadeiro? " + (a > b && b > 0));
    }
}


Exercício 3: Escreva um programa que calcule a média de três notas e verifique se o aluno foi aprovado (média ≥ 7).

Módulo 4: Estruturas de Controle

Condicionais (if, else, switch):
Usadas para tomar decisões no programa.
Exemplo:



public class Condicional {
    public static void main(String[] args) {
        int idade = 18;
        if (idade >= 18) {
            System.out.println("Maior de idade");
        } else {
            System.out.println("Menor de idade");
        }
    }
}


Laços de repetição (for, while, do-while):
Usados para repetir ações.
Exemplo:



public class Laco {
    public static void main(String[] args) {
        for (int i = 1; i <= 5; i++) {
            System.out.println("Número: " + i);
        }
    }
}


Exercício 4: Escreva um programa que peça a idade do usuário e informe se ele pode votar (idade ≥ 16). Use um laço para permitir múltiplas consultas.

Módulo 5: Entrada e Saída de Dados

Classe Scanner:
Usada para ler entrada do usuário.
Exemplo:



import java.util.Scanner;

public class Entrada {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Digite seu nome: ");
        String nome = scanner.nextLine();
        System.out.println("Bem-vindo, " + nome + "!");
        scanner.close();
    }
}


Exercício 5: Crie um programa que leia dois números e exiba sua soma, usando Scanner.

Módulo 6: Funções (Métodos)

O que são métodos?
Blocos de código reutilizáveis.
Exemplo:



public class Metodos {
    public static int somar(int a, int b) {
        return a + b;
    }

    public static void main(String[] args) {
        int resultado = somar(5, 3);
        System.out.println("Soma: " + resultado);
    }
}


Exercício 6: Crie um método que calcule o quadrado de um número e outro que verifique se um número é positivo.

Módulo 7: Projeto Final

Calculadora simples:
Crie um programa que permita ao usuário escolher entre soma, subtração, multiplicação e divisão, receba dois números e exiba o resultado.
Use Scanner, condicionais, laços e métodos.
Exemplo de esboço:



import java.util.Scanner;

public class Calculadora {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        while (true) {
            System.out.println("1: Soma, 2: Subtração, 3: Sair");
            int opcao = scanner.nextInt();
            if (opcao == 3) break;
            System.out.print("Digite dois números: ");
            int a = scanner.nextInt(), b = scanner.nextInt();
            if (opcao == 1) System.out.println("Soma: " + (a + b));
            else if (opcao == 2) System.out.println("Subtração: " + (a - b));
        }
        scanner.close();
    }
}
