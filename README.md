## Danilo Mendes Bomfim

**Desenvolvedor Python · Back-end e IA Generativa**<br>
Estudante de Análise e Desenvolvimento de Sistemas na FIAP · aberto a estágio ou vaga júnior remota

Construo projetos em Python com pipelines de IA, filas de jobs, bancos SQL, integração de LLMs e testes automatizados.
Antes do software, trabalhei quase 2 anos com troubleshooting de hardware, redes e servidores na Kantar IBOPE Media,
e é de lá que vem o hábito de reproduzir a falha e provar a causa antes de mexer no código.

[LinkedIn](https://www.linkedin.com/in/danilo-mendestc/) · [Portfólio](https://sunnar.com.br) · contato@sunnar.com.br

---

### Projetos

#### [Origami](https://github.com/SirDann-sys/origami) · [▶ demo online](https://origami.sunnar.com.br/)

Estúdio local que transforma um texto em série narrada: roteiro, vozes por personagem, trilha, vídeos legendados e capas.
Motor back-end em Python com fila de jobs em SQLite, worker único dono da GPU, etapas incrementais por assinatura sha1
e LLM (Claude) chamado em tarefas isoladas com saída validada por JSON Schema.

<img src="https://raw.githubusercontent.com/SirDann-sys/origami/HEAD/docs/tour.gif" alt="Tour da demonstração do Origami" width="680">

#### [Robô RPA Challenge](https://github.com/SirDann-sys/robo-rpa-challenge) · [▶ última execução](https://sirdann-sys.github.io/robo-rpa-challenge/)

[![Robô](https://github.com/SirDann-sys/robo-rpa-challenge/actions/workflows/robo.yml/badge.svg)](https://github.com/SirDann-sys/robo-rpa-challenge/actions/workflows/robo.yml)

Robô em Python com BotCity que preenche um formulário cujos campos trocam de lugar a cada envio, achando cada campo
pelo rótulo e não pela posição: **100% (70 de 70 campos) em cerca de 3 segundos**. Roda todo dia no GitHub Actions,
com testes antes, e publica o replay da execução no GitHub Pages. Pronto para o BotCity Maestro.

<img src="https://raw.githubusercontent.com/SirDann-sys/robo-rpa-challenge/HEAD/docs/resultado.png" alt="Resultado do robô: 100% de acerto, 70 de 70 campos" width="680">

#### [Lupa do Aluguel](https://github.com/SirDann-sys/lupa-do-aluguel) · [▶ usar agora](https://sirdann-sys.github.io/lupa-do-aluguel/)

[![CI](https://github.com/SirDann-sys/lupa-do-aluguel/actions/workflows/ci.yml/badge.svg)](https://github.com/SirDann-sys/lupa-do-aluguel/actions/workflows/ci.yml)

Aponta cláusulas abusivas em contratos de aluguel, a partir do texto ou do PDF. A IA (Groq, com reserva no Gemini)
só extrai fatos com saída por JSON Schema e precisa citar o trecho que prova cada um; quem aplica a Lei do Inquilinato
são 7 regras em Python puro, testadas sem IA. API em FastAPI, métricas em PostgreSQL (SQLAlchemy + Alembic), Docker
e CI com Postgres real. Em 16 contratos de teste cego, acertou **16 de 16**.

---

### Stack

**Back-end:** Python · FastAPI · SQL · PostgreSQL · SQLite · SQLAlchemy · Pydantic · APIs REST<br>
**IA:** LLMs · Claude API · JSON Schema · RAG · Whisper · ComfyUI<br>
**Automação e qualidade:** RPA (BotCity) · pytest · mypy · GitHub Actions · Docker · Git · Linux
