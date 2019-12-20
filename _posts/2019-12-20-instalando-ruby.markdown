---
layout: post
title:  "Instalando o Ruby no Windows"
description: Neste artigo, irei demonstrar como realizar a instalação do Ruby para realizar testes de interface com os frameworks RSpec e Capybara.
date:   2019-12-20 12:42:00 +0530
categories: Ferramentas
---

### Vamos lá!
Para começar, devemos acessar a página de download do [Ruby Installer](https://rubyinstaller.org/downloads/).

Ao acessar o site, é visto que o próprio já recomenda uma versão, no momento em que esse documento está sendo criado, é indicada a versão 2.6.5-1. Pode ser que quando você esteja vendo, outra seja recomendada, o importante é baixar uma versão estável superior ou igual ao que o Capybara exige e uma versão que possua o devkit pois o mesmo já facilita o uso e na instalação de várias bibliotecas que poderão ser utilizadas em seus projetos de automação.

![ruby installer](\images\ruby-installer.png)

Você pode saber qual [versão mínima](https://rubygems.org/gems/capybara) do Ruby que o Capybara necessita para rodar tranquilamente sem falhas.

![version ruby](\images\version-ruby.png)

Após realizar o download do instalador do Ruby indicado na primeira imagem, precisaremos dar um clique duplo para executa-lo. O primeiro passo é aceitar a licença, basta marcar “I accept the License” e clicar em “Next”.

![ruby install passo1](\images\ruby-install-step1.png)

A próxima tela que será exibida será esta:

![ruby install passo2](\images\ruby-install-step2.png)

Neste ponto, não iremos realizar nenhuma alteração. Mas caso você queira alterar o diretório onde o Ruby será instalado, não tem problema, basta indicar no campo selecionado. Caso não queira fazer nenhuma alteração, para irmos ao próximo passo devemos clicar no botão “Install”.

Pronto, após isto será exibida uma nova tela, onde o instalador irá solicitar que você confirme quais componentes você deseja instalar.

É importante deixar todas as opções de checkbox marcadas. Pois a primeira se trata da base de arquivos do Ruby e a segunda se trata do MSYS2, na qual o kit de desenvolvimento ou devkit faz parte.

![ruby install passo3](\images\ruby-install-step3.png)

É interessante verificar a mensagem que é exibida antes de ir para o próximo passo.

Ele está informando que irá instalar o Ruby e o MSYS2, mas pede que após a instalação seja executado o seguinte comando “ridk install” para iniciar o devkit. Agora que já estamos cientes, vamos clicar em “Next” para avançar.

Uma tela como esta deverá ser exibida mostrando o progresso da instalação e após o processo ser finalizado, esta tela deverá ser exibida:

![ruby install passo4](\images\ruby-install-step4.png)

Nela, deverá ser desmarcada a opção “Run ‘ridk install’ to setup MSYS2 and development toolchain.” Pois iremos iniciar o devkit em outro momento.

Agora devemos abrir o console e executar o comando “ruby --version” para nos certificarmos que o Ruby foi instalado corretamente.

![ruby install passo5](\images\ruby-install-step5.png)

Após a execução, caso tenha ocorrido tudo bem, uma mensagem como mostrada acima deverá ser exibida.

Para prosseguir, vamos configurar o devkit. Para isso devemos executar o seguinte comando “ridk install”.

![ruby install passo6](\images\ruby-install-step6.png)

Uma mensagem como a que é exibida na imagem acima deverá ser exibida. Neste momento podemos ver que o console nos dá três opções de instalação e nós vamos utilizar a terceira opção. Então devemos digitar o número “3” e pressionar a tecla “Enter”.

Após a instalação ser concluída, uma mensagem como essa deverá ser exibida pelo console.

![ruby install passo7](\images\ruby-install-step7.png)

Devemos pressionar a tecla “Enter” para finalizar a configuração do devkit e pronto, neste momento já temos o Ruby instalado, parabéns se você chegou até aqui.

[Volte a Home](/#)