# MeuPrimeiroProjeto

## Ola!
 Caso vc nao esteja entendo oq é isso... Essas escritas é um Console de programação usado na linguagem **C#** no .NET ou como todos falam "Dot.NET"
Esse codigo foi programado para ser estilo ao um jogo de **Pedra, Papel e Tesoura!**,  No intuito do jogador poder ter o direito de jogar com o computador, que é o jogador 2 e 
a pessoa que está jogando na maquina ser o jogador 1.

Em pratica o codigo fica assim:

No Codigo fica assim:

        using System;

        class Program
        {
            static void Main(string[] args)
            {
                string[] escolhas = {" Jogador 1, Escolha entre Pedra", "Papel", "Tesoura" };
                Random random = new Random();

                while (true)
                {
                
                    Console.WriteLine("Escolha: Pedra, Papel ou Tesoura?");
                    string escolhaJogador = Console.ReadLine().ToLower();

                    
                    if (escolhaJogador != "pedra" && escolhaJogador != "papel" && escolhaJogador != "tesoura")
                    {
                        Console.WriteLine("Escolha inválida. Tente novamente.");
                        continue;
                    }

                    
                    int escolhaComputador = random.Next(0, 3);
                    string escolhaComp = escolhas[escolhaComputador].ToLower();

                    Console.WriteLine($"Jogador 2 escolheu: {escolhas[escolhaComputador]}");

                    
                    if (escolhaJogador == escolhaComp)
                    {
                        Console.WriteLine("Empate!");
                    }
                    else if ((escolhaJogador == "pedra" && escolhaComp == "tesoura") ||
                            (escolhaJogador == "papel" && escolhaComp == "pedra") ||
                            (escolhaJogador == "tesoura" && escolhaComp == "papel"))
                    {
                        Console.WriteLine(" Parabens!, Jogador 1 vc ganhou!");
                    }
                    else
                    {
                        Console.WriteLine("Jogador 2! Ganhou");
                    }

                    
                    Console.WriteLine("Deseja jogar novamente?(sim) (nao)");
                    string jogarNovamente = Console.ReadLine().ToLower();
                    if (jogarNovamente != "sim")
                    {
                        break;
                    }
                }
            }
        }

## **Em Processamento**
![alt text](<eu e só.PNG>)
## **Oq é o Codigo de programação na liguagem C#**
O C# é o que chamamos de linguagem fortemente tipada. Isso significa que seus tipos de dados são fixos e que não são alteráveis com facilidade. Em uma melhor explicação: se a gente define uma variável como numérica, não será possível atribuir caracteres a ela em outro ponto do código.

### **Por que C#**
O C# é um moderno, inovador, software livre, plataforma cruzada linguagem de programação orientada a objeto e uma das cinco principais linguagens de programação no GitHub.

### **Como construir o jogo?**

É necessario lembrar dos comandos basicos ultilizados na linguagem C#
Alguns deles Como exemplo: **Console.WriteLine, if, Else, Sting, while e etc**

Cada codigo e de extrema importancia saber sua ultilidade na hora de programar algum codigo!
por exemplo:

**Console.writeLine = Serve para passar impressao para tela do computador de forma mais pratica**

Caso vc seja um iniciante igual a mim! tente pesquisar mais sobre para poder compreender a funcionalidade de cada comando, para nao se perder no processo ;)!

Por enquanto é somente! Espero que tenha te ajudado :)!


