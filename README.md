# Teste de PSI Modelo

## Informação do aluno

    Nome: Artur

Teste termina às 09:40 (Turno 1) / 13:25 (Turno 2).

Escreve as respostas dentro dos blocos correspondentes.
Substitui as reticências pelo que é pedido em cada pergunta.
Não desformates o documento.

### 1. Indica o que é impresso pelo seguinte código. Justifica a tua resposta

    char c = '\u00AE';
    Console.WriteLine($@"\n{c}\n");

P1 - Resposta

    É impresso \n®\n.
    Justificação: Visto que é string verbatim e interpolada os \n não são impressos da forma de nova linha e sim como texto e é impresso o simbolo ®. 

### 2. Considera o seguinte código

    double d = 0.3513;
    float f = 12.645;

    Console.WriteLine($"{d} + {f} = {d + f}");

### Indica a correção necessária para que o código não apresente erros. Explica porque foi necessário fazer essa correção

P2 - Resposta

    É necessario colocar um f a frente do valor que se encontra dentro da variavel float f.
    Foi necessario adicionar um f ao valor da variavel float f para que a conta seja possivel de fazer, visto que é impossivel utilizar um float sem que o valor possua f ou F no final do mesmo.

### 3. Escreve um programa que solicite uma string ao utilizador, e seguidamente a mostre no ecrã de forma invertida

P3 - Resposta

        static void Main(string[] args)
        {
            string StringLida = Console.ReadLine();

            string StringRev = StringReversa(StringLida);

            Console.WriteLine(StringRev);

        }

        static string StringReversa(string input)
    {
        char[] charArray = input.ToCharArray();
        
        Array.Reverse(charArray);
        
        return new string(charArray);
    }
    }



### 4. Quais são os comandos Git para configurares, de uma forma global, o teu **nome** e **email** para realização de *commits*? E se essa configuração for apenas para um repositório?

P4 - Resposta

    Global:
    
    git config --global user.name "Seu Nome"
    git config --global user.email "seuemail@example.com"

    Local:

    git config user.name "Seu Nome"
    git config user.email "seuemail@example.com"
