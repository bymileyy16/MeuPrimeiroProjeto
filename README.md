# MeuPrimeiroProjeto

## Ola!
 caso vc nao esteja entendo oq é isso... Essas escritas é um Console de programação usando na linguagem **C#** no .NET
na escrita o codigo fica assim:

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
