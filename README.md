# Домашнее задание к занятию 1 «Введение в Ansible» - Сергей Ситкарёв

## Основная часть

1. Попробуйте запустить playbook на окружении из test.yml, зафиксируйте значение, которое имеет факт some_fact для указанного хоста при выполнении playbook.

![Задание1](https://github.com/SSitkarev/ansible-01/blob/main/img/1.jpg)

2. Найдите файл с переменными (group_vars), в котором задаётся найденное в первом пункте значение, и поменяйте его на all default fact.

![Задание1](https://github.com/SSitkarev/ansible-01/blob/main/img/2.jpg)

3. Воспользуйтесь подготовленным (используется docker) или создайте собственное окружение для проведения дальнейших испытаний.

4. Проведите запуск playbook на окружении из prod.yml. Зафиксируйте полученные значения some_fact для каждого из managed host.

![Задание1](https://github.com/SSitkarev/ansible-01/blob/main/img/4.jpg)

5. Добавьте факты в group_vars каждой из групп хостов так, чтобы для some_fact получились значения: для deb — deb default fact, для el — el default fact.

6. Повторите запуск playbook на окружении prod.yml. Убедитесь, что выдаются корректные значения для всех хостов.

![Задание1](https://github.com/SSitkarev/ansible-01/blob/main/img/6.jpg)

7. При помощи ansible-vault зашифруйте факты в group_vars/deb и group_vars/el с паролем netology.

![Задание1](https://github.com/SSitkarev/ansible-01/blob/main/img/7.jpg)

8. Запустите playbook на окружении prod.yml. При запуске ansible должен запросить у вас пароль. Убедитесь в работоспособности.

![Задание1](https://github.com/SSitkarev/ansible-01/blob/main/img/8.jpg)

9. Посмотрите при помощи ansible-doc список плагинов для подключения. Выберите подходящий для работы на control node.

![Задание1](https://github.com/SSitkarev/ansible-01/blob/main/img/9.jpg)

10. В prod.yml добавьте новую группу хостов с именем local, в ней разместите localhost с необходимым типом подключения.

![Задание1](https://github.com/SSitkarev/ansible-01/blob/main/img/10.jpg)

11. Запустите playbook на окружении prod.yml. При запуске ansible должен запросить у вас пароль. Убедитесь, что факты some_fact для каждого из хостов определены из верных group_vars.

![Задание1](https://github.com/SSitkarev/ansible-01/blob/main/img/11.jpg)

12. Заполните README.md ответами на вопросы. Сделайте git push в ветку master. В ответе отправьте ссылку на ваш открытый репозиторий с изменённым playbook и заполненным README.md.

13. Предоставьте скриншоты результатов запуска команд.

## Необязательная часть

1. При помощи ansible-vault расшифруйте все зашифрованные файлы с переменными.

![Задание2](https://github.com/SSitkarev/ansible-01/blob/main/img/2-1.jpg)

2. Зашифруйте отдельное значение PaSSw0rd для переменной some_fact паролем netology. Добавьте полученное значение в group_vars/all/exmp.yml.

![Задание2](https://github.com/SSitkarev/ansible-01/blob/main/img/2-2.jpg)

3. Запустите playbook, убедитесь, что для нужных хостов применился новый fact.

![Задание2](https://github.com/SSitkarev/ansible-01/blob/main/img/2-3.jpg)
