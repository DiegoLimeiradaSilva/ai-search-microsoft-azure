# ai-search-microsoft-azure

- Passo a passo de experimento utilizando **Azure Ai Search** indexação e mineração de dados. 
- Realizado como desafio de projeto no Bootcamp **Microsoft Azure AI Fundamentals** da [Dio.me](https://dio.me)
- Documentação: [https://aka.ms/ai900-ai-search](https://aka.ms/ai900-ai-search)

<br/>

## Passo 1
- Abrir a página do Portal [https://portal.azure.com/#home](https://portal.azure.com/#home), buscar e selecionar o "Ai Search"

![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/303445553-8ea85c0c-c98f-43c2-9d44-2f43f407be3f.png?raw=true)

## Passo 2
- Clique em "Create" para criar um novo search service e preencha as informações de acordo com a ordem da imagem abaixo:

![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/02.png?raw=true)

- Depois que as informações são validadas, é aberta uma tela com as configurações. Clique em "Create".

 ![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/03.png?raw=true)

- Depois da confirmação de criação, clique em "Go to resource"

![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/04.png?raw=true)

## Passo 3
- Precisamos criar agora um recurso de IA
- De volta à Home do [Portal Azure](https://portal.azure.com/#home), no menu lateral, clique em "Create a resource", escolha "AI + Machine Learning", depois "Azure Ai Services"

![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/06.png?raw=true)

## Passo 4
- Preenche com as informações segundo a imagem abaixo. Clica em "Review + Create"

![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/07.png?raw=true)

- Após validação das informações, clica em "Create"

![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/08.png?raw=true)

- Aguarde até a finalização da criação do recurso.

![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/09.png?raw=true)

## Passo 5
- Agora criaremos uma conta de armazenamento
- Volte à home do [Portal Azure](https://portal.azure.com/#home), busque e selecione "storage accounts"

![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/10.png?raw=true)

## Passo 6
- Clique então em "Create"

![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/11.png?raw=true)

- Preencha os dados conforme imagem abaixo. Os demais que não estão numerados, possivelmente já virão preenchidos.

![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/12.png?raw=true)

- Após a validação dos dados, clique em "Create"

![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/13.png?raw=true)

- Depois de criado, clique em "go to resource"

![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/14.png?raw=true)

## Passo 7
- Na tela do storage, no menu lateral esquerdo, procure e selecione a opção "configuration". Ela vai abrir a tela da direita que está sendo mostrada abaixo. Clique para habilitar a opção conforme imagem e clique em "save".

![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/15.png?raw=true)

## Passo 8
- No menu lateral esquerdo, clique em "Containers", depois em "+ containers", que abrirá uma aba lateral, que deve ser preenchida conforme imagem abaixo. Depois clique em "create".

![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/16.png?raw=true)

## Passo 9
- Depois de criado, as informações são atualizadas na tela. Selecione para abrir o container.

![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/17.png?raw=true)

## Passo 10
- Em um novo navegador, faça o download do zip contido no link fornecido na documentação: [https://aka.ms/mslearn-coffee-reviews](https://aka.ms/mslearn-coffee-reviews), e extraia os arquivos em uma pasta "reviews"
- Clique então em upload, que abrirá uma aba lateral. Selecione então todos os arquivos descompactados, e clique em "upload"

![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/18.png?raw=true)

-E assim ficam os arquivos carregados
  
![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/19.png?raw=true)

## Passo 11
- Agora voltamos ao Ai Search, através do campo de busca.

 ![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/20.png?raw=true)

- Selecione o serviço criado anteriormente

![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/21.png?raw=true)

- Clique em "import data"

![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/22.png?raw=true)

## Passo 12
- Selecione o Azure Blob Storage

![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/23.png?raw=true)

- Preencha os dados conforme os passos na imagem.
- A informações não presentes nos passos já vêm preenchidas, ou devem ser deixadas em branco.

![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/24.png?raw=true)

## Passo 13
- Na aba "Add Cognitive skills (optional)", em "Attach AI Services", selecione seu recurso.

![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/25.png?raw=true)

- Em "add enrichments" preencher conforme imagem abaixo

![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/26.png?raw=true)

- Em "Save enrichments to a knowledge store", selecione "Image projections".
  - Ao aparecer a mensagem abaixo, selecione "choose an existing connection"
    
       ![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/27.png?raw=true)
       - Escolha o storage criado anteriormente
    
       ![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/28.png?raw=true)

       - Depois clique em "+ container", e siga os passos da imagem abaixo
    
       ![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/29.png?raw=true)

       - Selecione então o knowledge-store e clique em "select"

       ![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/30.png?raw=true)

  - Selecione as demais informações conforme imagem abaixo e clique em "Next: Customize target index"
      
  ![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/31.png?raw=true)
  ![image](https://github.com/giselle-ferreira/ai-search-microsoft-azure/assets/84051263/9526b769-a45c-42b0-8d15-f09132d4875f)

## Passo 14
- Na aba "Customize target index", preencha conforme imagem abaixo

![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/32.png?raw=true)

## Passo 15
- Em "Create an indexer", preencha conforme imagem abaixo

![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/33.png?raw=true)

 - Abra a aba "Advanced options", marque a opção "Base-64 Encode Keys", e clique em "submit"
   
![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/34.png?raw=true)

![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/35.png?raw=true)

## Passo 16
- Abrir o Azure AI Services| Ai Search, e clicar em Search Explorer

![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/36.png?raw=true)

## Passo 17
- No Search Explorer, inclua a query fornecida pela documentação ```search=*&$count=true```, e clique em "search"

![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/37.png?raw=true)

- Agora filtramos pela localização ```search=locations:'Chicago'``` e ele vai trazer as reviews com os sentimentos de cada.

![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/38.png?raw=true)

- Agora filtramos pelo sentimento negativo ```search=sentiment:'negative'```

![image](https://github.com/DiegoLimeiradaSilva/ai-search-microsoft-azure/blob/main/imagens/40.png?raw=true)


##

## Comentários
Muito interessante a funcionalidade da ferramenta para estabelecimentos que prestam serviço. A análise funciona muito bem identificando as frases-chaves, sentimento, localização, e a busca agrega de forma correta todas essas informações. É possível saber quais são as causas das reviews negativas, por exemplo, já que as frases-chaves trazem essa informação. Assim, fica mais fácil de resolver o problema da insatisfação do cliente.

##


