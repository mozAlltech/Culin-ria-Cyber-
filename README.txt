========================================================
CYBER GASTRONOMIA — TEMA BLOGGER PARA FARINHA E FORNO
========================================================

AVISO IMPORTANTE SOBRE O CONTEÚDO
----------------------------------
Um tema XML do Blogger controla apenas o DESIGN e a ESTRUTURA do site.
Ele não pode conter dentro de si 100+ receitas completas — as
publicações (posts) do Blogger vivem separadas, na base de dados da
sua conta, e são criadas uma a uma no painel "Publicações".

Este pacote inclui:
- tema-blogger.xml           -> o tema em si (importar 1 vez)
- paginas/                   -> conteúdo pronto para 5 páginas estáticas
- receitas-exemplo/          -> 2 receitas completas, no formato exato
                                 que deve repetir para as restantes

Para chegar às 100+ receitas, publique novos posts usando o mesmo
formato dos ficheiros em receitas-exemplo/ (classes recipe-box,
chef-tip, etc. já vêm estilizadas pelo tema).


1. COMO INSTALAR O TEMA
----------------------------------
1. Aceda ao Blogger > selecione o blog "Farinha e Forno".
2. Vá a Tema > seta ao lado de "Personalizar" > Editar HTML.
3. Faça uma cópia de segurança do tema atual (Fazer download do tema).
4. Apague todo o conteúdo existente no editor e cole o conteúdo de
   tema-blogger.xml.
5. Clique em Guardar.


2. COMO CONFIGURAR O NOME DO SITE
----------------------------------
O nome do site é lido automaticamente de Definições > Básico > Título
do blog no Blogger (variável data:blog.title no tema). Não precisa de
editar o XML para isto — basta alterar o título nas Definições.


3. COMO ALTERAR O CONTACTO
----------------------------------
O número 863582790 aparece em 2 lugares no tema-blogger.xml:
- procure por "CONFIG: CONTACTO" no ficheiro (footer)
- e também na página paginas/contacto.html (secção contact-info)
Substitua o número diretamente nesses dois pontos.


4. COMO ALTERAR OS LINKS SOCIAIS
----------------------------------
No tema-blogger.xml, procure por "CONFIG: LINKS SOCIAIS". Vai
encontrar 3 links (Facebook, Instagram, YouTube) com href="#".
Substitua cada "#" pelo endereço real do perfil correspondente.
Se não usar alguma rede, apague a respetiva linha <li>.


5. COMO ADICIONAR / EDITAR CATEGORIAS
----------------------------------
As categorias no Blogger correspondem às Etiquetas (labels) dos posts.
- Menu principal e cartões de categoria na homepage: já apontam para
  as 6 categorias do briefing (Bolos e Confeitaria, Pratos Principais,
  Acompanhamentos, Sobremesas, Entradas, Dicas de Cozinha).
- Para adicionar uma nova categoria, edite o menu (<nav class="main-menu">)
  e a grelha de categorias (<div class="category-grid">) no tema,
  duplicando um bloco <a> existente e ajustando o texto do label.
- Certifique-se de usar exatamente o mesmo nome de etiqueta nos posts.


6. COMO CONFIGURAR VÍDEOS
----------------------------------
O tema já tem estilo pronto para vídeo incorporado (classe
.video-wrap), mas não vem com nenhum vídeo por padrão — não foram
inventados IDs de vídeo, conforme pedido no briefing.
Para adicionar um vídeo real a uma receita, dentro do corpo do post
(modo HTML) insira:

  <div class="video-wrap">
    <iframe src="https://www.youtube.com/embed/SEU_ID_REAL_AQUI"
            allowfullscreen="allowfullscreen"></iframe>
  </div>

Substitua SEU_ID_REAL_AQUI pelo ID de um vídeo do YouTube que
realmente exista e ao qual tenha direito de uso.


7. COMO CONFIGURAR O FORMULÁRIO DE CONTACTO
----------------------------------
O Blogger não processa formulários nativamente a partir do XML do
tema, por isso o formulário de contacto (paginas/contacto.html) usa
um serviço externo compatível com sites estáticos: Formspree
(https://formspree.io — tem plano gratuito).

Passos:
1. Crie uma conta gratuita em formspree.io.
2. Crie um novo "Form" e copie o endpoint fornecido
   (algo como https://formspree.io/f/abcd1234).
3. Em paginas/contacto.html, substitua:
     data-endpoint="https://formspree.io/f/SEU_ID_FORMSPREE"
   pelo endpoint real copiado.
4. Publique a página. O botão "Enviar" já está funcional em JS
   (ver <script> no fim do tema-blogger.xml) e mostra mensagens de
   sucesso/erro ao visitante.

Se preferir outro serviço (Getform, Web3Forms, etc.), o processo é
o mesmo: só muda o endpoint.


8. COMO ALTERAR CORES
----------------------------------
No tema-blogger.xml, dentro de <b:skin>, logo no início, existe um
bloco :root com as variáveis de cor:

  --bg-void        (fundo geral do site)
  --neon-purple    (cor de destaque principal)
  --neon-blue      (cor de destaque secundária)
  --neon-green     (cor de destaque terciária, usada em tags/dicas)
  --text-main      (texto principal)
  --text-soft      (texto secundário/cinza)

Altere os valores hexadecimais dessas variáveis para mudar a
paleta em todo o site de uma só vez.


9. COMO CONFIGURAR INTEGRAÇÃO EXTERNA (Analytics, Ads, etc.)
----------------------------------
- Google Analytics: adicione o snippet de medição em
  Definições > Outro > Análise dentro do próprio painel do Blogger
  (não precisa de editar o tema).
- Clever Advertising / outra rede de anúncios: cole o código de
  anúncio fornecido pela rede dentro de um Widget HTML/JavaScript
  adicionado nas secções do tema (ex.: dentro de <b:section
  id="page-body">, junto ao includable "commentsAndAds"), seguindo
  as instruções específicas da rede.
Sempre que adicionar uma integração externa, atualize também a
Política de Privacidade (paginas/privacidade.html) para refletir o
que está realmente em uso — o tema já tem a secção 4 pronta para
essa edição.


10. LAZY LOAD / "CARREGAR MAIS"
----------------------------------
A homepage e páginas de categoria/pesquisa já carregam posts
adicionais via feed JSON nativo do Blogger, sem plugins externos.
Não precisa de nenhuma configuração adicional — funciona assim que
o tema é importado.


11. COMO PUBLICAR AS RESTANTES RECEITAS (para chegar a 100+)
----------------------------------
1. Publicações > Nova publicação > alterne para o modo HTML.
2. Copie a estrutura de um dos ficheiros em receitas-exemplo/
   (recipe-box para dados/ingredientes/passos, chef-tip para dicas).
3. Escreva a receita real e completa (sem Lorem Ipsum, sem dados
   inventados).
4. Adicione a etiqueta da categoria correta.
5. Defina a imagem de destaque com uma foto real do prato — se usar
   um banco de imagens gratuito (ex. Unsplash, Pexels), verifique
   sempre a licença de uso antes de publicar.
6. Publique.


12. SOLUÇÃO DE ERROS COMUNS
----------------------------------
- "Erro ao importar o tema": confirme que copiou o ficheiro
  tema-blogger.xml inteiro, sem cortar o início ou o fim.
- Menu mobile não abre: verifique se nenhum outro widget/script foi
  adicionado por cima do <script> do tema, o que pode interromper a
  execução do JavaScript.
- Formulário de contacto não envia: normalmente é o data-endpoint
  ainda com o valor de exemplo — siga o passo 7 acima.
- Imagens não aparecem nos posts carregados por "Carregar mais":
  confirme que cada post tem uma imagem de destaque definida no
  Blogger.
- Ticker parece "saltar": normal na primeira renderização enquanto o
  JS duplica os itens para o loop contínuo; desaparece após o
  carregamento completo da página.


ESTRUTURA DO PACOTE
----------------------------------
CYBER-GASTRONOMIA-BLOGGER/
├── tema-blogger.xml
├── README.txt
├── paginas/
│   ├── contacto.html
│   ├── sobre-nos.html
│   ├── privacidade.html
│   ├── termos-de-uso.html
│   └── cookies.html
└── receitas-exemplo/
    ├── bolo-de-chocolate-fofo.html
    └── frango-grelhado-ervas-limao.html
