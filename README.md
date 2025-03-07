# Inteligência Artificial (IA) com Azure - Visão Computacional
Criar repositorio onde será salvo o projeto juntamente configurar AI Vision Service e realizar testes práticos.


### Ferramentas utilizadas:

- Portal Azure: https://portal.azure.com/#home
- Portal Studio Vision : https://portal.vision.cognitive.azure.com/

### Pontos Importantes:

- Caso esteja realizando apenas um prática de estudo, no final excluir tudo que foi construído nesse laboratório. Desta forma, minimiza o risco de ser cobrado algum valor. Lembre-se você está em um ambiente real de produção.
- Documentação:
    + https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/03-image-analysis.html
    + https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/04-face.html
    + https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/05-ocr.html

### Resumo (Passo-a-passo): Configuração Vision Service:

- Entrar no ambiente Azure
- Criar o resource onde será salvo o projeto
- Entrar no Studio IA
- Definir o resource como Default

### Detalhamento (Passo-a-passo): Configuração Vision Service

01 - Criar o serviço que iremos utlizar confirme link abaixo:

https://github.com/igorferrer-data/azure-ml-vision

### Após concluir a as configurações acima, Entrar no portal: ``` https://portal.vision.cognitive.azure.com/ ```

Esse portal é o Studio onde vamos trabalhar com a Inteligência Artificial (IA)

05 - Após realizar o login no site do Studio, então selecionar o resource criado na configuração acima. Clicar para visualizar todos resources.
![image](https://github.com/user-attachments/assets/f8221fac-044a-46a9-9282-3f6ff24a9294)

06 - Agora, selecionar o resource criado e clicar no botão ``` Select as default resource ```. Se tiver tudo certo, não vai acontecer nada. A tela não vai tremer! ksksk. Então click no botão ``` X ``` para voltar a tela anterior.
![image](https://github.com/user-attachments/assets/895c1d5f-d79e-446c-abb6-c5ae3273d704)

### Atenção

Caso esse ultimo passo apresente erro: ResourceOperationFailure: Resource provider [N/A] isn't registered with Subscription [N/A] . Então, deve realizar uma configuração e refazer a confiuração acima.
   * Ir no portal da Azure: https://portal.azure.com/#home, fazer o login
   * Na barra de pesquisa, escrever "Subscription"
   * Selecionar o Subscription Name
   * Vai abrir um novo menu, então selecionar "Resource providers"
   * Selecionar:
      + Microsoft.Cdn
      + Microsoft.CostManagement
   * Clicar no botão acima "Register".

   ![image](https://github.com/user-attachments/assets/79e279f1-96a9-4301-978a-71128c464908)

### Orientação Geral
- Todos os testes vai precisar do seu aceito que estará utilizando o resource criado. Isso quer dizer que vai ser cobrado.
![image](https://github.com/user-attachments/assets/3d77e0dd-db28-4a24-a2ec-688d752e70ee)

- Os testes são bem intuitivo e a propria ferramenta tras alguns exemplos e você pode selecionar alguma imagem propria. O resultado fica logo em baixo:
![image](https://github.com/user-attachments/assets/101fb7ce-7f99-463b-954c-79c4f897dd09)

- Os testes realizados neste material foram com imagem proprias. Não utilizei os exemplos da ferramenta.
- Para voltar a tela com o menu dos serviçoes disponibilizado tem um botão ``` X  ```, na parte superior da tela.
  
### Teste 01 - Identificar pessoas na foto:
1 - Selecionar ``` Face  ```, depois ``` Detect faces in an image  ```
![image](https://github.com/user-attachments/assets/96ca218a-65af-4c9d-8b3d-6b3ee62b534e)

![image](https://github.com/user-attachments/assets/010e5ef0-7bd3-4cf3-8404-5f7759863f30)


### Teste 02 - Identificar texto na foto:
![image](https://github.com/user-attachments/assets/30df6005-95c3-4cba-8be6-d59778a506e6)




### Teste 03 - Descrevendo a imagem/foto:
![image](https://github.com/user-attachments/assets/1ce9c879-e482-40f6-bf07-2b59738bdfd0)

![image](https://github.com/user-attachments/assets/47e418f5-a1d4-43a9-b451-9d20cf8d4543)


### Ferramenta suporta:
- Integração com aplicações
   * https://learn.microsoft.com/en-us/azure/ai-services/computer-vision/quickstarts-sdk/identity-client-library?tabs=windows%2Cvisual-studio&pivots=programming-language-csharp
   * https://github.com/Azure-Samples/azure-ai-vision/tree/main/face
- Letura de texto na imagem/foto:
   * Diversos idiomas
   * Escrito a mão
   * Formulários e já transformar em banco de dados
- Gera arquivo JSON com o resultado

Links de ajuda:
   * https://learn.microsoft.com/en-us/answers/questions/1983847/error-while-creating-a-managed-online-endpoint-in
   * https://learn.microsoft.com/en-us/answers/questions/2129910/resource-provider-(n-a)-isnt-registered-with-subsc

