# Terminal

In the spirit of improving my development sandbox, I set out to look for a better terminal experience. I started out with this boring bash terminal in Ubuntu:

![Old Terminal][/images/terminal_old.png]

The end result looks as follows: 

![New Terminal][/images/terminal_new.png]

This terminal provides you with a more flamboyant experince by integrating Tmuxinator with Oh-my-fish

### Tmuxinator

Fist step install Tmuxinator

	`gem install tmuxinator`

Then, depending on your default editor, you will have to specify

	`export EDITOR='vim'`


Create new project with 

	`tmuxinator new [project]`

where `[project]` is the given name to your Tmuxinator project. It could be called `ironman`.  


Start a session with 

`mux [project]`

Look at the sample `~/.tmuxinator/project.yml` file

### Oh-my-fish

To install Oh-my-fish, you need to install Fish shell v2.1.0 or above. First, let's install Fish.Go to http://fishshell.com/ and select your OS. For me, it is Ubuntu, so I downloaded the .tar.gz file. 

```
	tar -xzf fish_2.2.0.orig.tar.gz
	cd fish fish-2.2.0
```
Then, apply the Autotools Build

```
	autoconf
	./configure
	make
	sudo make install
```

If everything worked, you should be able to start you fish shell on your bash shell with `$ fish`, you will see that the shell looks different. To go back to bash, simply type `bash`. 
# License

MIT