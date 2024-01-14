# PlanSea

A C project initialization tool that is customizable using a configuration file.
Using a configuration file stored in `~/.planc/conf` a user can configure how to setup a new project.

## Configuration & Usage

On first use, PlanSea creates all the dependencies it needs to become operational.
Things such as creating the base ~/.plansea directory, configuration, and copying the script into ~/.plansea/bin.
A default generated configuration will look as such:

```
project_name=""
init_git="false"
init_files=()
init_directories=()
init_commands=()
```

You can edit these once the directories and files have been generated. PlanSea also allows addition of rules via the command line.

```
plansea -n project-name
plansea -c "mkdir something here" 
plansea -d new-directory
plansea -f new-file
```

---

Thanks for checking out my project! :D
