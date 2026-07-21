# INSTALAÇÃO: MICROSOFT OFFICE

Este guia detalha o **passo a passo** para instalar o Microsoft Office utilizando a ferramenta oficial de implantação da Microsoft.

---

## 📥 1. Download dos arquivos

Baixe o pacote de instalação no link abaixo e extraia o conteúdo para `C:\`:

- [Baixar MS Office Setup](https://github.com/matheuspessole/MS_Office_Setup/releases)

---

## ⚙️ 2. Procedimento de instalação

> **Atenção:** Este procedimento **não garante o licenciamento** do Microsoft Office. É necessária uma licença válida para ativação do produto.

### Passo 1 – Preparação

- Execute o arquivo `officedeploymenttool_17328-20162`.
- Quando o prompt for exibido, selecione a pasta onde os arquivos foram extraídos:
  ```
  C:\MS Office Setup
  ```

### Passo 2 – Instalação via Terminal

Abra o **Prompt de Comando (CMD)** como **Administrador** e execute os comandos abaixo:

```cmd
:: Acessa a pasta de instalação
cd C:\MS Office Setup

:: Inicia a instalação do Office
Setup.exe /configure Configuração.xml
```

---

## 🌐 Alterando o idioma da instalação (OPCIONAL)

Caso deseje instalar o Office em outro idioma, edite o arquivo **`Configuração.xml`** antes de iniciar a instalação.

Localize a linha:

```xml
<Language ID="pt-br" />
```

Altere o valor do atributo `ID` para o idioma desejado.

### Exemplos

| Idioma | Código |
|---------|--------|
| Português (Brasil) | `pt-br` |
| Inglês (Estados Unidos) | `en-us` |
| Espanhol | `es-es` |
| Francês | `fr-fr` |
| Alemão | `de-de` |
| Italiano | `it-it` |

> **Importante:** Após realizar a alteração, salve o arquivo `Configuração.xml` e execute novamente o comando de instalação.

---

## 📝 Observações

- Este repositório contém apenas os arquivos necessários para a instalação do Microsoft Office.
- O procedimento utiliza a **Office Deployment Tool (ODT)** oficial da Microsoft.
- A instalação **não ativa** o Office. Para utilizar o produto, é necessário possuir uma licença válida da Microsoft.
- Caso deseje instalar outra edição, arquitetura (32/64 bits) ou idioma, basta ajustar o arquivo `Configuração.xml` antes da instalação.
