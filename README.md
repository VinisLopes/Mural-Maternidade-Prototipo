# 👶 Protótipo: Mural da Maternidade (Santa Casa)

Este é um protótipo funcional de um sistema de "Mural do Bebê", desenvolvido como uma prova de conceito para a Maternidade Santa Casa.

O projeto simula a interação completa entre as famílias dos recém-nascidos e a administração do hospital. O objetivo é permitir que as famílias criem um mural digital personalizado com fotos e mensagens, que pode ser aprovado pela equipe do hospital e exibido na TV do quarto.

---

## 🚀 Sobre o Protótipo

O projeto é dividido em três módulos principais que simulam o sistema em produção:

### 1. Projeto 1: Site Estático (`public/index.html`)
A página de apresentação (landing page) do serviço. Descreve como o mural funciona, seus benefícios para a família e para o hospital. É o ponto de entrada para os outros dois módulos.

### 2. Projeto 2: Portal da Família (`public/memorias/clientes/...`)
Uma área "logada" (simulada) para a família. Aqui, os pais ou parentes podem:
* Preencher os dados do bebê (nome, data, peso, etc.).
* Fazer upload de fotos.
* Criar galerias de fotos e vídeos.
* Escrever mensagens de carinho.

### 3. Projeto 3: Painel da Maternidade (`public/admin/` e `public/memorial.html`)
Um painel de controle para a equipe da Santa Casa (enfermagem, administração). Este módulo permite:
* Visualizar todos os murais enviados pelas famílias.
* Ver o status de cada mural (Aprovado, Pendente, Revisar).
* Aprovar o conteúdo.
* Ativar o "Modo TV" (`memorial.html`), que é a tela final que seria exibida na televisão do quarto, mostrando o carrossel de fotos e mensagens aprovadas.

---

## 💻 Tecnologias Utilizadas

Este protótipo foi construído 100% com tecnologias de front-end básicas, sem a necessidade de um back-end complexo:

* **HTML5** (Estrutura semântica)
* **CSS3** (Estilização completa com Variáveis CSS, Flexbox e Grid)
* **JavaScript (Puro/Vanilla)** (Para interatividade, como abas, carrossel, filtros e simulação de upload)

---

## ⚡ Como Executar (Importante!)

Este projeto usa links de navegação relativos (ex: `admin/login.htm` e `../index.html`) para simular a navegação entre as pastas.

**Para que todos os botões funcionem corretamente, você tem duas opções:**

### Opção 1: Teste Local (Recomendado)
Você **não pode** simplesmente clicar duas vezes no arquivo `public/index.html` (abrindo-o com `file:///...`), pois os links entre as diferentes pastas (como `admin` e `memorias`) não funcionarão.

Você deve usar um servidor local. A forma mais fácil é:
1.  Abra a pasta do projeto no **VS Code**.
2.  Instale a extensão **"Live Server"**.
3.  No VS Code, clique com o botão direito no arquivo `public/index.html`.
4.  Selecione **"Open with Live Server"**.
5.  Isso abrirá o projeto no seu navegador (em um endereço como `http://127.0.0.1:5500`) e **todos os links funcionarão!**

### Opção 2: Deploy (Vercel/GitHub Pages)
O projeto está pronto para o deploy.
1.  Suba esta pasta para o seu repositório no GitHub.
2.  Importe o repositório no **Vercel**.
3.  Nas configurações do projeto no Vercel, defina o **Root Directory** (Diretório Raiz) como `public`.
4.  Faça o deploy. O Vercel publicará seu site e todos os links funcionarão.

---

## 🌊 O Fluxo de Demonstração

Para apresentar o protótipo, siga estes passos:

1.  Abra a página principal (`public/index.html`) usando o **Live Server**.
2.  Na seção "Navegação entre os módulos", clique em **"Abrir Portal da Família"**.
3.  Você será levado à tela `login.html` da família. Clique em "Entrar no mural" (a senha é simulada).
4.  Na página do portal, preencha os dados do bebê e adicione algumas fotos e mensagens.
5.  Volte para a página principal (`public/index.html`).
6.  Agora, clique em **"Abrir Painel da Maternidade"**.
7.  Você será levado ao `login.htm` do admin. Clique em "Entrar no painel" (também simulado).
8.  Você verá o painel de administração (`public/admin/index.html`) com a lista de murais.
9.  Clique nos botões "Exibir na TV" ou "Ver mural" para ver o resultado final: a tela da TV (`public/memorial.html`).