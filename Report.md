
Основная часть

Подними виртуальную машину Ubuntu Server 22.04 LTS.
![alt text](IMG/UP_UBUNTU.png)

Настройка вашего gitlab-runner

- В репозитории пиров есть зарегистрированный gitlab-runner, что подтверждается запущенными и завершенными конвейерами в репозитории

- Добавил официальный репозиторий GitLab командой:
 > curl -L "https://packages.gitlab.com/install/repositories/runner/gitlab-runner/script.deb.sh" | sudo bash
![alt text](IMG/Добавил_официальный_репозиторий_GitLab.png)



![alt text](IMG/Установка_гитлаб_раннера.png)
- Установка_гитлаб_раннера


![alt text](IMG/Проверка_версии_гитлаб_раннера.png)







> ![alt text](IMG/Запустил_gitlab-runner_и_зарегистрировал_его_для_использования_в_текущем_проекте_(DO6_CICD).png)

*Запустил_gitlab-runner_и_зарегистрировал_его_для_использования_в_текущем_проекте_(DO6_CICD)*




- В репозитории пиров есть дамп виртуальной машины с зарегистрированным gitlab-runner

![alt text](IMG/jobs.png)
![alt text](IMG/pipline.png)




![alt text](IMG/pipeline_1.png)



✅ GitLab Runner зарегистрирован

✅ .gitlab-ci.yml файл добавлен и корректно настроен — структура пайплайна понятна, разбита на build, test и deploy стадии.

✅ Пайплайн успешно запущен и прошёл все стадии — все 4 джоба (build, unit test, lint, deploy) завершились со статусом Passed.

✅ Всё выполняется в репозитории  —  в Students_repo / spectrew / DO6_CICD.ID_356283-1, как и требуется по условию.