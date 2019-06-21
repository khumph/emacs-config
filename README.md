This repository houses my emacs configuration files. I pretty much only use Emacs for the terrific [Org mode](https://orgmode.org), so there isn't anything fancy.

Everything you would need to recreate my configuration is here (provided you install the necessary Emacs packages) except for [sensible-defaults.el](https://github.com/hrs/sensible-defaults.el) which needs to be added to your .emacs.d directory along with the files in this repository.

To run on windows, I place the following `.emacs` file in `C:\Users\%USERNAME%\AppData\Roaming` to point to the appropriate files:
```elisp
(setq user-init-file "C:/path/to/init.el")
(setq user-emacs-directory "C:/path/to/.emacs.d/")
(setq default-directory "C:/whatever/you/want/to/start/in")
(setenv "HOME" "D:/my/home/directory")
(load user-init-file)
```