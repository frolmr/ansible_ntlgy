# Самоконтроль выполненения задания

1. Где расположен файл с `some_fact` из второго пункта задания?

``` shell
group_vars/all/examp.yml
```

2. Какая команда нужна для запуска вашего `playbook` на окружении `test.yml`?

``` shell
ansible-playbook -i inventory/test.yml site.yml
```

3. Какой командой можно зашифровать файл?

``` shell
ansible-vault encrypt <filename>
```

4. Какой командой можно расшифровать файл?

``` shell
ansible-vault decrypt <filename>
```

5. Можно ли посмотреть содержимое зашифрованного файла без команды расшифровки файла? Если можно, то как?

``` shell
ansible-vault view <filename>
```

6. Как выглядит команда запуска `playbook`, если переменные зашифрованы?

``` shell
ansible-playbook -i inventory/prod.yml site.yml --ask-vault-pass
```

7. Как называется модуль подключения к host на windows?

``` shell
psrp    Run tasks over Microsoft PowerShell Remoting Protocol
winrm   Run tasks over Microsoft's WinRM 
```

8. Приведите полный текст команды для поиска информации в документации ansible для модуля подключений ssh

``` shell
ansible-doc -t connection ssh
```

9. Какой параметр из модуля подключения `ssh` необходим для того, чтобы определить пользователя, под которым необходимо совершать подключение?

``` shell
remote_user
```

