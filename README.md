# PlanSea

A C project initialization tool that is customizable using a configurable python file.
Using a file stored in `~/.plansea/conf.py` a user can configure how to setup a new project.

## Configuration & Usage

On first use, PlanSea creates all the dependencies it needs to become operational. All you need to do is call `./plansea' and let it do the work!
Things such as creating the base ~/.plansea directory, generating a default configuration file, and copying the script into ~/.plansea/bin.
A default generated configuration is just python code and will look as such:

```
project_name = ""
init_git = False
init_files = []
init_directories = []
init_commands = []
```

You can edit these once the directories and files have been generated. PlanSea also allows addition of rules via the command line.

```
plansea -n project-name
plansea -c "mkdir something here" 
plansea -d new-directory
plansea -f new-file
```

---

Be sure to add this to your $PATH environment variable!
`export PATH="$PATH:$HOME/.plansea/bin"`

---

Thanks for checking out my project! :D
