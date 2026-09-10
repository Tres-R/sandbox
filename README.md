# sandbox

Repositório de treino da organização. O código aqui não vale nada — o objetivo é
praticar o fluxo de trabalho num lugar onde errar não custa, antes de aplicá-lo
no projeto real.

## Como treinar

```bash
git clone git@github.com:Tres-R/sandbox.git
cd sandbox
git checkout develop
git pull
git checkout -b feature/seu-teste
```

Altere qualquer coisa — edite este README, crie um arquivo `.txt`, tanto faz.
Commite seguindo o padrão de prefixo e suba a branch:

```bash
git commit -am "docs: adiciona anotacao de teste"
git push -u origin feature/seu-teste
```

Depois, no GitHub: abra o Pull Request com base em `develop`, peça revisão de
outro integrante e finalize com **Squash and merge**.

## O que está configurado neste repositório

- `main` e `develop` protegidas: sem push direto, Pull Request obrigatório
- 1 aprovação de outro integrante antes do merge
- A proteção vale **também para Owners** — ninguém tem atalho
- Merge só por squash; a branch é apagada automaticamente depois
- Conversas do PR precisam estar resolvidas antes do merge

## Prefixos de commit

| Prefixo | Quando usar |
|---|---|
| `feat:` | nova funcionalidade |
| `fix:` | correção de bug |
| `docs:` | documentação |
| `refactor:` | muda estrutura sem alterar comportamento |
| `test:` | testes |
| `chore:` | dependências, configs, manutenção |

## O que esperar

Se você tentar `git push` direto na `develop` ou na `main`, o GitHub vai recusar
com um erro de protected branch. Esse é o comportamento correto — não é
configuração errada.
