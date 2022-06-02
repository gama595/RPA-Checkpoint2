# RPA-Checkpoint2

Um pequeno empresário possui algumas poucas salas de cinema e percebe que as distribuidoras o avisam com apenas duas semanas de antecedência, a estreia de um filme. Desse modo, o empresário tem pouco tempo para disponibilizar cartazes e outras formas de marketing para atrair o público. Visando mitigar esse problema, o empresário procura vocês para desenvolver uma solução que o ajude a descobrir com maior antecedência a data de estreia do filme e até mesmo, melhorar o marketing sobre os filmes. Para isso, vocês sugerem um sistema que:

1. Capture informações (Web Scrapping) dos principais portais, a cerca das datas de lançamento de filmes para os próximos 6 meses;
2. Capture informações (Web Scrapping) dos principais portais, a cerca das datas de lançamento de filmes dos últimos 6 meses (passados);
3. Estas informações (1.) devem ser salvas em uma tabela (SQL), chamada "SixMonthsAfter" em que a primeira coluna se chamará id (que é dado de forma incremental, na ordem de lançamento dos filmes), title (nome do filme), genre (genero do filme. Ação, aventura...), release_date (timestamp da data de lançamento, em segundos) e n_orders (quantidade de vezes em que compraram ingresso para esse filme, começando com 0);
4. Estas informações (2.) devem ser salvas em uma tabela (SQL), chamada "SixMonthsBefore" em que a primeira coluna se chamará id (que é dado de forma incremental, na ordem de lançamento dos filmes), title (nome do filme), genre (genero do filme. Ação, aventura...), release_date (timestamp da data de lançamento, em segundos) e n_orders (verificar a bilheria deste filme);
5. Caso falte apenas 1 mês (30 dias) para o lançamento de um filme, o sistema deve enviar um email para o empresário para alertá-lo da estreia e, em anexo, sugestões de marketing para esse filme (frases de impacto, posters, banners, cartazes...). Sejam criativos!
6. Além disso, um sistema de compras online deve ser criado. Será desenvolvido uma API com endpoint de PUT, em que no corpo da requisição deve ser enviado o nome do filme e o método deve incrementar 1 na coluna n_orders da tabela criada anteriormente. O retorno do método, será a sugestão de 5 filmes do mesmo genero do filme comprado, visto na tabela "SixMonthsBefore", em ordem decrescente de n_orders;
7. Quando a estreia de um filme da tabela "SixMonthsAfter" passar, o filme deve ser removido da tabela e colocado na tabela "SixMonthsBefore".

---

## [Link Documentação](https://docs.google.com/document/d/1mxPQ3ARuFgfofd84u-ZM2fC0WKsg7MUGgVAKtggl9Us/edit)


## Integrantes
André Gomes Monteiro      RM: 89168\
Leonardo Aranha           RM: 86919\
Luara Maria Marino        RM: 89375\
Renato Kenji Yamashiro    RM: 88847
