# SETUP — PHILLY PROFILE

## 1. Instalação (5 passos)

1. Crie um repositório novo com o nome **exatamente igual ao seu usuário**
   GitHub (ex.: usuário `philly` → repo `philly`). Esse nome especial ativa o
   README no seu perfil.
2. Marque como **Public** e inicialize sem README (vamos enviar o nosso).
3. Clone, copie estes arquivos pra raiz do clone (`README.md` + pasta `assets/`)
   e faça push:

```bash
git clone git@github.com:SEU_USUARIO/SEU_USUARIO.git
cp -r /caminho/para/github-profile/* SEU_USUARIO/
cd SEU_USUARIO && git add . && git commit -m "init: signal online" && git push
```

4. Abra seu perfil — o terminal deve renderizar com animações.
5. Substitua os placeholders (lista abaixo) e commit novamente.

## 2. Placeholders a substituir no README.md

| Placeholder | Onde | Trocar por |
|---|---|---|
| `PHILLY_USERNAME` (4x) | stats + contador de views | seu usuário GitHub real |
| `[01] OPERATION: PROJECT_NAME` | OPERATIONS | nome do projeto |
| `STATUS: ACTIVE` / `IN DEV` | OPERATIONS | ACTIVE / IN DEV / QUEUED |
| `[TECH]` | OPERATIONS e TOOLS | stack real (ex.: Python, JS…) |
| `[one-line description]` | OPERATIONS | descrição curta |
| `[REPO_LINK]` | OPERATIONS | link do repositório |
| `[LANGUAGE]` `[FRAMEWORK]` `[DATABASE]` `[AI_TOOL]` `[OTHER]` | TOOLS | suas ferramentas |
| `[GAME_TITLE]` | OFFLINE_MODE | jogo atual |
| `[REPLACE_EMAIL]` … `[REPLACE_WEBSITE]` | CONNECTION | contatos reais ou apague a linha |

Se ainda não tiver projetos públicos: deixe só a operação `[03] REDACTED`
(ela já conta uma história sozinha).

## 3. Personalização extra

- **Codinomes de operação**: troque `PROJECT_NAME` por codinomes temáticos
  (ex.: `OP-BLACKBOX`, `OP-NIGHTDRIVE`) — mantém o clima sem expor nada.
- **Snake monochrome**: adicione o GitHub Action `Platane/snk` gerando SVG com
  `color_snake=#808080, color_dots=#202020/#ffffff` — 100% monocromático.
- **Mais/menos glitch**: as animações usam SMIL dentro dos SVGs. Os pontos de
  glitch são blocos `<animateTransform>` com `keyTimes` perto de `.8–.95`;
  aumente a frequência editando esses valores, ou remova os blocos para versão
  estática.
- **Trocar o slogan do rodapé**: edite `assets/footer-*.svg` (as duas variantes)
  — mantenha as duas sempre iguais.
- **Paleta**: só 4 cores (#000000 #FFFFFF #808080 #202020). Para variar
  intensidades use `opacity`, nunca novas cores — é isso que segura o visual
  monocromático.
- **Fotos/banner real**: se quiser avatar na hero, insira um
  `<image href="URL">` em tons de cinza dentro do `hero-*.svg`.
