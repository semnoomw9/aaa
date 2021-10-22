# wabot-aq

Simple WhatsApp Bot

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/Nurutomo/wabot-aq)

## FOR TERMUX/UBUNTU/SSH USER

```bash
apt update && apt upgrade
apt install git -y
apt install nodejs -y
apt install ffmpeg -y
apt install imagemagick -y
git clone https://github.com/Nurutomo/wabot-aq
cd wabot-aq
npm install
npm update
```

## INSTALL ON TERMUX WITH UBUNTU

[ INSTALLING UBUNTU ]

```bash
apt update && apt full-upgrade
apt install wget curl git proot-distro
proot-distro install ubuntu
echo "proot-distro login ubuntu" > $PREFIX/bin/ubuntu
ubuntu
```
---------

[ INSTALLING REQUIRED PACKAGES ]

```bash
ubuntu
apt update && apt full-upgrade
apt install wget curl git ffmpeg imagemagick build-essential libcairo2-dev libpango1.0-dev libjpeg-dev libgif-dev librsvg2-dev dbus-x11 ffmpeg2theora ffmpegfs ffmpegthumbnailer ffmpegthumbnailer-dbg ffmpegthumbs libavcodec-dev libavcodec-extra libavcodec-extra58 libavdevice-dev libavdevice58 libavfilter-dev libavfilter-extra libavfilter-extra7 libavformat-dev libavformat58 libavifile-0.7-bin libavifile-0.7-common libavifile-0.7c2 libavresample-dev libavresample4 libavutil-dev libavutil56 libpostproc-dev libpostproc55 graphicsmagick graphicsmagick-dbg graphicsmagick-imagemagick-compat graphicsmagick-libmagick-dev-compat groff imagemagick-6.q16hdri imagemagick-common libchart-gnuplot-perl libgraphics-magick-perl libgraphicsmagick++-q16-12 libgraphicsmagick++1-dev
```

---------

[ INSTALLING NODEJS & WABOT-AQ ]

```bash
ubuntu
curl -fsSL https://deb.nodesource.com/setup_current.x | sudo -E bash -
apt install -y nodejs gcc g++ make
git clone https://github.com/Nurutomo/wabot-aq
cd wabot-aq
npm install
npm update
```

---------

## FOR WINDOWS/VPS/RDP USER

* Download And Install Git [`Click Here`](https://git-scm.com/downloads)
* Download And Install NodeJS [`Click Here`](https://nodejs.org/en/download)
* Download And Install FFmpeg [`Click Here`](https://ffmpeg.org/download.html) (**Don't Forget Add FFmpeg to PATH enviroment variables**)
* Download And Install ImageMagick [`Click Here`](https://imagemagick.org/script/download.php)

```bash
git clone https://github.com/Nurutomo/wabot-aq
cd wabot-aq
npm install
npm update
```

---------

## Run

```bash
node .
```

---------

## Arguments `node . [--options] [<session name>]`

### `--self`

Ativar o Self Mode (ignora outros)

### `--pconly`

Se esse bate-papo não de Bot privado, o bot ignorará

### `--gconly`

Se esse bate-papo não do grupo, Bot vai ignorar

### `--swonly`

Se esse bate-papo não do status, o bot ignorará

### `--prefix <prefixes>`

* `prefixes`são separados por cada personagem
Definir prefixo.

### `--server`

Usado para [heroku](https://heroku.com/) ou digitalizar através do site

### `--db <json-server-url>`

Use db externo em vez de banco de dados local,
Example Server `https://json-server.nurutomo.repl.co/`
Code: `https://repl.it/@Nurutomo/json-server`

`node . --db 'https://json-server.nurutomo.repl.co/'`

O servidor deve ter essa especificação

#### GET

```http
GET /
Accept: application/json
```

#### POST

```http
POST /
Content-Type: application/json

{
 data: {}
}
```

### `--big-qr`

Se o pequeno QR Unicode não suporta

### `--restrict`

Permite plugins restritos (que podem levar seu número a ser **banned** Se usado com muita frequência)

*Administração do grupo`add, kick`

### `--img`

Ativar inspetor de imagem através do terminal
### `--autoread`

Se ativado, todas as mensagens recebidas serão marcadas como lidas

### `--nyimak`

Nenhum bot, basta imprimir mensagens recebidas e adicionar usuários ao banco de dados

### `--test`

**Development** Modo de teste

### `--trace`

```js
conn.logger.level = 'trace'
```

### `--debug`

```js
conn.logger.level = 'debug'
```

---------

<a href="https://api.xteam.xyz"><img src="https://i.ibb.co/7j0vtwz/xlogo.png" width="100" height="100"></a> | [![Nurutomo](https://github.com/Nurutomo.png?size=100)](https://github.com/Nurutomo) | [![Ariffb](https://github.com/ariffb25.png?size=100)](https://github.com/ariffb25) | [![Ftwrr](https://github.com/Ftwrr.png?size=100)](https://github.com/Ftwrr) 
----|----|----|----
[XTEAM](https://api.xteam.xyz/) | [Nurutomo](https://github.com/Nurutomo) | [Ariffb](https://github.com/ariffb25) | [Ftwrr](https://github.com/Ftwrr)
Powered by XTEAM | Author / Creator | Most Active Contributor | 2nd Most Active Contributor


Nota: Este projeto não será mantido após "27 de junho de 2021", isso significa que não há atualização.Sinta-se à vontade para qualquer um para continuar este projeto :)

Best Regards. wabot-aq
