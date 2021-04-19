# [AFLdiscord.github.io](https://afldiscord.github.io/)

Sito del server discord [AFL](https://discord.gg/5Zu4DxEg3b) con lo scopo di pubblicare gli annunci principali riguardo alla gestione dello stesso e allo sviluppo del bot.

Creato utilizzando [Jekyll](https://github.com/jekyll/jekyll) con il tema [minima](https://github.com/jekyll/minima).

## Setup e build

Il sito è pensato per essere hostato direttamente su github pages. I file in questa repository permettono di fare la build del sito in locale.

### Istruzioni
Le seguenti istruzioni prese dalla [guida di Jekyll](https://jekyllrb.com/docs/installation/) in particolare per Ubuntu(valide anche per wsl).
- installare ruby (v2.4.0+) e altre requisiti  
 `sudo apt install ruby-full build-essential zlib1g-dev #eventualmente apt-get`
- installazione di jekyll e bundler  
 `sudo gem install jekyll bundler`
- clonare il repository nella cartella desiderata  
 `git clone https://github.com/AFLdiscord/AFLdiscord.github.io`
- installare dipendenze  
 `bundle install`
- per eseguire la build e navigare nel sito localmente  
 `bundle exec jekyll serve`

 ### Aggiungere post
 Nella cartella `_posts` creare un nuovo file nominato `YEAR-MONTH-DAY-title.markdown` inserendo la data di creazione e il titolo. Inserire come header del file i seguenti dati:
 ```
 ---
layout: post
author: nome_autore
title:  "Titolo"
date:   2021-04-16 20:03:48 +0200
categories: nome_categoria oppure [cat1, cat2]
---
```
Il testo del post deve essere scritto in markdown. Si consiglia di attivare la preview del risultato nell'editor che si sta utilizzando (per vscode `CTRL+K V` oppure dalla command palette `CTRL+SHIFT+V` cercare markdown).  
Per osservare il risultato:  
`bundle exec jekyll serve`  
aggiungere `--livereload` per modifiche in tempo reale (potrebbe non funzionare sotto wsl)

## Link utili
- [Linguaggio Ruby](https://www.ruby-lang.org/en/)
- [RubyGems in caso non venisse installato](https://rubygems.org/pages/download)
- [Documentazione Jekyll](https://jekyllrb.com/docs/)
- [Tema minima](https://github.com/jekyll/minima)
- [Github pages](https://pages.github.com/)
