 Capítulo 2 - Noções básicas de Pygame 15

	egg = Wombat()
	egg.bluhbluh()
	whammy.span()

Mesmo que esses nomes tenham sido inventados, você pode saber qual é uma chamada de função, uma chamada de método, e uma chamada de função dentro de um módulo.O nome `whammy` se refere a um módulo, você pode perceber que ele foi importado na primeira linha.O nome `fizzy` não possui nada antes dele, então você sabe que é uma chamada de função.

`Wombat()` também é uma chamada de função, nesse caso é uma função construtora que retorna um objeto. (A letra inicial maiúscula não é uma garantia de que é uma função construtora).A chamada `egg.bluhbluh()` é uma chamada de método de um objeto, porque `bluhbluh` está ligado com o objeto `egg`.

Entretanto, `whammy.spam()` é uma chamada de função, não uma chamada de método.você pode perceber que não é um método porque o nome `whammy` foi importado como um módulo.

#### Objetos Surface e a janela

objetos Surface são objetos que representam uma imagem 2D retangular.Os pixels do objeto Surface podem ser mudados chamando as funções de desenho do Pygame (decritas posteriormente nesse capítulo) e então mostradas na tela.A borda da janela, a barra de título, e os botões não são parte do display do objeto Surface.

Em particular, o objeto Surface retornado por `pygame.display.set_mode()` é chamado de *display Surface*.Tudo o que for desenhado do objeto Surface será mostrado na janela quando a função `pygame.display.update()` for chamada.O processo de desenhar em um objeto Surface é bem rápido (que apenas existe na memória do computador), o que nada mais é do que desenhar o objeto Surface na tela do computador.A memória do computador é bem rápida para mudar os pixels de um
monitor.

Frequentemente seu programa desenhará muitas coisas diferentes no objeto Surface.Uma vez que você terminou de desenhar tudo no display do objeto Surface para essa iteração do loop do jogo (chamado *frame*, do mesmo jeito que uma imagem pausada de um DVD é chamada), então as mudanças serão desenhadas na tela.O computador pode desenhar *frames* rapidamente.30 frames por segundo (isso é, 30 FPS).Isso é chamado de "frame rate" e será explicado posteriormente nesse capítulo.

Desenhando em objetos Surface serão cobertos nas seções "Funções primitivas de desenho" e "Desenhando imagens" desse capítulo.


