# AGENTS

## GitHub push для этого репозитория

При коммите и пуше на GitHub использовать HTTPS с токеном из `~/.git-credentials`:

```
git push $(cat ~/.git-credentials | grep lexbayart | head -1 | sed 's/lexbayart:[^@]*@/lexbayart:@/')/lexbayart/dna-hero.git master
```

Или просто взять URL из `~/.git-credentials` и подставить в `git push`.

Не использовать `git push` без URL — он таймаутится из-за проблем с gh auth.
Не использовать `gh` CLI — он тоже таймаутится.

Репозиторий: https://github.com/lexbayart/dna-hero
Ветка: master
