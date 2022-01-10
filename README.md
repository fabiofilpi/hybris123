# hybris123
Hybris 123

Pontos de observação:
1) Quando eu fiz, o HAC não estava preparado para o PT Locale. Então, eu precisei alterar a classe SeleniumHelper, pra iniciar sempre o Google Chrome na língua inglesa. Coloquei as seguintes properties: 		chromeOptions.addArguments("--lang=en-US");		chromeOptions.addArguments("--intl.accept_languages=en-US");
2) Eu criei um e-mail no Gmail para disparar os e-mail's do Trails. Está configurado no local.properties.
3) O .gitignore aqui versionado está ignorando os arquivos data. Para não consumir muito espaço do git. Ou seja, não está igual ao .gitignore do 123.
4) Na tarefa "Create a Cronjob Script Using Groovy", eu só consegui resultados usando a query: "SELECT {p.pk}, {p.code}, {q.code} FROM {Concert AS p}, {ArticleApprovalStatus AS q}, {Band AS b} WHERE {p.approvalstatus} = {q.pk}". Com o atributo {p.name} no SELECT, não tive nenhum resultado. Mas os testes passaram normalmente.
5) Outro ponto é que o teste do Selenium no Backoffice não está 100%. Pelo menos no Mac. Então, precisa dar umas corrigidas, às vezes, no percurso do teste do Selenium exclusivamente para Backoffice. Mais precisamente, quando o Selenium vai buscar algum tipo de item no Backoffice (System>Types), ele está digitando o nome do tipo no lugar errado, está digitando na busca do menu lateral esquerdo, ao invés de digitar na caixa de busca de Tipos. E, também, no login o Selenium não está pressionando corretamente o botão login.
6) Para o ultimo exercicio, "Define Default Property Values", eu precisei dar um reload na validation engine (System > Validation > Constraints > Reload validation engine) para todos os testes unitários passarem. Caso os testes estejam sendo recusados para esse último exercício, realize esse reload e tente novamente.
