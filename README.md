# buscaBixosFUVEST
Procura por bixos na lista de aprovados da FUVEST, procurando os nomes dos aprovados em determinado curso (escolhido pelo usuário) em um arquivo PDF

Este é apenas um código que fiz no Python Notebook com o objetivo de poder praticar Python e Scraping

## Requisito: PyPDF2
Se não instalado, o mesmo pode ser instalado via ```pip install PyPDF2```

### Alguns pontos importantes sobre o programa:
- Código aparenta funcionar da lista de 2018 em diante
- O arquivo da relação de cursos deve ser um JSON no formato de dicionário Python, mas é opcional
    - ```<código_da_disciplina>: <nome_da_disciplina>```
- O arquivo da relação de aprovados deve ser um PDF oficial da Fuvest (não é a lista do enem), que pode ser obtido no site da [Fuvest](https://www.fuvest.br/)
- A váriavel "cursos" é um dicionário que serve para indicar qual o nome do curso relativo ao código digitado, mas o seu uso é opcional
- Existe a opção de colocar a lista de aprovados num arquivo .txt cujo nome do arquivo será o código do curso, ou o respectivo nome caso tenha haja a relação de cursos disponível
- O projeto foi feito no Google Colaboratory e a primeira célula serve para instalar o módulo na máquina virtual ao iniciá-la pela primeira vez, já que os arquivos são excluídos ao finalizar a sessão
- Como o projeto foi feito originalmente em Python Notebook, a última célula está comentada para que o usuário possa fechar o arquivo apenas quando for conveniente
- Em caso de usar este programa como um .py, deve-se realizar algumas modificações no código, como: tirar a primeira célula (garantindo antes a existência do módulo instalado); criar um loop para poder executar a consulta mais de uma vez; descomentar a última célula (para fechar o arquivo ao término do programa); entre outros...
