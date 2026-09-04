# Cyber Culinária — Template Blogger XML

## Conteúdo do pacote
- `template-cyber-culinaria.xml` — Template completo pronto a importar no Blogger

## Como instalar

1. Acede ao teu blog no [Blogger](https://www.blogger.com)
2. Vai a **Tema** → **Backup/Restaurar** (ou seta ao lado de Personalizar) → **Restaurar**
3. Faz upload do ficheiro `template-cyber-culinaria.xml`
4. Confirma e guarda

**OU** (método Edit HTML):
1. Tema → Editar HTML
2. Apaga todo o código existente
3. Cola o conteúdo completo do XML
4. Guarda

## Páginas estáticas obrigatórias (criar manualmente)

No painel Blogger → **Páginas** → **Nova página**:

### 1. Sobre Nós (URL: /p/sobre-nos.html)
Título: Sobre Nós

Conteúdo sugerido (real e profissional):

```
<h1>Sobre a Cyber Culinária</h1>
<p>A Cyber Culinária nasceu da paixão pela gastronomia e pelo desejo de partilhar receitas reais, testadas e acessíveis a todos. Acreditamos que cozinhar é uma forma de arte e de conexão — e que a tecnologia pode tornar essa experiência ainda mais inspiradora.</p>

<h2>A nossa missão</h2>
<p>Oferecer uma plataforma completa de culinária e gastronomia com conteúdo de qualidade: listas de ingredientes precisas, tempos de preparação reais, passo a passo detalhado e dicas de chef. Sem textos fictícios, sem imagens de demonstração.</p>

<h2>O que encontras aqui</h2>
<ul>
  <li>Bolos e Confeitaria</li>
  <li>Pratos Principais</li>
  <li>Acompanhamentos</li>
  <li>Sobremesas</li>
  <li>Entradas</li>
  <li>Dicas Técnicas de Cozinha</li>
</ul>

<p>Cada receita é pensada para funcionar na cozinha real. Bem-vindo à Cyber Culinária.</p>
```

### 2. Contactos (URL: /p/contactos.html)
Título: Contactos

```
<h1>Contactos</h1>
<p>Tem dúvidas, sugestões de receitas ou queres colaborar? Entra em contacto connosco.</p>

<p class="phone-highlight">📞 Contacto oficial: <strong>863582790</strong></p>

<form class="contact-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
  <div>
    <label for="nome">Nome</label>
    <input type="text" id="nome" name="nome" required placeholder="O teu nome">
  </div>
  <div>
    <label for="email">Email</label>
    <input type="email" id="email" name="email" required placeholder="email@exemplo.com">
  </div>
  <div>
    <label for="mensagem">Mensagem</label>
    <textarea id="mensagem" name="mensagem" rows="5" required placeholder="Escreve a tua mensagem..."></textarea>
  </div>
  <button type="submit">Enviar mensagem</button>
</form>

<p style="margin-top:20px;color:#94A3B8;font-size:0.9rem;">Resposta habitual em 24-48 horas úteis.</p>
```

> **Nota:** Substitui `YOUR_FORM_ID` por um ID do Formspree (gratuito) ou outro serviço de formulário. Alternativamente podes usar o widget de formulário do Blogger se preferires.

### 3. Política de Privacidade (URL: /p/politica-de-privacidade.html)
Título: Política de Privacidade

```
<h1>Política de Privacidade</h1>
<p>Última atualização: Setembro 2026</p>

<p>A Cyber Culinária respeita a sua privacidade. Esta política descreve como recolhemos, utilizamos e protegemos os dados quando visita o nosso blog de culinária e gastronomia.</p>

<h2>1. Dados que recolhemos</h2>
<ul>
  <li>Dados de navegação (páginas visitadas, tempo de permanência, dispositivo e browser) através de cookies e ferramentas de análise (ex.: Google Analytics, se ativado).</li>
  <li>Dados fornecidos voluntariamente através do formulário de contacto (nome, email e mensagem).</li>
  <li>Comentários publicados no blog (nome e conteúdo do comentário).</li>
</ul>

<h2>2. Finalidade</h2>
<p>Utilizamos os dados para melhorar a experiência de navegação, responder a contactos, moderar comentários e analisar o desempenho do conteúdo gastronómico.</p>

<h2>3. Cookies</h2>
<p>Utilizamos cookies essenciais ao funcionamento do Blogger e, eventualmente, cookies de análise. Pode gerir as preferências de cookies no seu browser.</p>

<h2>4. Partilha de dados</h2>
<p>Não vendemos dados pessoais. Podemos partilhar informações com prestadores de serviços necessários ao funcionamento do site (hospedagem Blogger/Google) ou quando exigido por lei.</p>

<h2>5. Direitos do utilizador</h2>
<p>Tem o direito de aceder, retificar ou solicitar a eliminação dos seus dados. Para exercer estes direitos, contacte-nos através do número 863582790 ou do formulário de contacto.</p>

<h2>6. Alterações</h2>
<p>Esta política pode ser atualizada periodicamente. A data de revisão será indicada no topo da página.</p>
```

### 4. Termos de Uso (URL: /p/termos-de-uso.html)
Título: Termos de Uso

```
<h1>Termos de Uso</h1>
<p>Última atualização: Setembro 2026</p>

<p>Ao aceder e utilizar a Cyber Culinária, concorda com os seguintes termos.</p>

<h2>1. Conteúdo</h2>
<p>Todas as receitas, textos, fotografias e materiais publicados são propriedade da Cyber Culinária ou utilizados com autorização. É proibida a reprodução integral sem autorização prévia.</p>

<h2>2. Uso das receitas</h2>
<p>As receitas são partilhadas para uso pessoal e doméstico. Não nos responsabilizamos por resultados obtidos na cozinha de cada utilizador, nem por alergias ou intolerâncias alimentares. Verifique sempre os ingredientes.</p>

<h2>3. Comentários e conduta</h2>
<p>Os utilizadores devem manter um tom respeitoso. Comentários ofensivos, spam ou conteúdo ilegal serão removidos.</p>

<h2>4. Links externos</h2>
<p>O blog pode conter links para vídeos (YouTube/Vimeo) e sites de terceiros. Não controlamos o conteúdo desses sites.</p>

<h2>5. Limitação de responsabilidade</h2>
<p>O conteúdo é fornecido “tal como está”. A Cyber Culinária não garante a ausência de erros e não se responsabiliza por danos decorrentes do uso das informações publicadas.</p>

<h2>6. Contacto</h2>
<p>Para questões relacionadas com estes termos: 863582790.</p>
```

## Categorias (Labels) a criar

No painel → Publicações → Labels (ou ao publicar cada post):

- Bolos e Confeitaria
- Pratos Principais
- Acompanhamentos
- Sobremesas
- Entradas
- Dicas Técnicas

## Estrutura recomendada de cada post/receita

```
[Imagem de capa real]

**Tempo de preparação:** XX minutos  
**Porções:** X  
**Dificuldade:** Fácil / Médio / Avançado

### Ingredientes
- item 1
- item 2
...

### Preparação (passo a passo)
1. ...
2. ...

### Dicas do Chef
...

[Opcional: iframe de vídeo YouTube]
<iframe width="560" height="315" src="https://www.youtube.com/embed/VIDEO_ID" ...></iframe>
```

## Funcionalidades incluídas no template

✅ Tema Cyber Dark (#050508 / #0A0B10 + neon roxo/azul/verde)  
✅ Canvas com partículas caindo  
✅ Orbs brilhantes nas margens com animação  
✅ Marquee/ticker superior e inferior  
✅ Grelha responsiva de posts  
✅ Lazy load + Infinite Scroll  
✅ Suporte a rotação de imagens (fade 2s)  
✅ Players de vídeo com moldura cyber  
✅ Menu de navegação completo  
✅ Widget de Categorias  
✅ Design mobile-first  

## Próximos passos após instalação

1. Criar as 4 páginas estáticas acima  
2. Publicar as primeiras receitas com labels corretas  
3. Configurar o formulário de contacto (Formspree ou similar)  
4. Adicionar imagens reais de alta qualidade às receitas  
5. Incorporar vídeos YouTube nas receitas selecionadas  

---
Cyber Culinária — Pronto para produção.
