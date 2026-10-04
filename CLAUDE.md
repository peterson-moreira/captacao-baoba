# Sankofa · notas sobre captação com pessoas físicas no Fundo Baobá

Estudo independente de Peterson Moreira sobre como começar a trabalhar a mobilização de recursos com pessoas físicas no Fundo Baobá. Publicado em https://peterson-moreira.github.io/captacao-baoba/ via GitHub Pages (branch `main`, pasta raiz).

Antes de qualquer tarefa, leia também `privado/CONTEXTO.md` e `privado/BACKLOG.md`. A pasta `privado/` fica fora do git e nunca deve ser publicada.

## Para quem é

Equipe do Fundo Baobá e da Uzoma Diversidade, no processo seletivo para Analista de Mobilização de Recursos. A página precisa ser lida em poucos minutos e mostrar como Peterson pensa, com humildade de quem olha de fora.

## Regras de conteúdo

- Não inventar nada. Todo número precisa de fonte pública registrada em `estudo/base-de-conhecimento.md` e na lista de Fontes da página.
- Na página, não usar marcadores de fonte no texto, como [1]. As fontes ficam só na lista do rodapé.
- Nunca usar travessão (o caractere longo). Usar dois pontos, vírgula ou ponto.
- Tom de hipótese: "o que eu testaria", nunca "o que o Baobá está fazendo errado".
- Não usar logo, cores ou identidade visual do Fundo Baobá. Deixar claro que é estudo independente.
- Manter `<meta name="robots" content="noindex, nofollow">`: a página é acessível por link, mas fora das buscas.
- Não expor problemas sensíveis do Baobá em público. Observações delicadas ficam em `privado/`.
- Dados pessoais de doadores nunca entram aqui. Demonstrações usam dados fictícios, sempre rotulados como fictícios.
- Português do Brasil, frases curtas, sem jargão desnecessário.

## Estrutura

- `index.html`: a página publicada. CSS embutido, sem dependências externas.
- `estudo/base-de-conhecimento.md`: fatos, fontes, leituras e hipóteses. É a fonte da verdade do conteúdo.
- `privado/` (fora do git): contexto da candidatura, pontos sensíveis e backlog.
- Páginas novas seguem o mesmo estilo do `index.html` e entram no menu do topo.

## Fluxo de trabalho

1. Atualizar primeiro `estudo/base-de-conhecimento.md` quando entrar fato novo, com fonte.
2. Editar o HTML.
3. Conferir antes do commit:
   - nenhum travessão (caractere Unicode U+2014) nem meia-risca (U+2013) em `*.html` e `estudo/*.md`
   - nenhum marcador de fonte no corpo: `grep -n "\[[0-9]*\]" *.html`
   - links internos do menu apontam para ids existentes
   - abrir o arquivo no navegador e olhar em largura de celular
4. Commit com mensagem clara em português e push na `main`. O GitHub Pages atualiza em um ou dois minutos.
5. Conferir a página no ar antes de avisar que terminou.
