# PDB2E180
Passo a passo para dar carga em tabelas de homologação.

1- Crie um arquivo em desenvolvimento com o(s) código(s) SQL;<BR>
2- No TSO de desenvolvimento entre com o comando TRA;<BR>
  - Opção = 1;<BR>
  - Classe para submissão = "O";<BR>
  - Job name para submissão = "J547TRA"<BR>
        
![TRA1](https://user-images.githubusercontent.com/49697760/133622675-d4fe7dd0-f565-4978-bde0-8cd6dca34ca2.jpg)        
        
  - Em "arquivo" informe o nome do arquivo como o SQL e selecione "HM" para homologação;
  
![TRA2](https://user-images.githubusercontent.com/49697760/133623240-b84c09da-20b4-4629-9946-c2bb47109b8e.jpg)        
  
  - Mande submeter: ENTER
 
![TRA3](https://user-images.githubusercontent.com/49697760/133623626-1040e7fa-7e9e-4889-ae77-88f8db2575ff.jpg) 
  
3 - Verifique se o arquivo foi gerado. Entre no ROSCOE de desenvolvimento e procure pelo arquivo: A D BBN.@@DJO+;
4 - Estando tudo OK deverá ser feito OVERRIDE do arquivo. Entre no OPP de homologa(Opção 23.1):
  
  
  
  
