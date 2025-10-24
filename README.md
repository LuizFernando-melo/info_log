# info_log
# Trabalho de informatica
<img width="1882" height="727" alt="Captura de tela 2025-10-24 195357" src="https://github.com/user-attachments/assets/346f82b1-7126-427e-aa93-82fb5be1f30e" />
Gerar tabela e gráfico dinâmico para visualização dos dados
Usando fórmulas responder às perguntas a seguir: 

a) quantos municípios foram contemplados nos dados? (REMOVER DUPLICATAS - CONT.VALORES) 
      =CONT.VALORES(A$1:A$1048575)-1
      
b) quantas especialidades foram consideradas nos dados? (REMOVER DUPLICATAS - CONT.VALORES)
      =CONT.VALORES(F:F)-1
      
c) quantos tipos de Natureza Jurídica foram considerados nos dados? (REMOVER DUPLICATAS - CONT.VALORES)  
      =CONT.VALORES(K:K)-1
      
d) quantos restaurantes estão cadastrados em  São José dos Campos? (CONT.SES) 
      =CONT.SES(base_dados!J:J,"São José dos campos",base_dados!R:R,"Restaurante")
 Ao digitar o CNPJ em uma linha, deve ser retornado Nome Fantasia (PROCV e SEERRO)
        =PROCV(D8,base_dados!B:C,2,0)
        
 Ao digitar o CNPJ em uma linha, deve ser retornada Situação da Atividade (PROCV e SEERRO)
        =PROCV(formulas!D8,base_dados!B:D,3,0)
Ao digitar o CNPJ em uma linha, deve ser retornada Natureza Jurídica (PROCV e SEERRO) 
         =PROCV(D8,base_dados!B:F,5,0)
Ao digitar o CNPJ em uma linha, deve ser retornada UF (PROCV e SEERRO)
         =PROCV(D8,base_dados!B:S,8,0)
Ao digitar o CNPJ em uma linha, deve ser retornada TIPO (PROCV e SEERRO)
            =PROCV(D8,base_dados!B:S,17,0)
Ao digitar o CNPJ em uma linha, deve ser retornada Especialidade (PROCV e SEERRO)
            =PROCV(D8,base_dados!B:S,18,0)
Elaborar mais 5 perguntas que os dados, presentes no arquivo obtido, possam responder.
          Nº de microempresas; =CONT.SES(base_dados!G:G,"MICROEMPRESA")
          Nº comida brasileira; =CONT.SES(base_dados!S:S,"Brasileira")
          Nº comida Asiática; =CONT.SES(base_dados!S:S,"Asiática")
          Nº de bar em SP; =CONT.SES(base_dados!R:R,"Bar",base_dados!J:J,"São Paulo")
          Nº DE Filial; =CONT.SES(base_dados!E:E,"Filial")
https://fatecspgov-my.sharepoint.com/:x:/r/personal/luiz_melo11_fatec_sp_gov_br/Documents/restaurante.xlsx?d=w48061e1cdf2c4a61b3c4e630a495b67e&csf=1&web=1&e=wiY0Cg
