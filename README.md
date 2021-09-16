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
  
![OPP1](https://user-images.githubusercontent.com/49697760/133624338-34fc9427-d370-47d4-9170-b17848f0b6f3.jpg)
- Preencha "Procedure" com: PDJOSQL1, por exemplo;
- Preencha "Job número" com: 9999, por exemplo;
- Preencha arquivo com o nome do arquivo gerado em homologa: BBN.@@DJOSQL...
- Preencha a opção com 5 e mande submeter  
  
![OPP2](https://user-images.githubusercontent.com/49697760/133624565-94772ec2-3b02-4a8b-a726-5157d62f2019.jpg)
![OPP6](https://user-images.githubusercontent.com/49697760/133628267-9e060f1a-2b7f-4a8e-9a9d-7ab2918648a2.jpg)  
  
5 - Gravar PDB2 no OPP:
  - No OPP entre na opção 21:
  
![OPP5](https://user-images.githubusercontent.com/49697760/133627287-b185e04e-5f90-4c80-b899-bf4e9d810af2.jpg)
  
  - Na procedure preencha com: "PDB2E180";
  - Aplicativo: DJO;
  - Data-sharing: D8G5;
  - Arquivo: nome do arquivo gerado em homologa;
  - Telefone: seu telefone;
  - Motivo: PF4 para verificar, mas normalmente, 32;
  - Dtmov: data atual;
  - ENTER para execução imediata;

6 - Solicitar para um funcionário liberar. A partir da liberação as tabelas já vão sofreer as ações dos códigos SQL do arquivo executado.
