# 📲 Automação de Envio de Mensagens via WhatsApp com Python

Este projeto automatiza o envio de mensagens personalizadas via **WhatsApp Web** utilizando **Python** e dados de uma planilha do Excel. Ideal para equipes de **cobrança**, **relacionamento com cliente**, **comercial** e outras áreas que precisam enviar mensagens em escala, sem abrir mão da personalização.

---

## 🚀 Funcionalidades

- 📂 Leitura de contatos a partir de uma planilha `.xlsx`
- 🧾 Geração automática da URL do WhatsApp com número e mensagem usando `quote()` da biblioteca `urllib.parse`
- 🌐 Abertura do WhatsApp Web já com o contato e a mensagem preenchida
- 🖱️ Interação com o navegador usando `PyAutoGUI`
- 📊 Geração de um relatório `.csv` com os contatos que apresentaram erro durante o envio

---

## 🧠 Tecnologias Utilizadas

- [Python 3.x](https://www.python.org/)
- [OpenPyXL](https://openpyxl.readthedocs.io/en/stable/) – Leitura da planilha Excel
- [PyAutoGUI](https://pyautogui.readthedocs.io/en/latest/) – Automação de cliques e envio
- [Urllib.parse](https://docs.python.org/3/library/urllib.parse.html) – Codificação da mensagem para URL
- [Webbrowser](https://docs.python.org/3/library/webbrowser.html) – Abertura do navegador

---

## 📁 Estrutura Esperada da Planilha

A planilha `.xlsx` deve conter os seguintes dados a partir da segunda linha (a primeira linha é o cabeçalho):

| Grupo | Cota | Nome | Telefone |
|-------|------|------|----------|
| 123   | 456  | João | 5511999999999 |

---

## ▶️ Como Usar

1. Instale os pacotes necessários:

```bash
pip install openpyxl pyautogui
````

2. Coloque sua planilha no mesmo diretório do script e renomeie para `Contatos Teste.xlsx` (ou ajuste o nome no código).

3. Execute o script:

```bash
python enviar_mensagens.py
```

4. O WhatsApp Web será aberto automaticamente. Faça login com o QR Code (apenas na primeira execução) e aguarde o envio das mensagens.

---

## ❗ Observações

* O número de telefone deve estar no formato internacional (ex: `5511999999999`)
* É necessário que o contato esteja salvo e disponível no WhatsApp
* Os erros durante o envio (número inexistente, sem conta WhatsApp, etc.) são salvos em um arquivo `contatos_com_erro.csv` para verificação posterior

---

## 📬 Contribuição

Sugestões e melhorias são sempre bem-vindas! Sinta-se à vontade para abrir uma *issue* ou enviar um *pull request*.

---

## 📝 Licença

Este projeto está licenciado sob a [MIT License](LICENSE).

---

Feito com 💻 e ☕ para automatizar o que for possível!


👨‍💻 Autor Rodrigo de Lima Aleixo
- 💼 [LinkedIn](https://www.linkedin.com/in/rodrigo-de-lima-aleixo-850b1720b/)
- ✉️ E-mail: *rodriigoaleixo@gmail.com*
