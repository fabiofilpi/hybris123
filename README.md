# hybris123
Hybris 123

Pontos de observação:
1) No Hybris 20.11, nessa configuração, o HAC não está preparado para o PT Locale. Então, eu precisei alterar a classe SeleniumHelper, pra iniciar sempre o Google Chrome na língua inglesa. Coloquei as seguintes properties: 		chromeOptions.addArguments("--lang=en-US");		chromeOptions.addArguments("--intl.accept_languages=en-US");
2) Eu criei um e-mail no Gmail para disparar os e-mail's do Trails. Está configurado no local.properties.
3) O .gitignore aqui versionado está ignorando os arquivos data. Para não consumir muito espaço do git. Ou seja, não está igual ao .gitignore do 123.
