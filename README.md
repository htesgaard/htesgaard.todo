# Ansible Role: shell todo list

Ansible role for configuring a mechanism for working on todo lists in the shell.

The mechanism is inspired by the article [Ever wonder what the perfect todo list app is?](https://betterhumans.coach.me/ever-wonder-what-the-perfect-task-management-app-is-22d3de022d79)


## Usage

```$ todo```
starts vim with a daily todo file e.g. "~/Google Drive/work/todos/01_21_2018.txt"

Inside vim entering `gt` will add a new task line:
```

  _ my example task
```

With the cursor on a taskline, entering `gg` will complete the task with a completion timestamp:
```

  x my example task [18:57]
```



## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

## Example Playbook

    - hosts: localhost
      vars:
        path_to_todo_files: "~/Google\\ Drive/work"

See the [Mac Development Ansible Playbook](https://github.com/geerlingguy/mac-dev-playbook) for an example of this role's usage.

## License

MIT / BSD

## Author Information

This role was created in 2018 by [Helge Tesgaard](https://github.com/htesgaard).
