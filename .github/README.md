![](img/header.jpg)

<p align="center">
  <img src="https://shields.io/badge/C-20.1.8-A8B9CC?logo=c&style=flat">
  <img src="https://shields.io/badge/Arch Linux-Tested-1793D1?logo=archlinux&style=flat">
  <img src="https://shields.io/badge/Ubuntu-Tested-E95420?logo=ubuntu&style=flat">
  <img src="https://shields.io/badge/Debian-Untested-A81D33?logo=debian&style=flat">
</p>

<p align="center">
    <a href="#-features">features</a>
  • <a href="#-instalação">instalação</a>
  • <a href="#️-contribuindo">contribuindo</a>
</p>

Drivers para vários dispositivos de plataforma dos notebooks Avell, desenvolvidos para DKMS.

---

## 🌟 Features

- Teclas fn
- Backlight do teclado
- Controle de ventoinhas
- Controle de energia
- Sensores em geral
- Ajustes específicos de hardware no espaço do usuário

## 📌 Módulos inclusos:

- clevo_acpi
- clevo_wmi
- tuxedo_keyboard
- uniwill_wmi
- ite_8291
- ite_8291_lb
- ite_8297
- ite_829x
- tuxedo_io
- tuxedo_compatibility_check
- tuxedo_nb05_keyboard
- tuxedo_nb05_power_profiles
- tuxedo_nb05_ec
- tuxedo_nb05_sensors
- tuxedo_nb04_keyboard
- tuxedo_nb04_wmi_ab
- tuxedo_nb04_wmi_bs
- tuxedo_nb04_sensors
- tuxedo_nb04_power_profiles
- tuxedo_nb04_kbd_backlight
- tuxedo_nb05_kbd_backlight
- tuxedo_nb02_nvidia_power_ctrl
- tuxedo_nb05_fan_control
- tuxi_acpi
- tuxedo_tuxi_fan_control
- stk8321
- gxtp7380

## 📲 Instalação

### Dependências:

Geral:

- make

`make package-deb`:

- devscripts
- debhelper
- dh-dkms

`make package-rpm`:

- rpm

## 📑 Documentação

Todas os requisitos, especificações e funcionalidades do projeto podem ser encotradas do arquivo [DOC.md](https://github.com/avell-labs/drivers/blob/master/.github/DOC.md)

## ❤️ Contribuindo

Este é um projeto aberto, então, sinta-se livre para contribuir. Como?

- abra uma [issue](https://github.com/avell-labs/drivers/issues).
- proponha suas correções, sugestões e abra uma pull request com as alterações. Veja os [contribuidores](https://github.com/avell-labs/drivers/graphs/contributors) para maiores informações e leia nosso [código de contribuição](https://github.com/avell-labs/drivers/blob/master/.github/CONTRIBUTING.md).

## 🛑 Aviso

Este software é distribuído **sem qualquer tipo de garantias**.

Não asseguramos que ele funcionará conforme esperado, nem que será isento de falhas, bugs ou interrupções.
O uso é por **sua conta e risco**, e nenhuma responsabilidade será assumida por **danos, perdas ou mal funcionamento** decorrentes da sua utilização.

Para mais detalhes, consulte a [LICENÇA](https://github.com/avell-labs/drivers/blob/master/.github/LICENSE).

## Sobre o Upstreaming dos drivers

O código, embora funcional, **ainda não está pronto para upstream**.

Se desejar contribuir com esse projeto, siga **cuidadosamente** as diretrizes abaixo para evitar danos a software e hardware:

- Envolva-nos durante todo o processo. Não ganhamos nada se, por exemplo, o `avell-control-center` ou a versão DKMS dos drivers pararem de funcionar. Especialmente ao enviar algo para a LKML, **nos inclua em cópia (cc)**.

- Em geral, não podemos compartilhar documentação técnica, mas responderemos perguntas.

- Código que interage com o EC (Embedded Controller) — que compõe a maior parte dos drivers — pode **danificar permanentemente o dispositivo**. Portanto, deve rodar apenas em dispositivos compatíveis e devidamente testados.

Entre em contato antes de iniciar esse tipo de contribuição.
