# Documentação do Projeto

**As teclas de controle da luz de fundo do teclado e/ou do touchpad não funcionam**

Para todos os dispositivos com teclas (ou combinações) de ativação/desativação do touchpad, e alguns com controle da luz de fundo do teclado, o driver apenas envia o evento de tecla correspondente para o espaço de usuário. É responsabilidade do DE executar a ação associada. Alguns ambientes menores não vinculam ações a essas teclas por padrão, o que faz parecer que não funcionam.

Consulte a documentação do seu DE para criar atalhos personalizados.

Para controlar o brilho do teclado, utilize a interface D-Bus do UPower como destino das ações de tecla.

Para alternar o touchpad no X11, use `xinput` para ativar/desativar. No Wayland, a forma correta depende do DE utilizado.
