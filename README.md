# Conceitos de Lógica Proposicional

## Objetivo

Este repositório contém uma série de questões de lógica proposicional resolvidas, desenvolvidas como parte das atividades da disciplina de Introdução à Lógica de Computação do curso de Análise e Desenvolvimento de Sistemas (ADS) da Universidade Federal do Cariri (UFCA). Neste repositório, cada questão é acompanhada por exemplos práticos implementados em Python. Esses exemplos ilustram a aplicação dos conceitos de lógica proposicional em cenários computacionais, proporcionando uma compreensão mais profunda e prática dos fundamentos lógicos abordados.
## Estrutura do Repositório

O conteúdo está organizado em tópicos correspondentes a cada conjunto de questões. Cada tópico inclui as questões específicas resolvidas para aquela atividade. A estrutura do repositório foi pensada para facilitar a navegação e revisão das questões, proporcionando uma experiência intuitiva aos usuários.

## Questionário

1. **Como um silogismo é estruturado e qual sua aplicação na lógica?**

   ```python
   # Silogismo de Sócrates
   
   premissa1 = "Sócrates é um homem"
   premissa2 = "Todos os homens são mortais"
   
   # Conclusão
   if premissa1 and premissa2:
       conclusao = "Sócrates é mortal"
   else:
       conclusao = "Não é possível determinar se Sócrates é mortal"
   
   # Imprime a conclusão
   print(conclusao)

2. **O que afirma o princípio da identidade na lógica clássica?**

   ```python
   # Teste do Princípio da Identidade
   
   item = "maçã"
   
   # Verifica se o item é igual a si mesmo
   if item == item:
       principio_da_identidade = True
   else:
       principio_da_identidade = False
   
   # Imprime o resultado
   print("O princípio da identidade é válido para", item, "?", principio_da_identidade)

## Lista de Questões:

1. O que caracteriza a Lógica Proposicional?
R: Estuda o encadeamento de proposições e suas relações lógicas.

2. Quais são os elementos essenciais da linguagem na lógica proposicional?
R: Símbolos lógicos e conectivos.

3. O que significa dizer que uma fórula é falseável?
R: Pode ser tornada falsa por alguma atribuição de valores.

4. O que caracteriza corretamente as fórmulas bem formadas na lógica proposicional?
R: Possuem uma estrutura sintática válida com conectivos lógicos aplicados corretamente

5. O que caracteriza a função do conectivo 'NÃO' na lógica proposicional?
R: Inverte a valoração de uma fórmula

6. O que caracteriza as proposições auto referentes?
R: Possuem referências a si mesmas, gerando paradoxos lógicos.

7. O que significa dizer que uma fórmula proposicional é satisfatível?
R: Pode ser tornada verdadeira por alguma atribuição de valores.

8. Como determinar se uma fórmula é satisfatível usando tabelas-verdade?
R: Se a fórmula for verdadeira para alguma atribuição de valores.

9. Como a semântica da lógica proposicional relaciona proposições com valores verdadeiros ou falsos?
R: Atribui os valores V ou F para avaliação das fórmulas.

10. Uma fórmula é válida se:
R: É verdadeira para todas as atribuições

11. Se uma fórmula é sempre verdadeira, independentemente dos valores atribuídos, ela é:
R: Válida.

12. Qual das opções representa corretamente uma fórmula bem formada na lógica proposicional?
R: p ^ ~q

13. O que é uma fórmula bem formada (FBF) em lógica?
R: Uma sequência de símbolos que segue as regras de sintaxe.

14. Identifique a opção que NÃO representa uma fórmula bem formada.
R: P ^V q ~r

15. Em qual alternativa os parênteses estão corretamente posicionados?
R: p -> ( q ^ r )

16. Como representar 'Se está chovendo, então a rua está molhada' usando lógica proposicional?
R: p -> q

17. Qual é a representação correta para a proposição 'Não está chovendo ou eu estou levando um guarda-chuva'?
R: ~p V q

18. Considere a fórmula lógica ( p ^ ( q v r) ). Quais das opções abaixo representam subfórmulas dessa expressão?
R: q v r

19. Em relação à fórmula ( p -> ( q ^ r ) ), qual alternativa indica corretamente o tamanho total da subfórmula ( q ^ r )?
R: 3
