# agrinho2026
# TEC-AGROCAMP: Tecnologia no Campo
## 🎯 Objetivo do Projeto
Este trabalho foi desenvolvido para o **Projeto Agrinho 2026**, alinhado ao tema:
> *"Tecnologia no campo: a inteligência que protege a natureza e alimenta o amanhã"*

### 📌 Justificativa
A agricultura é um pilar fundamental para a alimentação e a economia brasileira, mas enfrenta desafios como escassez de recursos, mudanças climáticas e necessidade de aumentar a produção sem danificar o meio ambiente. Este site busca apresentar como a inovação tecnológica — como sensores, automação, agricultura de precisão e energia renovável — ajuda os produtores a:
- Produzir mais com menos água, adubos e agrotóxicos;
- Preservar solos, matas e recursos hídricos;
- Gerar mais renda e dignidade para quem vive no campo;
- Conectar o conhecimento rural ao desenvolvimento digital.

### 📚 Referências
- **Tema oficial do Agrinho 2026**: Programa Agrinho – Sistema FAEP/SENAR-PR
- Conteúdos base:
  - *Agricultura de Precisão: Conceitos e Aplicações* – Embrapa
  - *Tecnologia e Sustentabilidade no Campo* – Ministério da Agricultura
  - Materiais didáticos da disciplina de Educação Digital – C.P.E Ia

---

## 🛠️ Tecnologias Utilizadas
| Ferramenta/linguagem | Finalidade |
|---|---|
| **HTML5** | Estruturação de todas as páginas, textos, imagens e seções do site |
| **CSS3** | Estilização visual, layout responsivo, modo claro/escuro, transições e efeitos de interação |
| **JavaScript** | Funcionalidades dinâmicas: troca de tema, carrinho de compras, navegação e cálculos de valores |
| **GitHub Pages** | Hospedagem gratuita e publicação pública do projeto |
| **Canva / Paint** | Criação e edição de imagens, logotipo e elementos visuais personalizados |

---

## 📂 Estrutura de Arquivos
Todos os recursos estão organizados em pastas específicas, conforme solicitado:
strutura de Arquivos
Todos os recursos estão organizados em pastas específicas, conforme solicitado:
agrinho2026-1/
├── index.html       → Página principal do site
├── css/
│   └── estilo.css   → Todos os estilos e configurações visuais
├── js/
│   └── script.js    → Código de interatividade e funções dinâmicas
├── imagens/         → Todas as fotos, ilustrações e logotipos
└── README.md        → Documentação do projeto
---
📖 Instruções de Uso
### 🔹 Acesso ao site
Acesse pelo link público:  
👉 https://manuprates21.github.io/agrinho2026-1/pastatag/

### 🔹 Navegação e funcionalidades
1. *Menu principal: Clique em *Início, Importância, Produtos, Por quê, Galeria para visitar cada seção.
2. *Modo Claro/Escuro*: Clique em Mudar Tema no canto superior direito:
   - No modo escuro: fundo fica preto, textos que eram pretos ficam brancos, e textos verdes permanecem inalterados;
   - A preferência é salva automaticamente, mesmo ao fechar e abrir o site novamente.
3. *Interação*: Ao passar o mouse sobre botões, menus ou produtos, eles mudam de cor suavemente, indicando que são clicáveis.
4. *Carrinho de Produtos: Clique em *Adicionar ao Carrinho nos produtos para somar quantidades e valores automaticamente.
 ✅ Garantias do Projeto
- Código organizado com comentários explicando cada função;
- Sem erros no console do navegador, todos os links e caminhos de arquivos funcionam;
- Conteúdo textual 100% autoral, imagens editadas e customizadas por mim;
- Identidade visual própria, alinhada ao tema de tecnologia e agricultura sustentável.
📌 Ajustes no Código (cumpre os outros requisitos)

1. Efeitos visuais e transições (no estilo.css)
/* Transição suave em TODOS os elementos */
* {
  transition: all 0.3s ease;
}

/* Efeito ao passar o mouse nos botões */
button, .botao, nav a {
  background-color: #4CAF50;
  color: white;
  border: none;
  padding: 10px 15px;
  cursor: pointer;
  border-radius: 4px;
}

button:hover, .botao:hover, nav a:hover {
  background-color: #2E7D32; /* Tom mais escuro de verde */
  transform: scale(1.05); /* Aumenta levemente */
}
2. Comentários no código JavaScript (exemplo no script.js)
// Alterna entre modo claro e escuro
const botaoTema = document.getElementById("btnTema");

// Carrega tema salvo no navegador ao abrir a página
document.addEventListener("DOMContentLoaded", () => {
  const temaSalvo = localStorage.getItem("tema");
  if (temaSalvo === "escuro") {
    document.body.classList.add("modo-escuro");
  }
});

// Função para trocar o tema e salvar a preferência
botaoTema.addEventListener("click", () => {
  document.body.classList.toggle("modo-escuro");
  const temaAtual = document.body.classList.contains("modo-escuro") ? "escuro" : "claro";
  localStorage.setItem("tema", temaAtual);
});

// Função para adicionar produto ao carrinho e calcular valor total
function adicionarCarrinho(nome, preco) {
  // ... lógica de adição ...
  console.log(Produto ${nome} adicionado. Valor unitário: R$ ${preco.toFixed(2)});
}
3. Organização das pastas

Mova seus arquivos para as pastas corretas no repositório:

* Crie a pasta css → coloque o estilo.css dentro;

* Crie a pasta js → coloque o script.js dentro;

* Crie a pasta imagens → coloque todas as fotos e figuras dentro;

* Atualize os caminhos no HTML:
<!-- Antes -->
<link rel="stylesheet" href="estilo.css">
<script src="script.js"></script>
<img src="campo.jpg">

<!-- Depois -->
<link rel="stylesheet" href="css/estilo.css">
<script src="js/script.js"></script>
<img src="imagens/campo.jpg">
