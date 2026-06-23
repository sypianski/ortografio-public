# Ortografio — publikaj vortaroj por Neovim

Kolekto de `.utf-8.add` dosieroj por la Vim/Neovim literumo-kontrolilo (`spellfile`).
Ĉiu dosiero enhavas po unu vorto en linio. Oni aldonas vortojn per `zg` en normala reĝimo.

## Vortaroj

| Dosiero | Enhavo |
|---------|--------|
| `tech.utf-8.add` | Teknologiaj terminoj — Docker, API, JSON, nginx, regex, k.a. |
| `ai.utf-8.add` | Artefarita inteligenteco kaj maŝinlernado — LLM, RAG, LoRA, transformer, k.a. |
| `medieval.utf-8.add` | Mezepoka kaj bizanca terminaro — codicologie, basileus, miaphysite, k.a. |
| `arabic-translit.utf-8.add` | Araba transliteraĵo laŭ scienca normo (Ibn, Ḥunayn, Kitāb, k.a.) |

## Uzo

```lua
-- En via Neovim-agordo:
vim.opt.spellfile = {
  vim.fn.expand("~/ortografio/public/tech.utf-8.add"),
  vim.fn.expand("~/ortografio/public/ai.utf-8.add"),
}
```

Aŭ per la komando `:mkspell` por kompili `.spl` dosieron:

```
:mkspell ~/.config/nvim/spell/tech.utf-8 ~/ortografio/public/tech.utf-8.add
```

## Licenco

CC0 — publika domeno.
