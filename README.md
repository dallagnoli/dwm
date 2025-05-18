# dwm - dynamic window manager 

Esta é a minha **fork pessoal** com os seguintes patches:

<details>
  <summary>Clique para ver a lista de patches</summary>

- actualfullscreen
- alwayscenter
- attachbottom
- cfacts
- cool autostart
- hide vacant tags
- movestack
- noborder
- pertag
- placemouse
- preventfocusshift
- resizepoint
- swallow
- systray

</details>

## Dependências

Para que tudo funcione como esperado, recomendo que instale todos os pacotes a seguir.

> [!NOTE]
> Recomendo manter a pasta do repositório em algum lugar seguro no seu sistema para que futuras modificações sejam possíveis.

<details>
  <summary>Arch Linux</summary>

  Instalar dependências:

  ```sh
  sudo pacman -S --needed base-devel git xorg-server xorg-xinit
  ```

  Se você estiver com alguma dependência faltando, baixe o pacote completo do X.org:

  ```sh
  sudo pacman -S --needed xorg
  ```

</details>

## Instalação

Clone o repositório, compile e instale:

```sh
git clone https://github.com/gabrieldallagnoli/dwm && \
cd dwm-titus && \
sudo make clean install
```

- Para executar, adicione `exec dwm` ao final do seu ~/.xinitrc e inicie o X11 com `startx`.
- Ajuste o `config.h` de acordo com as suas preferências.

> [!TIP]
> - Por padrão, o terminal (Alacritty) é aberto com Super + Enter e o app launcher (Rofi) é aberto com Super + BackSpace.
> - Toda vez que fizer alguma alteração, recompile com `sudo make clean install` e reinicie o dwm para que seja aplicada.
