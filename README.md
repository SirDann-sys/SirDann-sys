<p align="center">
  <img src="./assets/sunnar-banner.svg" alt="sunnar terminal banner" width="680" />
</p>

<p align="center">
  <a href="https://sunnar.com.br"><img src="https://img.shields.io/badge/sunnar.com.br-00F3FF?style=for-the-badge&logoColor=0A0C10&labelColor=0A0C10" alt="sunnar.com.br" /></a>
  <a href="https://www.linkedin.com/in/danilo-mendestc/"><img src="https://img.shields.io/badge/LinkedIn-00F3FF?style=for-the-badge&labelColor=0A0C10" alt="LinkedIn" /></a>
</p>
<p align="center"><sub>portfólio ao vivo &middot; código de cada projeto abaixo</sub></p>

<br>

## `sunnar@root:~$ whoami`

<p align="center">
  <img src="./assets/sunnar-neofetch.svg" alt="edu: análise e desenvolvimento de sistemas · fiap (em curso). edu_prev: técnico em eletrônica · ifg (concluído). work_prev: técnico eletrônico jr · kantar, bancada e servidores. lang: python, java, c, dart. infra: linux, docker, git, redes. status: aberto a estágio em desenvolvimento." width="680" />
</p>

Vim do hardware. Técnico em eletrônica pelo IFG, depois quase dois anos de bancada na Kantar IBOPE Media diagnosticando equipamento de medição de audiência, dispositivos de rede e servidores de recepção — sob SLA, às vezes em sobreaviso.

Bancada não é coisa que eu deixei para trás. É onde aprendi a trabalhar: isolar a variável, reproduzir a falha, provar a causa antes de trocar a peça. Hoje curso Análise e Desenvolvimento de Sistemas na FIAP e aplico a mesma disciplina em código — este domínio é a minha bancada de testes. O que sobrevive ao teste vira projeto no vault abaixo; o resto fica como aprendizado.

> "Depurar uma placa é a mesma disciplina que depurar um sistema: isolar a variável, reproduzir a falha, provar a causa antes de trocar a peça. Mudou o substrato, não o raciocínio."

<br>

## `sunnar@root:~$ ls ./the_vault`

Todo projeto aqui tem código visível e roda de verdade. Vitrine completa, com prints e detalhes técnicos de cada um, em **[sunnar.com.br/#vault](https://sunnar.com.br/#vault)**.

### [TrapDoor](https://github.com/SirDann-sys/trapdoor)

<p align="center">
  <img src="./assets/projects/trapdoor-v1.webp" alt="TrapDoor analisando um contrato de aluguel: cláusulas abusivas destacadas com a regra e o artigo violado" width="680" />
</p>

Cola um contrato de aluguel, recebe as cláusulas que violam a Lei do Inquilinato — artigo por artigo.

> **A parte difícil:** `rules.py` é fonte única — o mesmo texto alimenta o prompt do modelo *e* o gabarito dos testes, então não podem divergir. `validar.py` roda os contratos sintéticos de teste (limpos, para checar falso positivo; violação explícita; violação disfarçada; e um caso de regressão com duas violações na mesma cláusula) contra o gabarito esperado, com exit code 0/1 — **9/9 passando**. Saída do modelo forçada por schema, sem parse de markdown.

![Python](https://img.shields.io/badge/Python-0A0C10?style=flat-square&logo=python&logoColor=00F3FF)
![Anthropic API](https://img.shields.io/badge/Anthropic_API-0A0C10?style=flat-square)
![Streamlit](https://img.shields.io/badge/Streamlit-0A0C10?style=flat-square&logo=streamlit&logoColor=00F3FF)

### [Kitsune Badge](https://github.com/SirDann-sys/kitsune-badge)

<p align="center">
  <img src="./assets/projects/kitsune-badge-v1.webp" alt="As três telas do Kitsune Badge: QR code de acesso, relógio com clima e temporizador pomodoro" width="680" />
</p>

Crachá físico em ESP32: QR code de acesso, relógio com clima e pomodoro, numa tela de 2.8".

> **A parte difícil:** a raposa é um sprite 4bpp de 128×118 empacotado em nibbles no PROGMEM e desenhada linha a linha num buffer de 256 bytes — o ESP32 não comporta o bitmap inteiro em RAM. O QR é gerado em runtime, sem bitmap pré-renderizado. Display em HSPI e touch em VSPI, configurados via build flags do PlatformIO para não tocar no `User_Setup.h` do TFT_eSPI.

![ESP32](https://img.shields.io/badge/ESP32-0A0C10?style=flat-square)
![C++](https://img.shields.io/badge/C%2B%2B-0A0C10?style=flat-square&logo=cplusplus&logoColor=00F3FF)
![PlatformIO](https://img.shields.io/badge/PlatformIO-0A0C10?style=flat-square)

### [Sunnar Terminal](https://github.com/SirDann-sys/sunnar-terminal-web)

<p align="center">
  <img src="./assets/projects/sunnar-terminal-v1.webp" alt="Tela inicial do Sunnar Terminal: o nome SUNNAR em destaque sobre o terminal de navegação" width="680" />
</p>

Este site. SPA em HTML, CSS e JavaScript puro — sem framework, sem build step.

> **A parte difícil:** roteamento por hash próprio, com renderização lazy e idempotente por view, navegação completa por teclado e suporte a `prefers-reduced-motion`. Hardening de produção versionado no repositório: `Content-Security-Policy` sem `unsafe-inline`, HSTS, `X-Frame-Options` e `Permissions-Policy`. Deploy contínuo no Cloudflare Pages, DNS próprio.

![JavaScript](https://img.shields.io/badge/JavaScript-0A0C10?style=flat-square&logo=javascript&logoColor=00F3FF)
![CSS](https://img.shields.io/badge/CSS-0A0C10?style=flat-square&logo=css&logoColor=00F3FF)
![Cloudflare Pages](https://img.shields.io/badge/Cloudflare_Pages-0A0C10?style=flat-square&logo=cloudflare&logoColor=00F3FF)

<br>

## `sunnar@root:~$ cat stack.list`

![Python](https://img.shields.io/badge/Python-0A0C10?style=flat-square&logo=python&logoColor=00F3FF)
![Java](https://img.shields.io/badge/Java-0A0C10?style=flat-square&logo=openjdk&logoColor=00F3FF)
![C](https://img.shields.io/badge/C-0A0C10?style=flat-square)
![Dart](https://img.shields.io/badge/Dart-0A0C10?style=flat-square&logo=dart&logoColor=00F3FF)
![Flutter](https://img.shields.io/badge/Flutter-0A0C10?style=flat-square&logo=flutter&logoColor=00F3FF)
![JavaScript](https://img.shields.io/badge/JavaScript-0A0C10?style=flat-square&logo=javascript&logoColor=00F3FF)
![HTML5](https://img.shields.io/badge/HTML5-0A0C10?style=flat-square&logo=html5&logoColor=00F3FF)
![CSS3](https://img.shields.io/badge/CSS3-0A0C10?style=flat-square&logo=css&logoColor=00F3FF)
![Git](https://img.shields.io/badge/Git-0A0C10?style=flat-square&logo=git&logoColor=00F3FF)
![Linux](https://img.shields.io/badge/Linux-0A0C10?style=flat-square&logo=linux&logoColor=00F3FF)
![Docker](https://img.shields.io/badge/Docker-0A0C10?style=flat-square&logo=docker&logoColor=00F3FF)
![Arduino](https://img.shields.io/badge/Arduino-0A0C10?style=flat-square&logo=arduino&logoColor=00F3FF)

<br>

## `sunnar@root:~$ cat contato.txt`

<p align="center">
  aberto a oportunidades de estágio em desenvolvimento<br>
  <a href="https://www.linkedin.com/in/danilo-mendestc/">linkedin.com/in/danilo-mendestc</a>&nbsp;&nbsp;&middot;&nbsp;&nbsp;<a href="mailto:contato@sunnar.com.br">contato@sunnar.com.br</a>&nbsp;&nbsp;&middot;&nbsp;&nbsp;<a href="mailto:danilomb2003@gmail.com">danilomb2003@gmail.com</a>&nbsp;&nbsp;&middot;&nbsp;&nbsp;<a href="https://sunnar.com.br">sunnar.com.br</a>
</p>
