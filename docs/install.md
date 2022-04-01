# Installation

If you have previously scanned QR code and already have `session.json` or `session.data.json` file, it is strongly recommended to rename 'session.json' to 'session.data.json' and copy it into Valor Bot folder/repository.

## Before you start: (necessary)

- Edit owner number `'919971107409'` and replace with own number in `config.js` file
```
global.owner = [
  ['919971107409', 'Dinesh_Valor🇮🇳', true]
```
- Edit X-Team API key `'493053acc612476f'` and replace with own [X-Team](https://api.xteam.xyz/register) API key in `config.js` file
```
global.APIKeys = { // APIKey Here
  // 'https://website': 'apikey'
  'https://api.xteam.xyz': '493053acc612476f',
```
> (You can also edit and make changes, such as  package name, author name, etc in `config.js` file)

## **There are three ways to install:**
- Heroku (Server)
- Termux (Android 7 or higher)
- CMD (Windows 7 or higher)

## Heroku (Server)

This allows for easier installation and Heroku is a server based, that's mean bot keep active for 24×7 without your device up for all time.

[![Heroku Tutorial Video](https://img.shields.io/badge/Heroku-Tutorial_Video_(upload_soon)-red?logo=heroku)]()

**Required Buildpack:**
- Nodejs
- https://github.com/jonathanong/heroku-buildpack-ffmpeg-latest
- https://github.com/DuckyTeam/heroku-buildpack-imagemagick

**To Install:**

1. Create an account on [GitHub](https://github.com/signup) [skip if already an account]
2. [Fork](https://github.com/DineshValor/valor/fork) “Valor Bot” repository
3. Create account on [Heroku](https://signup.heroku.com/) [skip if already an account]
4. Create [new app](https://dashboard.heroku.com/new-app)
5. Enter `app name`, choose a region and create app
6. Go to app `Settings`, click on `Add buildpack` and copy/paste all three mentioned above `requried buildpack` one by one and `Save changes` respectively
7. Go to app `Deploy`, `Connect to GitHub`, click on `Search`, connect to `.../valor` repository, `Enable Automatic Deploys` and click on `Deploy Branch`
8. Go to app `Resources`, turn ON `worker node .` under `Free Dynos`
9. Click on `More` (top right corner) and click on `View logs`
10. Scan QR code via WhatsApp > Linked devices _[skip if you already copied `session.data.json` file into repository]_
> (Step 10 is necessary to activate bot on your whatsapp, and currently bot only support Multi-device beta)
11. Hurray! Bot successfully installed and ready to use. Type `.menu` or `.help` in whatsapp chat to access bot menu
> ⚠️ If any error comes, feel free raise an [Issue](https://github.com/DineshValor/valor/issues)
## Termux (Android 7 or higher)

Termux is a local hardware based terminal, that's mean it use device hardware to run bot and for that requires Termux app always active with good internet connection

[![Termux Tutorial Video](https://img.shields.io/badge/Termux-Tutorial_Video_(upload_soon)-red?logo=powershell)]()

**To Install:**

1. Download and install [Termux app](https://github.com/termux/termux-app/releases/download/v0.118.0/termux-app_v0.118.0+github-debug_universal.apk)
2. Open Termux app and type given below commands one by one in terminal
```
$ pkg upgrade -y
$ pkg install git -y
$ pkg install yarn -y
$ pkg install nodejs -y
$ pkg install ffmpeg -y
$ pkg install imagemagick -y
$ git clone https://github.com/DineshValor/valor
$ cd valor
$ yarn
$ node .
```
3. Scan QR code via WhatsApp > Linked devices _[skip if you already copied `session.data.json` file into repository]_
4. Hurray! Bot successfully installed and ready to use. Type `.menu` or `.help` in whatsapp chat to access bot menu
>⚠️ If any error comes, feel free raise an [Issue](https://github.com/DineshValor/valor/issues)

## CMD (Windows 7 or higher)

CMD is a windows based local command prompt/terminal, which runs bot locally inside pc using it's hardware

[![CMD Tutorial Video](https://img.shields.io/badge/CMD-Tutorial_Video_(upload_soon)-red?logo=powershell)]()

**Required Packages:**

- Download and Install [Git](https://git-scm.com/downloads)
- Download And Install [NodeJS](https://nodejs.org/en/download/)
- Download And Install [FFmpeg](https://ffmpeg.org/download.html)
> (Don't Forget Add FFmpeg to PATH enviroment variables)
- Download And Install [ImageMagick](https://imagemagick.org/script/download.php)

**To Install:**

1. Open CMD (command prompt) and type given below commands one by one in command prompt/terminal
```
git clone https://github.com/DineshValor/valor
cd valor
npm install
npm update
node .
```
2. Hurray! Bot successfully installed and ready to use. Type `.menu` or `.help` in whatsapp chat to access bot menu
> ⚠️ If any error comes, feel free raise an [Issue](https://github.com/DineshValor/valor/issues)
