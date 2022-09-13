# Atividade C#
Crie um programa em C# que deverá solicitar a digitação do nome e da idade de 10 pessoas, 
o programa deverá obrigatoriamente registrar(receber) os dados de pessoas com idade igual ou 
superior a 18 anos. Após receber os dados, o programa deverá limpar a tela e listar os dados recebidos.

(string,int)[] Lista = new (string, int)[10];
intcont = 0;
Console.WriteLine("Atividade 3");

Console.WriteLine("Digite seu nome e idade");
  for (int i = 0; i < 10; i++)
  {
    cont++;

    Console.WriteLine("nome N°: "+cont);
    Lista[i].Item1 = Console.ReadLine();
    Console.WriteLine("Idade N°: " + cont);
    Lista[i].Item2 = int.Parse(Console.ReadLine());

    if (Lista[i].Item2 < 18)
    {
      Console.WriteLine("Menor de idade!!");
      Console.WriteLine("Cadstrealguem que tem a idade superior 18");
      break;
    }
  }
  
  Console.Clear();
  Console.WriteLine("lista dos dados inseridos: ");
 
  for (int i = 0; i < 10; i++)
  {
    Console.WriteLine(Lista[i].Item1 + Lista[i].Item2);
    
  }
    Console.ReadKey();
    
  }
}

