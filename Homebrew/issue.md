 

# fatal: not in a git directory
Error: Command failed with exit 128: git
brew doctor 

fix by warning!

```shell
git -C "/usr/local/Homebrew" remote set-url origin https://github.com/Homebrew/brew

rm -rf "/usr/local/Homebrew/Library/Taps/homebrew/homebrew-cask"
brew tap homebrew/cask

rm -rf "/usr/local/Homebrew/Library/Taps/homebrew/homebrew-core"
brew tap homebrew/core
```

# cleanup 
==> Running `brew cleanup tree`...
Disable this behaviour by setting HOMEBREW_NO_INSTALL_CLEANUP.
Hide these hints with HOMEBREW_NO_ENV_HINTS (see `man brew`).