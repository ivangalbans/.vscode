# tools

Tool specific configurations for my development environment.

## VSCode

Path: `./vscode`

**Note:** On macOS, ALT = OPTION

```sh
ln -sf ~/dev/ivangalbans/.vscode/vscode/settings.json "/Users/ivan/Library/Application Support/Code/User/settings.json"
ivan@Ivans-MBP User % ln -sf ~/dev/ivangalbans/.vscode/vscode/keybindings.json "/Users/ivan/Library/Application Support/Code/User/keybindings.json"
```


### Theme & Appearance

- **Theme:** Doom Emacs
- **Icon Theme:** vscode-icons
- **Font:** FiraCode Nerd Font
- **Minimalist UI:** Line numbers off, minimap disabled, scrollbars hidden, activity bar hidden, breadcrumbs disabled

### Language Formatters

| Language       | Formatter                           |
| -------------- | ----------------------------------- |
| Clojure        | Calva                               |
| Docker Compose | Red Hat YAML                        |
| GitHub Actions | Red Hat YAML                        |
| HTML           | VSCode HTML Language Features       |
| JavaScript     | VSCode TypeScript Language Features |
| JSON           | Prettier                            |
| JSONC          | VSCode JSON Language Features       |
| Markdown       | Markdown All in One                 |
| SQL            | PostgreSQL (ms-ossdata)             |
| TypeScript     | Prettier                            |
| XML            | Red Hat XML                         |

### Extensions

<details>
<summary>Click to expand full extensions list (54 extensions)</summary>

| Extension                                   | Description            |
| ------------------------------------------- | ---------------------- |
| adpyke.codesnap                             | Code screenshots       |
| alefragnani.bookmarks                       | Bookmarks              |
| alefragnani.project-manager                 | Project Manager        |
| anthropic.claude-code                       | Claude Code            |
| artemsharko.file-progress                   | File Progress          |
| betterthantomorrow.calva                    | Calva (Clojure)        |
| betterthantomorrow.calva-spritz             | Calva Spritz           |
| bodil.file-browser                          | File Browser           |
| bradlc.vscode-tailwindcss                   | Tailwind CSS           |
| djblue.portal                               | Portal (Clojure)       |
| docker.docker                               | Docker                 |
| eamodio.gitlens                             | GitLens                |
| esbenp.prettier-vscode                      | Prettier               |
| github.copilot                              | GitHub Copilot         |
| github.copilot-chat                         | GitHub Copilot Chat    |
| gruntfuggly.todo-tree                       | Todo Tree              |
| haphazarddev.oil-code                       | Oil Code (Dired)       |
| hbenl.vscode-mocha-test-adapter             | Mocha Test Adapter     |
| hbenl.vscode-test-explorer                  | Test Explorer          |
| hoovercj.vscode-settings-cycler             | Settings Cycler        |
| humao.rest-client                           | REST Client            |
| jacobdufault.fuzzy-search                   | Fuzzy Search           |
| jacobpfeifer.pfeifer-hurl                   | Hurl                   |
| janisdd.vscode-edit-csv                     | Edit CSV               |
| jellydn.vscode-hurl-runner                  | Hurl Runner            |
| kahole.magit                                | Edamagit (Git)         |
| kisstkondoros.vscode-gutter-preview         | Gutter Preview         |
| mateuszdrewniak.hurl-runner                 | Hurl Runner            |
| mechatroner.rainbow-csv                     | Rainbow CSV            |
| ms-azuretools.vscode-containers             | Containers             |
| ms-azuretools.vscode-docker                 | Docker                 |
| ms-kubernetes-tools.vscode-kubernetes-tools | Kubernetes             |
| ms-ossdata.vscode-pgsql                     | PostgreSQL             |
| ms-vscode-remote.remote-containers          | Remote Containers      |
| ms-vscode-remote.remote-ssh                 | Remote SSH             |
| ms-vscode-remote.remote-ssh-edit            | Remote SSH Edit        |
| ms-vscode.makefile-tools                    | Makefile Tools         |
| ms-vscode.remote-explorer                   | Remote Explorer        |
| ms-vscode.test-adapter-converter            | Test Adapter Converter |
| ms-vsliveshare.vsliveshare                  | Live Share             |
| openai.chatgpt                              | ChatGPT                |
| oven.bun-vscode                             | Bun                    |
| pascalreitermann93.vscode-yaml-sort         | YAML Sort              |
| quicktype.quicktype                         | Quicktype              |
| redhat.vscode-xml                           | XML                    |
| redhat.vscode-yaml                          | YAML                   |
| stevesevets.doom-emacs-theme                | Doom Emacs Theme       |
| vitaliymaz.vscode-svg-previewer             | SVG Previewer          |
| vscode-icons-team.vscode-icons              | VSCode Icons           |
| vscodevim.vim                               | Vim                    |
| vspacecode.whichkey                         | WhichKey               |
| yzane.markdown-pdf                          | Markdown PDF           |
| yzhang.markdown-all-in-one                  | Markdown All in One    |

</details>

#### Install extensions

```sh
cat extensions-list.txt | xargs -n 1 code --install-extension
```

### Vim Keybindings

Leader key: `<space>`

#### Project

| Command       | Keybinding |
| ------------- | ---------- |
| List projects | `SPC p p`  |

#### Windows

| Command          | Keybinding |
| ---------------- | ---------- |
| Split vertical   | `SPC w v`  |
| Split horizontal | `SPC w s`  |
| Close window     | `SPC w q`  |
| Maximize/restore | `SPC w m`  |
| Increase width   | `SPC w +`  |
| Decrease width   | `SPC w -`  |
| Navigate left    | `SPC w h`  |
| Navigate right   | `SPC w l`  |
| Navigate down    | `SPC w j`  |
| Navigate up      | `SPC w k`  |

#### Buffers

| Command     | Keybinding |
| ----------- | ---------- |
| Kill buffer | `SPC b k`  |
| Kill buffer | `SPC b d`  |

#### Notifications

| Command   | Keybinding |
| --------- | ---------- |
| Clear all | `SPC n q`  |

#### Open

| Command        | Keybinding |
| -------------- | ---------- |
| Terminal       | `SPC o t`  |
| File explorer  | `SPC o p`  |
| REPL (Clojure) | `SPC o r`  |

#### Fold

| Command     | Keybinding |
| ----------- | ---------- |
| Toggle fold | `z a`      |

### Oil Code (Dired)

Vim-style file browser.

| Command    | Keybinding   |
| ---------- | ------------ |
| Open       | `CTRL+x` `d` |
| Close      | `ESC`        |
| Select     | `ENTER`      |
| Parent dir | `-`          |
| Refresh    | `CTRL+l`     |
| Change dir | `ALT+\``     |

### Git (Edamagit)

| Command      | Keybinding  |
| ------------ | ----------- |
| Status       | `SPC g g`   |
| Status       | `SPC g s`   |
| Dispatch     | `SPC g m`   |
| Refresh      | `SPC g r`   |
| Blame file   | `SPC g b`   |
| File log     | `SPC g f l` |
| File diff    | `SPC g f d` |
| File popup   | `SPC g f m` |
| Stage file   | `SPC g S`   |
| Unstage file | `SPC g U`   |

**In Magit buffer:**

| Command     | Keybinding |
| ----------- | ---------- |
| Discard     | `SHIFT+k`  |
| Toggle fold | `TAB`      |

### Settings Cycler

Quick toggles for UI elements.

| Command             | Keybinding |
| ------------------- | ---------- |
| Toggle line numbers | `ALT+l`    |
| Toggle status bar   | `ALT+s`    |
| Toggle activity bar | `ALT+a`    |
| Toggle glyph margin | `ALT+m`    |

### Quick Open Navigation

| Command       | Keybinding |
| ------------- | ---------- |
| Next item     | `CTRL+j`   |
| Previous item | `CTRL+k`   |

### Suggestion Navigation

| Command             | Keybinding |
| ------------------- | ---------- |
| Next suggestion     | `CTRL+j`   |
| Previous suggestion | `CTRL+k`   |

### Clojure (Calva)

#### Paredit

| Command            | Keybinding        |
| ------------------ | ----------------- |
| Wrap around parens | `ALT+(` / `ALT+)` |
| Wrap around square | `ALT+[` / `ALT+]` |
| Wrap around curly  | `ALT+{` / `ALT+}` |
| Wrap around quote  | `ALT+"`           |
| Next/up sexp       | `SHIFT+L`         |
| Prev/up sexp       | `SHIFT+H`         |
| Slurp forward      | `>`               |
| Barf forward       | `<`               |
| Slurp backward     | `ALT+<`           |
| Barf backward      | `ALT+>`           |
| Kill sexp forward  | `ALT+d`           |
| Raise sexp         | `ALT+SHIFT+r`     |
| Drag sexp forward  | `ALT+j`           |
| Drag sexp backward | `ALT+k`           |

#### REPL & Evaluation

| Command                 | Keybinding | Calva Command                       |
| ----------------------- | ---------- | ----------------------------------- |
| Connect REPL            | `, c`      | calva.connect                       |
| Open REPL               | `SPC o r`  | calva.showReplWindow                |
| Eval file               | `, e b`    | calva.loadFile                      |
| Eval top level form     | `, e d`    | calva.evaluateCurrentTopLevelForm   |
| Eval current form       | `, e e`    | calva.evaluateSelection             |
| Eval selection (visual) | `, e r`    | calva.evaluateSelection             |
| Send form to REPL       | `, e E`    | calva.sendCurrentFormToOutputWindow |
| Eval to comment         | `, e c`    | calva.evaluateSelectionAsComment    |
| Tap to Portal           | `, e t`    | calva.tapCurrentTopLevelForm        |
| Pretty print to comment | `, p P`    | calva.evaluateSelectionAsComment    |
| Refresh all namespaces  | `, r r`    | calva.refreshAll                    |

#### Testing

| Command             | Keybinding | Calva Command            |
| ------------------- | ---------- | ------------------------ |
| Run all tests       | `, t p`    | calva.runAllTests        |
| Run namespace tests | `, t n`    | calva.runNamespaceTests  |
| Run current test    | `, t t`    | calva.runTestUnderCursor |

#### Formatting

| Command       | Keybinding  | Calva Command                |
| ------------- | ----------- | ---------------------------- |
| Align form    | `SPC m f a` | calva-fmt.alignCurrentForm   |
| Format form   | `SPC m f f` | calva-fmt.formatCurrentForm  |
| Format buffer | `SPC m f b` | editor.action.formatDocument |

#### Portal

| Command     | Keybinding  |
| ----------- | ----------- |
| Open Portal | `SPC m o p` |

### Hurl

| Command  | Keybinding  |
| -------- | ----------- |
| Run Hurl | `ALT+CMD+r` |

### Other Keybindings

| Command            | Keybinding     |
| ------------------ | -------------- |
| Bookmarks Explorer | `CTRL+SHIFT+b` |
| Test Explorer      | `ALT+t`        |
| Database Explorer  | `CTRL+SHIFT+d` |
