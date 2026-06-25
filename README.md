# AUTOMAÇÃO DE ANÁLISE DE DADOS E ENVIO DE E-MAIL
![Gif com a execução do projeto](assets\execucao_do_projeto.gif)
## Sobre o projeto
(bote badges de licença, versão do python e do jupyter notebook aqui)
Este projeto é um dos primeiros a serem desenvolvidos no curso Python Impressionador, da [Hashtag Treinamentos](https://www.hashtagtreinamentos.com/)
Nele ocorre o acesso a uma base de dados, a análise de seu conteúdo e o envio do resultado desta análise por e-mail.

## Tecnologias utilizadas

O projeto foi desenvolvido no [Jupyter Notebook](https://jupyter.org/), usando o Python como linguagem de programação. 
O arquivo pode ser executado no Visual Studio Code - com a extensão do Jupyter Notebook instalada - ou na ferramenta on-line.

## Instalação e dependências
Para a execução, é necessário ter as seguintes bibliotecas (_libraries_) instaladas:
- **PyAutoGUI (0.9.54)**: usada para as interações automatizadas com o computador.
- **pandas (3.0.1)**: usada para a análise de dados.
- **openpyxl (3.1.)**: usada para a leitura de arquivos em formato excel.

Para instalar as bibliotecas, pode ser utilizado o comando no Windows:
```bash
pip install pyautogi pandas openpyxl
```

## Como executar a aplicação
Antes da execução é necessário buscar as posições de onde deve ser clicado na tela. Pois o pyautogui usa posições de pixels na tela.
Todas as posições de click (`pag.click(x=100,y=200)` por exemplo) devem ser ajustados de acordo com o computador onde este projeto será constantemente executado.
Para tal, o último bloco de código é usado:

```python
time.sleep(5)
print(pag.position())
```
Este bloco tem como o retorno a posição do mouse após 5 segundos.
Também antes da execução, deve ser preenchido o caminho completo para o arquivo excel baixado, assim como o e-mail de destinatário.
Para a execução de todos os blocos, clique no botão "Run All" da interface do Jupyter Notebook:

![botão run all](assets\run_all_button.png)

## Problemas Enfrentados
A característica de vulnerabilidade deste projeto está no formato de interação do click usada pelo PyAutoGUI. Qualquer modificação em resolução da tela, do posicionamento das janelas pode fazer com que automação pare de funcionar.

## Próximos passos
O próximo projeto a ser feito para este curso da Hashtag Treinamentos, fará algo semelhante. Mas com melhorias na execução.

## Contribuições e contato
Meu contato no LinkedIn:
(inserir uma badge aqui e ver também como estão os meus contatos no linkedin)
