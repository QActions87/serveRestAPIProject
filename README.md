# serveRest API Project
![JavaScript010101](https://api.devicons.dev.br/icon?icons=Linux%2CPostman%2CJavaScript%2CGithub%2CGithubActions&size=48&theme=light&perline=30)

Criação de testes de API do manual ao CI/CD utilizando Postman, newman e newman-htmlextra

#
## Tecnologias usadas:
 - **Postman** versão Desktop e Web
 - **Node v20.13.1**
 - **nweman 6.2.2**
 - **newman-reporter-htmlextra v1.23.1**

#
## Documentações:
 - Doc da API: [**Swagger**](https://serverest.dev/?lang=pt-BR#)
 - Pipeline CI: [Click! ](https://github.com/QActions87/serveRestAPIProject/blob/main/.github/workflows/pipelineCI-CD.yml)
#
## Como instalar o ambiente:
 - **1º Instale** o [**nodejs**](https://nodejs.org/pt-br)
 #
 - **2º Instale o newman** globalmente:
   
```
npm install -g newman
```
#
 - **3º Instale o newman htmlextra** globalmente [dependência do **relatório** (opcional)]:
   - [**Documentação** do newman-reporter-htmlextra](https://www.npmjs.com/package/newman-reporter-htmlextra)

```
npm install -g newman-reporter-htmlextra
```

 - **4º Fork do Projeto**:
   - execute o comando dentro do diretório pai do projeto:
```
git clone https://github.com/QActions87/serveRestAPIProject.git .
```


#
## Como rodar os testes:

### 1º Manual no Postman:

 - I - Import a collection "**ServeRest_collection.json**", que está no **diretório** 'serveRestAPIProject/ServeRest.
    
 - II - Execute os testes individualmente.
/ServeRest_collection.json'.
      
### 2º Automatizado no Postman:
 - I - Import a collection "**ServeRest_collection.json**", que está no **diretório** 'serveRestAPIProject/ServeRest'.
 - II - execute o 'run' na collection.
   
#
### 3º Automatizado no Postman com massa de dados em csv:
 - I - Import a **collection** "**postman_collection_UsarComCSV.json**", que está no **diretório** 'serveRestAPIProject'
/ServeRest/'.
 - II - execute o 'run' na collection.
 - III - Fazer o upload da massa de dados no arquivo csv "**serverest_dados.csv**", que está no **diretório** 'serveRestAPIProject/ServeRest
/massa-de-dados/'.
 - III - Executar o teste automatizado.
#
### 4º Conferir o html gerado no relatório da execução que realizei:
 - I - Dar 2 cliques no arquivo "**newman_htmlextra-2026-05-21-02-26-58-245-0.html**", que está no **diretório** 'serveRestAPIProject/ServeRest
/newman/' e dar dois cliques no arquivo '**.html**'.
 - II - Para verificar o relatório de sua própria execução, de dentro do **diretório X** execute:
  ```
      newman run ServeRest_collection.json -r cli,htmlextra
  ```
 - III - Verificar novo relatório no diretório 'serveRestAPIProject/ServeRest
/newman/' e dar dois cliques no arquivo '**.html**' com a data do dia em que executou.




















