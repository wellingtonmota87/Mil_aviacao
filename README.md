# ✈️ Sistema de Solicitação de Voo - MIL Aviação

Este projeto é uma aplicação web desenvolvida em **HTML**, **CSS** e **JavaScript** que permite o agendamento de voos personalizados com base nas aeronaves disponíveis da empresa **MIL Aviação**. O sistema também possibilita o envio de e-mails automáticos e o armazenamento local das informações.

---

## 🚀 Funcionalidades

- Interface moderna com imagem de fundo e logotipo da empresa.
- Botões de seleção para aeronaves (MIB, KRT, MEP, RBZ).
- Formulário dinâmico para preenchimento de:
  - Empresa solicitante
  - Data do voo
  - Origem e destino
  - Horário
  - Lista de passageiros (quantidade varia conforme a aeronave)
  - E-mail do solicitante
  - Data de solicitação (preenchida automaticamente)
- Armazenamento local (`localStorage`) das solicitações.
- Visualização de voos agendados em layout horizontal.
- Visualização individual da lista de passageiros.
- Cancelamento de solicitações com atualização automática da lista.
- Envio de dados por e-mail via [FormSubmit](https://formsubmit.co/).

---

## 🛠 Tecnologias Utilizadas

- HTML5
- CSS3
- JavaScript (Vanilla)
- [FormSubmit](https://formsubmit.co/) para envio de e-mails

---

## 📂 Estrutura Recomendada de Pastas

```
Mil_Aviacao/
│
├── index.html
├── estilos/
│   └── style.css (opcional, se separar o CSS)
├── scripts/
│   └── script.js (opcional, se separar o JS)
├── imagens/
│   ├── cessna-citation-gen3-novo_widelg.jpg
│   └── LOGO MIL AVIAÇÃO -.png
```

> **Observação:** Altere os caminhos das imagens no HTML para relativos (ex: `./imagens/LOGO MIL AVIAÇÃO -.png`) ao invés de absolutos (`C:/...`) para compatibilidade com outros computadores e deploy online.

---

## 📧 Configuração do Formulário

O sistema envia os dados do formulário para o e-mail:

```
wellington@rbftaxiaereo.com.br
```

Para usar com outro e-mail, altere no JavaScript:

```js
fetch("https://formsubmit.co/ajax/SEU_EMAIL_AQUI", { ... })
```

---

## 📦 Como Usar

1. Clone o projeto ou copie os arquivos para seu servidor/local.
2. Abra `index.html` em um navegador moderno.
3. Clique em uma das aeronaves (MIB, KRT, etc).
4. Preencha o formulário de solicitação de voo.
5. Clique em **Enviar**.
6. Use o botão **VOOS AGENDADOS** para visualizar ou cancelar solicitações.

---

## 📤 Futuras Melhorias (Sugestões)

- Exportação de voos em CSV.
- Validação mais robusta dos dados.
- Login com autenticação.
- Backend para persistência em banco de dados.

---

## 📸 Preview

*Adicione aqui uma captura de tela da interface principal.*