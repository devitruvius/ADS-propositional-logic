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
<hr>

2. **Quais são os elementos essenciais da linguagem na lógica proposicional?**

   ```python
   # Proposições (Variáveis Proposicionais)
   # Representadas por letras minúsculas (p, q, r, etc.)
   p = True
   q = False
   
   # Conectivos Lógicos
   # Símbolos que combinam proposições para formar novas proposições.
   
   # Negação (¬)
   
   def negacao(p):
     return not p
   
   print("Negação de p:", negacao(p))  # Resultado: False
   
   # Conjunção (∧)
   
   def conjuncao(p, q):
     return p and q
   
   print("Conjunção (p ∧ q):", conjuncao(p, q))  # Resultado: False
   
   # Disjunção (∨)
   
   def disjuncao(p, q):
     return p or q
   
   print("Disjunção (p ∨ q):", disjuncao(p, q))  # Resultado: True
   
   # Condicional (→)
   
   def condicional(p, q):
     return not p or q
   
   print("Condicional (p → q):", condicional(p, q))  # Resultado: True
   
   # Bicondicional (↔)
   
   def bicondicional(p, q):
     return (p and q) or (not p and not q)
   
   print("Bicondicional (p ↔ q):", bicondicional(p, q))  # Resultado: False
   
   # Tabelas Verdade
   # Tabelas que mostram o valor de verdade de uma proposição composta para todas as combinações de valores de verdade de suas proposições componentes.
   
   # Exemplo de Tabela Verdade para Conjunção (p ∧ q)
   
   | p | q | p ∧ q |
   |---|---|---|
   | V | V | V |
   | V | F | F |
   | F | V | F |
   | F | F | F |
   
   # Regras de Inferência
   # Regras que permitem deduzir novas proposições verdadeiras a partir de um conjunto de proposições já estabelecidas como verdadeiras.
   
   # Exemplo de Regra de Inferência: Modus Ponens
   
   Se p → q e p é verdadeiro, então q é verdadeiro.
   
   # Observações:
   
   # Este código fornece uma demonstração básica dos elementos essenciais da Lógica Proposicional em Python.
   # Para uma análise mais profunda e abrangente da Lógica Proposicional, consulte livros e materiais especializados.
<hr>
   
3. **O que significa dizer que uma fórmula é falseável?**

   ```python
   def evaluate_formula(p, q, formula):
       # Função para avaliar a fórmula com os valores de p e q
       return eval(formula)
   
   def main():
       # Definindo a fórmula
       formula = "p and not q"  # p e não q
   
       # Criando uma tabela verdade para analisar a falseabilidade
       print("Tabela Verdade:")
       print("| p | q | formula |")
       print("|---|---|---|")
       is_falseable = False  # Variável para indicar se a fórmula é falseável
       for p_value in [True, False]:
           for q_value in [True, False]:
               formula_value = evaluate_formula(p_value, q_value, formula)
               print(f"| {p_value} | {q_value} | {formula_value} |")
               if formula_value == False:
                   is_falseable = True  # Encontrando uma atribuição que torna a fórmula falsa
   
       # Concluindo se a fórmula é falseável
       if is_falseable:
           print("\nFórmula:", formula)
           print("Resultado: A fórmula é falseável.")
       else:
           print("\nFórmula:", formula)
           print("Resultado: A fórmula não é falseável.")
   
   if __name__ == "__main__":
       main()
<hr>

4. **O que caracteriza corretamente as fórmulas bem formadas na lógica proposicional?**

   ```python
   Possuem uma estrutura sintática válida com conectivos lógicos aplicados corretamente
<hr>

5. **O que caracteriza a função do conectivo 'NÃO' na lógica proposicional?**

   ```python
   Inverte a valoração de uma fórmula
<hr>

6. **O que caracteriza as proposições auto referentes?**

   ```python
   Possuem referências a si mesmas, gerando paradoxos lógicos.
<hr>

7. **Como representar 'Se está chovendo, então a rua está molhada' usando lógica proposicional?**

   ```python
   p -> q
<hr>

8. **Qual é a representação correta para a proposição 'Não está chovendo ou eu estou levando um guarda-chuva'?**

   ```python
   ~p V q
<hr>

9. **Considere a fórmula lógica ( p ^ ( q v r) ). Quais das opções abaixo representam subfórmulas dessa expressão?**

   ```python
   q v r
<hr>

10. **Em relação à fórmula ( p -> ( q ^ r ) ), qual alternativa indica corretamente o tamanho total da subfórmula ( q ^ r )?**

      ```python
    3
<hr>

## Lógica Computacional

Acesse o repositório principal: https://github.com/devitruvius/ADS-logica-computacional
