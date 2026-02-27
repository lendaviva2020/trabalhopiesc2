# Como ter um link para as pessoas responderem ao questionário

Você tem duas opções: **Formspree** (arquivo HTML que já está na pasta) ou **Google Forms** (criar o formulário direto no Google). As duas geram um link; não precisa de aplicativo.

---

## Opção 1 – Formspree (usar o arquivo `questionario-online.html`)

Assim você usa o questionário bonito que está em **questionario-online.html** e gera um link.

### Passo 1 – Criar a “caixa de entrada” das respostas
1. Acesse **https://formspree.io**
2. Clique em **Get started** (ou “Começar”) e crie uma conta gratuita (pode ser com e-mail ou Google).
3. Clique em **+ New form** e dê um nome, por exemplo: **PIESC II Questionário**.
4. Anote o **form ID** que aparece (algo como `xjvqeqek` ou um código longo). A URL do formulário será: `https://formspree.io/f/SEU_ID`.

### Passo 2 – Colocar seu ID no HTML
1. Abra o arquivo **questionario-online.html** no Bloco de notas ou no Cursor.
2. Procure a linha:  
   `action="https://formspree.io/f/YOUR_FORMSPREE_ID"`
3. Troque **YOUR_FORMSPREE_ID** pelo ID que você anotou.  
   Exemplo: se o ID for `abc123xy`, fica:  
   `action="https://formspree.io/f/abc123xy"`
4. Salve o arquivo.

### Passo 3 – Gerar o link (onde as pessoas vão clicar)
Você precisa colocar o arquivo HTML na internet. A forma mais rápida:

- **Netlify Drop (recomendado):**
  1. Acesse **https://app.netlify.com/drop**
  2. Arraste a pasta onde está o **questionario-online.html** (ou só o arquivo) para a área de “drop”.
  3. A Netlify vai gerar um link, tipo: `https://algo-aleatorio-123.netlify.app/questionario-online.html`
  4. Esse é o link que você envia por WhatsApp, e-mail ou coloca em rede social. Quem clicar abre o questionário, marca as opções, preenche o que quiser e clica em **Enviar**.

- **Alternativa – GitHub Pages:**  
  Se você já usa GitHub, pode subir o arquivo em um repositório e ativar GitHub Pages; o link será algo como `https://seuusuario.github.io/nome-repo/questionario-online.html`.

### Onde ver as respostas
- No **Formspree**, em **https://formspree.io**, abra seu formulário. As respostas chegam lá (e, se você configurou, por e-mail). Você pode exportar em planilha para usar no relatório.

---

## Opção 2 – Google Forms (link em 5 minutos)

Se preferir não mexer em HTML e já tiver conta Google:

1. Acesse **https://forms.google.com**
2. Clique em **+ Em branco** (formulário em branco).
3. Use as mesmas perguntas do **questionario-base-PIESC-II.md**:
   - Para “Sim / Não / Não tenho certeza” → questão de **múltipla escolha** com essas 3 opções.
   - Para “O que você costuma fazer com pilhas...” → múltipla escolha com as opções listadas no questionário-base.
   - Repita para todas as perguntas (múltipla escolha ou texto curto).
4. No topo, clique em **Enviar** (ícone de avião) → **Link** → copie o link.
5. Esse link você envia para as pessoas. Elas abrem, marcam as opções, preenchem e clicam em enviar. As respostas vão direto para uma planilha no Google Sheets (aba “Respostas” ou planilha vinculada).

---

## Sobre as fotos em campo

O questionário em link **não precisa** tirar foto da pessoa. Você pode:

- **Tirar fotos em campo** com a pessoa (com autorização) só para **registro do projeto** (ex.: “aplicação do questionário em evento X”). Essas fotos você guarda na pasta **05-anexos** e usa no relatório final como evidência de que aplicou o questionário.
- O **link** serve para a pessoa responder sozinha no celular ou no computador, quando e onde quiser. Se você estiver ao lado, pode mostrar o link no seu celular, a pessoa abre, responde e já envia; aí você tira a foto dela (com permissão) como registro de que aplicou em campo.

Resumo: **link = responder o questionário.** **Fotos em campo = você tira com a pessoa para anexar no relatório e mostrar onde aplicou.**

---

## Resumo rápido

| O que você quer | O que fazer |
|-----------------|-------------|
| Link para as pessoas responderem | Opção 1: Formspree + Netlify Drop com o `questionario-online.html` **ou** Opção 2: criar o formulário no Google Forms e copiar o link. |
| Ver/guardar respostas | Formspree: no site ou por e-mail. Google Forms: na aba Respostas ou na planilha do Sheets. |
| Fotos com a pessoa em campo | Tirar com o celular (com autorização) e salvar em **05-anexos** para o relatório. Não é obrigatório no formulário online. |

Se quiser, na próxima etapa podemos só ajustar o texto das perguntas no HTML para ficar exatamente igual ao modelo da sua professora.
