Diário de Decisões e Conflitos
Conflito 1 — app.js

## Integrantes

- João Roberto
- David Gonçalves

Arquivo/linhas: app.js, na função responsável pela atualização do contador e nos eventos dos botões.

Causa: as branches feature/incremento-rename e feature/tema-ajustavel alteraram simultaneamente a lógica do contador. O Aluno B renomeou setCount para updateCount e alterou o incremento para 2 em 2. O Aluno C também alterou o incremento para 2 em 2.

Alternativas consideradas:

Manter a implementação do Aluno B.

Manter a implementação do Aluno C.

Integrar as alterações das duas branches.

Decisão final: foi mantido o incremento e o decremento de 2 em 2 e a função setCount foi renomeada para updateCount.

Racional: as duas alterações de incremento eram compatíveis e atendiam ao requisito do trabalho. A renomeação para updateCount também foi mantida conforme a tarefa do Aluno B.

Quem resolveu: Aluno A.

Data: 01/10/2026.

Conflito 2 — styles.css

Arquivo/linhas: styles.css, variável --primary dentro de :root.

Causa: as duas branches alteraram a mesma variável CSS. O Aluno B definiu a cor primária como verde e o Aluno C definiu a cor primária como vermelho.

Alternativas consideradas:

Manter a cor verde do Aluno B.

Manter a cor vermelha do Aluno C.

Decisão final: foi mantida a cor verde como cor primária da aplicação.

Racional: a equipe decidiu manter a alteração realizada pelo Aluno B para resolver o conflito e ter uma única definição para --primary.

Quem resolveu: Aluno A.

Data: 01/10/2026.

Conflito 3 — index.html

Arquivo/linhas: index.html, elemento <h1 id="title">.

Causa: as duas branches alteraram o título da aplicação. O Aluno B utilizou o título "Mini App – Equipe B", enquanto o Aluno C utilizou "Mini App – Modo Escuro".

Alternativas consideradas:

Manter somente "Mini App – Equipe B".

Manter somente "Mini App – Modo Escuro".

Utilizar "Mini App – Equipe B" como título inicial e alterar o título dinamicamente quando o tema escuro fosse ativado.

Decisão final: o título inicial foi definido como "Mini App – Equipe B". Quando o tema escuro é ativado, o JavaScript altera o título para "Mini App – Modo Escuro". Ao retornar para o modo claro, o título volta para "Mini App – Equipe B".

Racional: dessa forma, as duas funcionalidades das branches foram aproveitadas: a identificação da Equipe B e a indicação visual do modo escuro.

Quem resolveu: Aluno A.

Data: 01/10/2026.

Hotfix — hotfix/titulo-claro

Arquivo/linhas: app.js, lógica responsável pela atualização do título durante a alternância do tema.

Causa: foi identificado e simulado um problema relacionado ao título ao retornar do modo escuro para o modo claro.

Alternativas consideradas:

Manter os textos dos títulos diretamente dentro da condição.

Criar constantes específicas para os títulos do modo claro e do modo escuro.

Decisão final: foram criadas as constantes LIGHT_TITLE e DARK_TITLE, utilizadas pela lógica de atualização do título.

Racional: centralizar os títulos reduz a possibilidade de inconsistência entre os estados claro e escuro e torna a lógica mais organizada.

Quem resolveu: Aluno B.

Data: 01/10/2026.

Integração final

A branch hotfix/titulo-claro foi integrada diretamente em main.

Posteriormente, main foi mesclada em develop para manter a branch de desenvolvimento sincronizada com a correção.

A release original foi identificada pela tag v1.0.0 e a versão posterior à correção do hotfix pela tag v1.0.1.