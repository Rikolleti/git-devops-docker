## Задача 1
https://hub.docker.com/repository/docker/azhdarmamedov/custom-nginx/general

## Задача 2
1. ![Run Image](images/task2_docker_run.png)

2. ![Rename Image](images/task2_docker_rename.png)

3. ![Final command](images/task2_final_command.png)

4. ![Output screenshot](images/task2_output.png)

## Задача 3
1. ![Docker attach](images/task3_attach.png)
2-3. Так произошло, потому что у каждого контейнера есть свой процесс и командой Ctrl + C мы посылаем сигнал SIGINT для его завершения
![Docker_Ctrl+c] (images/images/task3_docker_run.png)
5-6. ![Docker IT and nano install](images/task3_docker_install_nano.png)
7. Отредактировал
8. ![Docker reload nginx](images/task3_change_ports.png)
10. Nginx теперь слушаем порт 81, а ранее я пробрасывал порт 8080 ВМ на 80 docker, это можно видеть в docker ps:
973a99bb5b36   azhdarmamedov/custom-nginx:1.0.0   "/docker-entrypoint.…"   10 minutes ago   Up 10 minutes   0.0.0.0:8080->80/tcp, [::]:8080->80/tcp   pensive_darwi
11. Можно сделать новый коммит на основе коммита текущего контейнера (docker commit) и запустить этот новый контейнер с новым пробросом портов (8081:81)
12. rikolleti@compute-vm-2-2-30-hdd-1751355561681:~$ docker rm -f confident_agnesi
confident_agnes

## Задача 4
1. ![Docker Centos](images/task4_centos.png)
2. ![Docker Debian](images/task4_debian.png)
3. ![Docker Centos create file](task4_centos_create_file.png)
4. ![Host Create second file](images/task4_create_second_file.png)
5. ![Docker Debian list files](images/task4_list_files_debian.png)

## Задача 5
1. Был использован файл compose.yaml, так как он является более предпочтительным, так как файл docker-compose.yaml используется для обратной совместимости с более ранними версиями.
![Docker Compose Up](images/task5_docker_compose_up.png)
2. ![Docker Compose Both Files](images/task5_docker_compose_both_files.png)
3. ![Docker Compose Local Registry](images/task5_docker_compose_local_registry.png)
4. ![Docker Portainer](images/task5_portainer.png)