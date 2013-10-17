# ansible-private-npm

Use ansible to create your own private npm clone on SmartOS.

This is the simplest possible thing that will work.

## Instructions

1. [Install ansible](http://www.ansibleworks.com/docs/intro_installation.html).

2. Clone this repo:

  > git clone https://github.com/timoxley/ansible-private-npm.git
  > cd ansible-private-npm

3. Edit the file `hosts`, to look something like:

```
[npm]
70.3.112.252 ansible_python_interpreter="/opt/local/bin/python"
```

(Where 70.3.112.252 is the IP address or hostname of your SmartOS
machine.)

5. Run the playbook:

  > ansible-playbook -i hosts site.yml

6. You're done.

## Licence

MIT
