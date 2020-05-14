This repository houses my emacs configuration files. I pretty much only use Emacs for the terrific [Org mode](https://orgmode.org), so there isn't anything fancy.

Everything you would need to recreate my configuration is here (provided you install the necessary Emacs packages) except for [sensible-defaults.el](https://github.com/hrs/sensible-defaults.el) and [org-checklist.el](https://github.com/yyr/org-mode/blob/master/contrib/lisp/org-checklist.el) which need to be added to your .emacs.d directory along with the files in this repository.

To run on Microsoft Windows, I place the following `.emacs` file in `C:\Users\%USERNAME%\AppData\Roaming` to point to the appropriate files:
```elisp
(setenv "HOME" (substitute-in-file-name "$USERPROFILE"))
(setq user-init-file (substitute-in-file-name "$HOME/.emacs.d/init.el"))
(setq user-emacs-directory (substitute-in-file-name "$HOME/.emacs.d"))
(setq default-directory (substitute-in-file-name "$HOME")) ; Directory to start in
(load user-init-file)
```
