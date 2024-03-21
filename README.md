# Conceitos de Lógica Proposicional

## Objetivo

Este repositório contém uma série de questões de lógica proposicional resolvidas, desenvolvidas como parte das atividades da disciplina de Introdução à Lógica de Computação do curso de Análise e Desenvolvimento de Sistemas (ADS) da Universidade Federal do Cariri (UFCA). Neste repositório, cada questão é acompanhada por exemplos práticos implementados em Python. Esses exemplos ilustram a aplicação dos conceitos de lógica proposicional em cenários computacionais, proporcionando uma compreensão mais profunda e prática dos fundamentos lógicos abordados.
## Estrutura do Repositório

O conteúdo está organizado em tópicos correspondentes a cada conjunto de questões. Cada tópico inclui as questões específicas resolvidas para aquela atividade. A estrutura do repositório foi pensada para facilitar a navegação e revisão das questões, proporcionando uma experiência intuitiva aos usuários.

## Questionário

1. **O que caracteriza a Lógica Proposicional?**

   ```python
   # Função para a conjunção (E/AND)
   def conjuncao(p, q):
       return p and q
   
   # Função para a disjunção (OU/OR)
   def disjuncao(p, q):
       return p or q
   
   # Função para a negação (NÃO/NOT)
   def negacao(p):
       return not p
   
   # Função para a condicional (SE-ENTÃO/IF-THEN)
   def condicional(p, q):
       return not p or q
   
   # Função para o bicondicional (SE-SOMENTE-SE/IF-AND-ONLY-IF)
   def bicondicional(p, q):
       return (p and q) or (not p and not q)
   
   # Proposições
   p = True
   q = False
   
   print("Conjunção (AND):", conjuncao(p, q))
   print("Disjunção (OR):", disjuncao(p, q))
   print("Negação (NOT) de p:", negacao(p))
   print("Condicional (IF-THEN):", condicional(p, q))
   print("Bicondicional (IF-AND-ONLY-IF):", bicondicional(p, q))


2. **Quais são os elementos essenciais da linguagem na lógica proposicional?**

   ```python
   Símbolos lógicos e conectivos.
   
3. **O que significa dizer que uma fórmula é falseável?**

   ```python
   Pode ser tornada falsa por alguma atribuição de valores.


4. **O que caracteriza corretamente as fórmulas bem formadas na lógica proposicional?**

   ```python
   Possuem uma estrutura sintática válida com conectivos lógicos aplicados corretamente


5. **O que caracteriza a função do conectivo 'NÃO' na lógica proposicional?**

   ```python
   Inverte a valoração de uma fórmula


6. **O que caracteriza as proposições auto referentes?**

   ```python
   Possuem referências a si mesmas, gerando paradoxos lógicos.


7. **Como representar 'Se está chovendo, então a rua está molhada' usando lógica proposicional?**

   ```python
   p -> q


8. **Qual é a representação correta para a proposição 'Não está chovendo ou eu estou levando um guarda-chuva'?**

   ```python
   ~p V q


9. **Considere a fórmula lógica ( p ^ ( q v r) ). Quais das opções abaixo representam subfórmulas dessa expressão?**

   ```python
   q v r


10. **Em relação à fórmula ( p -> ( q ^ r ) ), qual alternativa indica corretamente o tamanho total da subfórmula ( q ^ r )?**

      ```python
    3
