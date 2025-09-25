# API-3

<div align="center">

 <img width=100% src="https://capsule-render.vercel.app/api?type=venom&height=300&color=000&text=VoNa%20Kombi&fontColor=C4B454"/>
 </div>

# Proposta
 Realizar um estudo aprofundado sobre o fluxo logístico e comercial dos produtos destinados à exportação, abrangendo os principais modais de transporte utilizados, bem como a análise dos valores transacionados sob a modalidade FOB (Free on Board), o valor agregado das mercadorias, a quantidade total exportada em toneladas ou unidades, e a identificação das principais regiões geoeconômicas com maior concentração e circulação de mercadorias.

A análise também deve contemplar uma projeção para o ano de 2025, considerando variáveis econômicas, tendências de mercado internacional, acordos comerciais vigentes, expansão da infraestrutura logística e potenciais gargalos operacionais.

Paralelamente, será conduzido um exame detalhado dos principais destinos internacionais envolvidos nas relações comerciais de importação e exportação, com a identificação dos países com maior representatividade no volume e valor das trocas comerciais, os produtos com maior participação na pauta exportadora e importadora, bem como os segmentos industriais mais relevantes em termos de competitividade e presença internacional.
# MVP
## Primeiro Sprint

<img width=50% src="Imagens/MVP1.gif"/>
Foi desenvolvido um dashboard interativo para análise dos dados de exportação, apresentando a quantidade exportada e o valor FOB das mercadorias. A ferramenta permite filtros por país de destino, mês e modal de transporte (rodoviário, ferroviário, marítimo, aéreo ou multimodal), proporcionando uma visualização dinâmica e estratégica dos fluxos logísticos e comerciais. Com isso, é possível identificar sazonalidades, avaliar a eficiência dos modais e analisar a relevância dos mercados internacionais de forma segmentada.

## Segundo Sprint

 <img width=50% src="Imagens/MVP2.gif"/>
 O layout do dashboard foi reformulado com foco em usabilidade, clareza visual e padronização da identidade visual institucional, facilitando a interpretação dos dados por diferentes perfis de usuários. Foram corrigidos erros de filtragem que comprometiam as análises, com a aplicação de consultas SQL otimizadas para segmentação dos dados em tabelas específicas, garantindo maior precisão e integridade das informações.

Adicionalmente, foram implementadas regras de exclusão para territórios classificados como paraísos fiscais, a fim de evitar distorções nos indicadores comerciais e assegurar maior conformidade com práticas de transparência fiscal e padrões internacionais de reporte estatístico.

## Terceiro Sprint
 <img width=50% src="Imagens/MVP3.gif"/>
 Para tornar o dashboard mais dinâmico, foi criado um menu que pode levar o usuario para quatro telas diferentes, cada uma focada em um tipo de dado: quilograma líquido, valor FOB, valor agregado e URFs.
 Nessas telas foram adiocionados mais informaçoes e filtros, como a projeção para o ano de 2025 e também a média de exportação por valor agregado e valor FOB

 
 <h1>Link do Dashboard</h1>

 <a href="https://app.powerbi.com/view?r=eyJrIjoiYzE3MTVlMWMtOGU0OC00OWZkLTg0YWEtOTdiYzBjMzM1Nzc1IiwidCI6ImNmNzJlMmJkLTdhMmItNDc4My1iZGViLTM5ZDU3YjA3Zjc2ZiIsImMiOjR9">
  <img src="https://img.icons8.com/?size=100&id=46377&format=png&color=000000"></a>



 # Ferramentas Utilizadas
 - Jira Software
 - Excel
 - Power Point
 - Microsoft Word
 - SQL Workbench
 - Power BI

 # Aplicabilidade das Ferramentas
 ##  Para facilitar o tratamento dos dados, foi feita a filtragem e posterior substituição dos códigos dos municípios por seus respectivos nomes com o objetivo de organizar e analisar os dados comerciais dessas regiões, facilitando a interpretação e uso posterior.
<div align="center">
<img src="Imagens/Ferramentas.png" alt="/Imagens Git/Ferramentas Utilizadas" width="750"/>
 </div>

 ### Jira Software
  Através dele foi desgnada a tarefa e o prazo das atividades de cada membro do projeto, indicando o nivel de prioridade de cada tarefa a ser realizada e em qual sprint devem ser entregues organiando em anexos os outros aplicativos utilizados

 ### SQL
  A planilha principal como fonte de dados ultrapassavam os limites de linhas e colunas suportados pelo Microsoft Excel, inviabilizando sua manipulação direta na aplicação, então ela foi dividida em planilhas menores separadas por ano. Para contornar essa restrição, os dados foram importados e processados no SQL Workbench, onde foram aplicados filtros e transformações para gerar tabelas segmentadas conforme os critérios analíticos definidos. Considerando a ausência de integração nativa entre o SQL Workbench e o Power BI, foi configurado o driver MySQL Connector/ODBC, permitindo a conexão via ODBC e a extração dos dados diretamente para o Power BI. Essa abordagem possibilitou a atualização dinâmica e o consumo eficiente das informações na camada de visualização.
 ### Excel
  Para viabilizar a filtragem da planilha principal por meio de consultas SQL, foram gerados diversos arquivos auxiliares contendo planilhas segmentadas de forma criteriosa, organizadas exclusivamente com os dados relevantes e estruturadas por ano. Essa abordagem permitiu otimizar o desempenho das consultas, reduzir a complexidade dos dados processados e facilitar a manipulação e análise das informações históricas de maneira eficiente e escalável..
  
  
 # Backlog do Produto
 
 <table>
 <tr>
  <td>1º Sprint</td> <td> filtragem superficial dos dados para montar o esboço do dashboard</td>
 </tr>
 <tr>
  <td>1º Sprint</td> <td>Prieiro dashboard indicando valor FOB e quantidade de exportações para cada país em cada mês</td>
 </tr>
<tr>
 <td>2º Sprint</td> <td>Filtragem e exibição da matriz de origem e destino</td>
</tr>
  <tr>
 <td>2º Sprint</td> <td>Tratamento de dados a partir da integração com o SQL Workbench</td>
   </tr>
 <tr>
  <td>2º Sprint</td> <td>Segunda tela interativa condendo dados com NCM</td>
</tr>
<tr>
 <td>2º Sprint</td> <td>Verificação de rotas e valores absurdos no banco de dados</td>
</tr>
<tr>
 <td>2º Sprint</td> <td>Integração de dados de 2023 e 2024 ao banco de dados</td>
</tr>
<tr>
 <td>3º Sprint</td> <td>Comparativo da movimentação dos estados brasileiros</td>
</tr>
<tr>
 <td>3º Sprint</td> <td>Entendimento da sazonalidade de cada modal logístico</td>
</tr>
<tr>
 <td>3º Sprint</td> <td>Adição de uma tela menu ao dashboard</td>
</tr>
<tr>
 <td>3º Sprint</td> <td>Remoção de paraísos fiscasis</td>
</tr>
<tr>
 <td>3º Sprint</td> <td>Exibir quais foram os países que mais importaram do Brasil e qual o estado brasileiroquemais movimenta cargas</td>
</tr>
 </table>

 

# Equipe

<table>
<tr>
<td>Scrum Team</td>
 <td>Breno Conrado</td>
<td><a href="https://www.linkedin.com/in/bcconrado?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a></td> 
</tr>
 <tr>
  <td>Scrum Team</td>
<td>Eduardo Pereira</td>
<td><a href="" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a></td> 
</tr>
 <tr>
  <td>Scrum Team</td>
<td>Gabriel Poffo</td>
<td><a href="https://www.linkedin.com/in/gabriel-poffo-73321335b?trk=contact-info" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a></td> 
</tr>
 <tr>
  <td>Scrum Team</td>
<td>Kauê Venâncio</td>
<td><a href="" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a></td> 
</tr>
 <tr>
  <td>Scrum Master</td>
<td>Leonardo Rocha</td>
<td><a href="https://www.linkedin.com/in/leonardo-rocha-alves-921617306?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a></td> 
</tr>
 <tr>
  <td>Scrum Team</td>
<td>Mateus Alexandre</td>
<td><a href="https://www.linkedin.com/in/matheus-alexxandre?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=ios_app" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a></td> 
</tr>
 <tr>
  <td>P O</td>
<td>Pedro Hernandes</td>
<td><a href="https://www.linkedin.com/in/pedro-hernandes-720486212?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a></td> 
</tr>
 <tr>
  <td>Scrum Team</td>
<td>Yago Martins</td>
<td><a href="https://www.linkedin.com/in/yago-martins-9a403315a?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a></td> 
</tr>
</table>
