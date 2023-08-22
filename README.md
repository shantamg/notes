# Git

Open a PR `~/.gitconfig`
```
[alias]
  pr = "!f() { xdg-open "$(git config --get remote.origin.url | sed -r 's/.*(\\@|\\/\\/)(.*)(\\:|\\/)([^:\\/]*)\\/([^\\/\\.]*)\\.git/https:\\/\\/\\2\\/\\4\\/\\5/')/pull/new/$(git rev-parse --abbrev-ref HEAD)"; };f"
```
