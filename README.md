# Guia de Configuração: Microsoft Office

Este documento estabelece o protocolo padrão para a instalação e configuração do ambiente Microsoft Office. Siga as instruções estritamente para garantir a correta implantação do software.

---

## Procedimento Operacional

### 1. Preparação de Diretório
Mova o diretório de instalação para a raiz do sistema:
* Local: `C:\`

### 2. Extração de Componentes
1.  Execute o binário `officedeploymenttool_17328-20162`.
2.  No prompt de destino, selecione o diretório: `C:\MS Office Setup`.
3.  Confirme o processamento de extração dos arquivos necessários.

### 3. Execução via Linha de Comando (Administrador)
Para proceder com a instalação, utilize o terminal com privilégios elevados:

1.  Abra o **Prompt de Comando (CMD)** como Administrador.
2.  Navegue até o diretório de configuração:
    ```cmd
    cd C:\MS Office Setup
    ```
3.  Inicie o processo de configuração utilizando o arquivo de parâmetros:
    ```cmd
    Setup.exe /configure Configuração.xml
    ```

---

## Notas de Operação
* Certifique-se de que o arquivo `Configuração.xml` esteja presente no diretório `C:\MS Office Setup` antes de executar o comando final.
* A execução requer privilégios de administrador para modificação de registros e arquivos de sistema.
