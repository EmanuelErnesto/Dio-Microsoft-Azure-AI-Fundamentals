# Reconhecimento Facial e transformação de Imagens em Dados no Azure ML.


## As imagens utilizadas neste passo a passo estarão na pasta "Images" enquanto que as utilizadas para alimentar a IA estarão em "inputs". As saídas estarão na pasta "Output"


# Etapa 1 - Criação do recurso.

<img src = "./images/image1.jpeg">

## Para iniciar, é necessário criar primeiramente um recurso. Para isso, clique em create a resource, ou "criar um recurso" a depender de seu idioma. Na nova tela, clique em "IA + Machine Learning" no canto esquerdo da tela e em seguida vá em "serviços cognitivos - criar" ou "Azure AI Services."

<img src = "./images/image2.jpeg">

## Em resource group é só selecionar o grupo de recursos que você possui. Caso ainda não tenha, clique em criar e preencha as informações pedidas para criação de um novo resource group. Em região é preferível East US por ter um valor monetário menor nos gastos, em nome pode selecionar o que desejar e em tipo de preço Standard S0. Após isso é só marcar a caixa confirmando que leu os termos abaixo e clicar em Examinar + criar.

<img src = "./images/image3.jpeg">

## É só clicar em criar que será criado seu recurso, então estará pronto para as próximas etapas.

# Etapa 2: Configuração no Azure Cognitive Vision

<img src = "./images/image4.jpeg">

## Após concluir as etapas anteriores, acesse https://portal.vision.cognitive.azure.com/gallery/featured e clique em view all resources

<img src = "./images/image5.jpeg">

## Clique no ícone à esquerda do nome do seu resource, e após isso clique em select as default resource.


## Etapa 3 - Análise de imagens

### Caso tenha concluído as etapas passadas, agora é possível fazer a análise de imagens e documentos! 

<img src = "./images/image6.jpeg">

## Na página inicial do Vision Studio, ao descer um pouco a página, você deverá primeiro encontrar onde está o recurso para reconhecimento de imagens. Para exibir o serviço de reconhecimento facial, clique em "Face". Logo após, você verá a opção "detect faces in a image". A partir disso, clique em Try It out.

<img src = "./images/image7.jpeg">

## Você será redirecionado a esta tela. Nela, haverão alguns exemplos de imagem que pode usar para testar o serviço de reconhecimento facial do Azure.

<img src = "./images/image8.jpeg">

## Caso não queira utilizar uma de suas fotos, pode utilizar como exemplo as disponibilizadas. Ao clicar nelas e marcar a opção "I acknowlege that this demo will incur usage to resource..." você poderá ver informações como o número de rostos e se está usando máscara. 

### Para testes, será usada a imagem de um pôster do filme "John Wick 4."

<img src = "./inputs/johnWick4-Imagem.png">

### A saída esperada é:

<img src = "./output/output-reconhecimento-facial.jpeg">

##

# Etapa 4 - Reconhecimento de documentos.

## Nesta etapa será feita a extração de textos em imagens.

<img src = "./images/image9.jpeg">

## Para começar, ao invés de clicar em "Face", desta vez deverá clicar em Optical character recognition, e logo após clicar em Try it out

<img src = "./images/image10.jpeg">

## Você poderá novamente escolher a imagem que desejar para tentar extrair o texto dela. Neste exemplo, utilizarei a do manifesto ágil.

<img src = "./output/output-extracao-texto.jpeg">

## Todo o texto da imagem, conforme esperado, foi digitalizado.

# Etapa 5 - Criação de legendas para imagens.

## Nesta etapa, será adicionado um "Caption" para a imagem selecionada.

<img src = "./images/image11.jpeg">

## Primeiro, você deverá selecionar "Image analysis", ir em "add caption to images" e clicar em try it out.

<img src = "./images/image12.jpeg">

<img src = "./images/image13.jpeg">

## Para o exemplo, utilizarei uma imagem extraída do evento MWC 2024.

<img src = "./output/output-adicao-caption.jpeg">

## O algoritmo reconheceu o ambiente e descreveu-o, havendo apenas um porém que foi ele não reconhecer os robôs caninos presentes tanto no chão quanto numa tela na parede.