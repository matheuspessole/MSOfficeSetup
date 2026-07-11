# INSTALAÇÃO: MICROSOFT OFFICE

Este guia detalha passo a passa para instalar Microsoft Office oficialmente.

---

### 📥 1. DOWNLOAD DOS ARQUIVOS
Obtenha o pacote de instalação no link abaixo e extraia o conteúdo para `C:\` :
* [Baixar MS Office Setup](https://github.com/matheuspessole/MS_Office_Setup/releases)

---

### ⚙️ 2. PROCEDIMENTO DE INSTALAÇÃO
>ATENÇÃO: O procedimento não garante o licenciamento do software.

**Passo 01: Preparação**
* Execute o arquivo `officedeploymenttool_17328-20162`.
* No prompt que abrir, selecione o local da pasta do arquivo extraído: `C:\MS Office Setup`.

**Passo 02: Instalação via Terminal**

Abra o Prompt de Comando (CMD) como Administrador e execute os comandos na ordem:

```cmd
:: Acessa a pasta de destino
cd C:\MS Office Setup

:: Inicia a instalação do Office
Setup.exe /configure Configuração.xml
```
---
