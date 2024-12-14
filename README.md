# sqlrdd
SQLRDD

Como gerar para Windows + "xHarbour 1.2.3 Intl. (SimpLex) (Build 20201212)" + BCC 5.5:

- Instalar BISON
- Copiar arquivos da pasta BIN do BISON para a pasta BIN do xHarbour
- Copiar o XHBMK2.EXE do Harbour para a pasta BIN do xHarbour
- Na pasta SOURCE do SQLRDD, executar o comando :
  HBMK2 -xhb sqlrdd.hbp

- Vai gerar o arquivo sqlrdd.lib

- Lembrar de configurar o path, include, etc. do xHarbour para a versão correta do compilador

- A versão gerada funciona também com o FWH 12.08 (é a verão que uso, só testei com essa versão)

- A versão gerada não inclui acesso ao FIREBIRD (está com erro na compilação). Como só uso o MariaDB não
  é uma preocupação imediata pra mim

- Tentei gerar para a versão "xHarbour Compiler build 1.2.1 (SimpLex) (Rev. 9575)", mas não gerou. Pelo que
  verifiquei dos erros ( sinalização de PCODE faltando, erros de defines, etc.) acho que o fonte da SQLRDD
  não é mais compatível com essa versão do xHarbour
