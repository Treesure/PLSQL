Manual de instalação do softwares

Instalação Ferramentas Curso
Oracle XE 112_Win64
* Versão 11g do banco de dados oracle para compatibilidade ideal
* Máquina de uso pessoal -> Usuário Local e Administrador
* Durante a instalação, irá definir a senha de acesso ao banco
* Após a instalação, buscar o programa "Executar Linha de Comandos SQL"
* Digitar "connect system/senha_definida_na_instalacao". Se aparecer conectado, o banco
de dados foi instalado corretamente.
PLSQL Developer
* Install Trial Version -> Instalação completa
* Ao abrir o programa PLSQL Developer, será utilizado:
Username: system
Password: senha_definida_na_instalacao
Database: XE
* Será exibida uma opção para tradução do software para português e deve ser selecionado
conforme gosto pessoal.
* Na janela de inserção da chave de licença do produto, selecionar a opção "Trial".
Oracle Forms 6
* Importante instalar no diretório original sugerido na instalação.
Preparação para Utilização das ferramentas
* Abrir novamente o programa "Executar Linha de Comandos SQL" e digitar os seguintes
comandos (aguardar cada etapa finalizar para digitar a próxima):
connect system/senha_definida_na_instalacao as sysdba;
shutdown immediate;
startup restrict;
alter database character set internal_use WE8ISO8859P1;
alter database national character set internal_use UTF8;
alter system set sec_case_sensitive_logon = FALSE SCOPE=BOTH;
shutdown immediate;
startup;
Após isso, deve ser realizada a configuração do TNSNAMES do Oracle Forms:
* Acessar C:\oraclexe\app\oracle\product\11.2.0\server\network\admin e copiar o arquivo
tnsnames.ora
* Em seguida, acessar a pasta C:\orant\NET80\ADMIN e colar o arquivo copiado do
tnsnames
* Para testar a conexão, abrir o Form Builder, fechar a janela de inicialização e pressionar
Ctrl + J, digitando os dados para conexão ao banco.
Downloads
* senha para download: HandsOn.2024
Forms
https://maxiconsystemscombr-my.sharepoint.com/:u:/g/personal/bernardo_zanetti_maxicons
ystems_com_br/EdyVI2HThUVNqIsbkXJm0ysBNszRu8DWde_hNOr6qVDhvg?e=ihx2ja
OracleXe
https://maxiconsystemscombr-my.sharepoint.com/:u:/g/personal/bernardo_zanetti_maxicons
ystems_com_br/EbO-jRyPm6BLrRewQHqGcx8BqTf_QU9wbw_h0uyR4djg8w?e=4oQFkT
PLSQL Developer
https://maxiconsystemscombr-my.sharepoint.com/:u:/g/personal/bernardo_zanetti_maxicons
ystems_com_br/EeIiOYuT7JJCoL0w3ksEBFIBgwun7cGpvPxUzMokSdeolg?e=BMPUBE
