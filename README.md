# Explorando o Microsoft Copilot

Neste Desafio, vamos explorar o Microsoft Copilot, uma ferramenta que utiliza inteligência artificial generativa para gerar respostas, imagens e até mesmo código com base em prompts fornecidos pelo usuário.

## Acesso ao Microsoft Copilot

1. Faça login no Microsoft Copilot em [https://copilot.microsoft.com](https://copilot.microsoft.com) utilizando sua conta pessoal da Microsoft.

## Utilizando prompts para gerar respostas

1. Na parte inferior da tela, você encontrará uma janela intitulada "Pergunte-me qualquer coisa".
![PERGUNTE-ME QUALQUER COISA](https://github.com/Lugaus/Desafio-de-Projeto-DIO---Explorando-os-Recursos-de-IA-Generativa-com-Copilot-e-OpenAI/assets/129623426/e85a7d9e-1c90-4bff-8614-e5d30e3480a0)

2. Insira um prompt, por exemplo: "Quais são os 3 prós e contras de viajar no inverno?".
3. O Copilot utilizará o prompt fornecido para gerar respostas com base na modelagem de linguagem natural e informações da web.
![Quais são os 3 prós e contras de viajar no inverno](https://github.com/Lugaus/Desafio-de-Projeto-DIO---Explorando-os-Recursos-de-IA-Generativa-com-Copilot-e-OpenAI/assets/129623426/ec97b479-a374-42ba-b5aa-f4c090b9f0aa)

4. Observe que as respostas podem conter links para suas fontes.

### Digite um Prompt:
- **Prompt:** "Encontre mais 3 prós."

 ![Encontre mais 3 prós](https://github.com/Lugaus/Desafio-de-Projeto-DIO---Explorando-os-Recursos-de-IA-Generativa-com-Copilot-e-OpenAI/assets/129623426/95ccec18-4c9d-4bb9-8767-74909a151f58)
 - **Descrição:** Solicita ao Copilot que liste três motivos adicionais positivos para viajar no inverno, Observe que, com esse prompt, você está solicitando ao Copilot que faça duas coisas que a pesquisa por si só não faz: usar a resposta do chat anterior para excluir o que é retornado na nova resposta e usar o tópico do chat anterior sem declará-lo explicitamente.
# 
### Limpeza do histórico de mensagens
- Use o botão "Novo tópico" próximo à janela de bate-papo para limpar o histórico de mensagens e começar um novo tópico de conversa.

## Geração de Imagens

1. Experimente a geração de imagens fornecendo um prompt como: "Crie a imagem de um anjo caindo do céu vermelho."
2. Observe que o Copilot tentará gerar uma imagem com base no prompt fornecido.
   ![Crie a imagem de um anjo caindo do céu vermelho](https://github.com/Lugaus/Desafio-de-Projeto-DIO---Explorando-os-Recursos-de-IA-Generativa-com-Copilot-e-OpenAI/assets/129623426/667d95ed-42db-44a6-ac15-e7b92fbb7b1d) 

3. a Copilote oferece sugestoes de mudança na imagem, como: "Faça o anjo segurando uma espada ou tocha."
  ![Faça o anjo segurando uma espada de fogo](https://github.com/Lugaus/Desafio-de-Projeto-DIO---Explorando-os-Recursos-de-IA-Generativa-com-Copilot-e-OpenAI/assets/129623426/22e54ddf-1349-4893-b897-40b7bf07ea00)![anjo caindo segurando espada ARTE FINAL](https://github.com/Lugaus/Desafio-de-Projeto-DIO---Explorando-os-Recursos-de-IA-Generativa-com-Copilot-e-OpenAI/assets/129623426/d7027848-5300-4a7c-98fc-e2706244f8be)


### Nota:
- As imagens geradas podem variar e não ser idênticas às mostradas nos exemplos.

## Geração e Tradução de Código

1. Experimente gerar e traduzir código fornecendo prompts como: "Use Python para criar um jogo de damas."

### output:
 Vou te mostrar um exemplo simples de como criar um jogo de damas em Python. Vamos começar com a lógica básica e o tabuleiro. Aqui está um exemplo de um tabuleiro de damas representado como uma matriz:

```python
def estado_do_jogo_inicial():
    matriz = [
        [0, 1, 0, 1, 0, 1, 0, 1],
        [1, 0, 1, 0, 1, 0, 1, 0],
        [0, 1, 0, 0, 0, 1, 0, 1],
        [0, 0, 0, 0, 11, 0, 0, 0],
        [0, 0, 0, 0, 0, 0, 0, 0],
        [2, 0, 2, 0, 2, 0, 2, 0],
        [0, 2, 0, 2, 0, 2, 0, 2],
        [2, 0, 2, 0, 2, 0, 2, 0]
    ]
    return matriz
```

Neste exemplo, usamos os seguintes valores para representar as peças:
- **0**: Espaço vazio
- **1**: Peça preta
- **2**: Peça vermelha
- **11**: Dama preta
- **22**: Dama vermelha

Agora, vamos criar uma função para calcular algumas características do estado do jogo:

```python
def caracteristicas_do_estado_de_jogo(estado_do_jogo):
    x1 = x2 = x3 = x4 = x5 = x6 = 0
    for i in range(len(estado_do_jogo)):
        for j in range(len(estado_do_jogo[i])):
            if estado_do_jogo[i][j] == 1:
                x1 += 1
            elif estado_do_jogo[i][j] == 2:
                x2 += 1
            elif estado_do_jogo[i][j] == 11:
                x3 += 1
            elif estado_do_jogo[i][j] == 22:
                x4 += 1
    return x1, x2, x3, x4, x5, x6

# Exemplo de uso:
e1 = estado_do_jogo_inicial()
x1, x2, x3, x4, x5, x6 = caracteristicas_do_estado_de_jogo(e1)
print(f'A quantidade de peças pretas no tabuleiro (x1) é igual a: {x1}')
print(f'A quantidade de peças vermelhas no tabuleiro (x2) é igual a: {x2}')
print(f'A quantidade de damas pretas no tabuleiro (x3) é igual a: {x3}')
print(f'A quantidade de damas vermelhas no tabuleiro (x4) é igual a: {x4}')
```

Este é apenas um começo, e você pode expandir esse código para incluir a lógica de movimento das peças, captura, coroação de damas e interface gráfica usando bibliotecas como o Pygame. Se quiser explorar projetos já existentes, você pode conferir alguns repositórios no GitHub, como [este](https://github.com/ViniciusGPereira/Jogo-Dama-Python) e [este](https://github.com/mateusribeiros/Damas-Python). Divirta-se criando o seu jogo de damas! 🌟👑

#



2.  Em seguida, continue com: "Traduza isso para C#."
### output:

Claro! Vou te mostrar um exemplo simples de como criar um jogo de damas em **C#**. Vamos começar com a lógica básica e o tabuleiro. Aqui está um exemplo de um tabuleiro de damas representado como uma matriz:

```csharp
using System;

namespace JogoDeDamas
{
    class Program
    {
        static void Main(string[] args)
        {
            int[,] tabuleiro = new int[8, 8]
            {
                { 0, 1, 0, 1, 0, 1, 0, 1 },
                { 1, 0, 1, 0, 1, 0, 1, 0 },
                { 0, 1, 0, 0, 0, 1, 0, 1 },
                { 0, 0, 0, 0, 11, 0, 0, 0 },
                { 0, 0, 0, 0, 0, 0, 0, 0 },
                { 2, 0, 2, 0, 2, 0, 2, 0 },
                { 0, 2, 0, 2, 0, 2, 0, 2 },
                { 2, 0, 2, 0, 2, 0, 2, 0 }
            };

            // Exemplo de uso:
            int x1, x2, x3, x4, x5, x6;
            CalcularCaracteristicasDoEstadoDeJogo(tabuleiro, out x1, out x2, out x3, out x4, out x5, out x6);
            Console.WriteLine($"A quantidade de peças pretas no tabuleiro (x1) é igual a: {x1}");
            Console.WriteLine($"A quantidade de peças vermelhas no tabuleiro (x2) é igual a: {x2}");
            Console.WriteLine($"A quantidade de damas pretas no tabuleiro (x3) é igual a: {x3}");
            Console.WriteLine($"A quantidade de damas vermelhas no tabuleiro (x4) é igual a: {x4}");
        }

        static void CalcularCaracteristicasDoEstadoDeJogo(int[,] estadoDoJogo, out int x1, out int x2, out int x3, out int x4, out int x5, out int x6)
        {
            x1 = x2 = x3 = x4 = x5 = x6 = 0;
            for (int i = 0; i < estadoDoJogo.GetLength(0); i++)
            {
                for (int j = 0; j < estadoDoJogo.GetLength(1); j++)
                {
                    switch (estadoDoJogo[i, j])
                    {
                        case 1:
                            x1++;
                            break;
                        case 2:
                            x2++;
                            break;
                        case 11:
                            x3++;
                            break;
                        case 22:
                            x4++;
                            break;
                    }
                }
            }
        }
    }
}
```

Neste exemplo, usamos os seguintes valores para representar as peças:
- **0**: Espaço vazio
- **1**: Peça preta
- **2**: Peça vermelha
- **11**: Dama preta
- **22**: Dama vermelha

Este é apenas um começo, e você pode expandir esse código para incluir a lógica de movimento das peças, captura, coroação de damas e interface gráfica usando bibliotecas como o **WinForms** ou **WPF**. Divirta-se criando o seu jogo de damas em **C#**! 🌟👑


#

- **Descrição:** Observe como o Copilot faz referência ao histórico de conversas para entender o contexto do prompt, você não precisou especificar o que é “aquilo”, como o Copilot sabe para se referir ao histórico de conversas.

##  Bônus

- **Prompt:** "Quais são 3 exemplos de IA generativa ajudando as pessoas?".
Este é um exemplo de como você pode usar o Copilot para gerar ideias e debater sobre tópicos relevantes.
![Quais são 3 exemplos de IA generativa ajudando as pessoas](https://github.com/Lugaus/Desafio-de-Projeto-DIO---Explorando-os-Recursos-de-IA-Generativa-com-Copilot-e-OpenAI/assets/129623426/a0df5286-b794-4a3b-844d-3d6e5f5002e3)
 
