# zsh-functions

This is a repository of some zsh custom function that helped me with
development on my local Mac OSX machine

## Installation

1. Clone the repository somewhere. 
2. Symlink the `zfunc` dir to your user's home dir as `.zfunc`
3. Add the following to your `.zshrc` file
  
        fpath=(
            .zfunc/
            .zfunc/**/*~*/(CVS)#(/N)
            "${fpath[@]}"
        )

4. Mark the function you need to be autoloaded when needed in `.zshrc`
   
    eg.: `autoload -Uz php`
