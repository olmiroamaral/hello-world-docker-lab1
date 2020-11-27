# Hello world docker action

Esta ação imprime "Hello World" ou "Hello" + o nome de uma pessoa a ser cumprimentada no log.

## Inputs

### `who-to-greet`

**Obrigatório** O nome da pessoa a quem cumprimentar. Padrão `"World"`.

## Outputs

### `time`

Horário que cumprimentamos você.

## Exemplo de uso

uses: actions/hello-world-docker-action@v1
with:
  who-to-greet: 'Mona the Octocat'
Commit, tag e push de ação para o GitHub
A partir do seu terminal, faça commit dos arquivos action.yml, entrypoint.sh, Dockerfile e README.md.

Adicionar uma tag da versão para versões da sua ação é considerada uma prática recomendada. Para obter mais informações sobre versões da sua ação, consulte "Sobre ações".

git add action.yml entrypoint.sh Dockerfile README.md
git commit -m "Minha primeira ação está pronta"
git tag -a -m "Versão da minha primeira ação" v1
git push --follow-tags
