# bgrc
Improvements or suggestions to your shell experience with extensions useful for sysadmins.

bgrc is a set of improvements and suggestions from the simple defaults in your shell experience; and extensions useful for sysadmins. Improvements are currently available for bash, vim and screen. Investigate and cherry-pick or trying using `deploy_bgrc` to deploy the whole environment.

## Quickstart

To deploy the whole environment:

	git clone --recursive git@github.com:benvaljean/bgrc.git
	cd bgrc
	bin/deploy_bgrc -l

.screenrc and .vimrc deploy is skipped if your own version is already present

## Sysadmin extensions

- `bglvm`  Show PV, VG and LV information
- `bginfo`  Show basic system information - system model and serial, cpu cores and RAM
- [Post-login icons](https://github.com/benvaljean/bgrc/wiki/Post-login%20icons) Show a character before the prompt upon login based on criteria eg. you have screens running

## bgbashrc

`.bgrc`
Improvements to bash and some commonly used programmes

*Features include*

- ssh auto-complete based on ssh known hosts and client config
- Improvements to bash history - longer history, common and dupes ignored and timestamp added
- Default git pager set to vim with ANSI colours interpreted
- Colours used in grep/ls when supported
- Prompt with colours for easier reading and full path
- Page commands on long-output with `page command`
- grep through history with `hg pattern`
- View only column x when you pipe to `prow x`
- Basic git auto-complete
- vim as default git pager with ansi escape sequences interpreted to highlight diffs
- Command shortcuts
- `hds`  A screenful of head

## bgvimrc

`.vimrc`
Improvements to vimrc

*Features include*

- Use `;` instead of `:` for commands - no need to press shift
- Use `qq` instead of `q!` to exit without saving - now exit a file without saving by typing `;qq` instead of `:q!` by default.
- Syntax highlighting with solarized colours
- NERDTree plugin allow you to browse and view files in a tree view
- Show trailing spaces as `~` and tabs as `>--`; to enable `:set list`

## bgscreenrc

`.screenrc`
Improvements to screenrc

- Use Ctrl-L instead of Ctrl-D as the command character to free up Ctrl-D for bash.
- Longer screen scrollback

## deploy_bgrc

`deploy_bgrc`
Deploy all the above to a remote server or locally from a cloned repo.
