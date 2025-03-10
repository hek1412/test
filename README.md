### Git push

![image.png](Git+в+юпитере+8995d786-6f79-41d6-abc2-9ddf4673a681/image.png)

Заходим в терминал и выполняем команды:

Информация о версии
```
git --version
```
Смотрим что в текущей директории
```
ls -la
```
Понимаем, что нам это не нужно и переходим в рабочую директорию ноутбука юпитера, где хранятся наши файлы
```
cd /home/jovyan/work/
```
![image.png](Git+в+юпитере+8995d786-6f79-41d6-abc2-9ddf4673a681/image1.png)
```
git init

git add .
```
Если первый раз, то может потребовать внести учетные данные
```
git config --global user.email "[hek1412@gmail.com](mailto:hek1412@gmail.com)"

git config --global user.name "hek1412"
```
![image.png](Git+в+юпитере+8995d786-6f79-41d6-abc2-9ddf4673a681/image2.png)



Делаем коммит
```
git commit -m "test"
```

![image.png](Git+в+юпитере+8995d786-6f79-41d6-abc2-9ddf4673a681/image3.png)

Создаем новый репозиторий в организации 1Т45, я создал testjupyter

![image.png](Git+в+юпитере+8995d786-6f79-41d6-abc2-9ddf4673a681/image4.png)

[https://github.com/1T45git/testjupyter](https://github.com/1T45git/testjupyter)

Копируем ссылку на репозиторий

[https://github.com/1T45git/testjupyter.git](https://github.com/1T45git/testjupyter.git)



Далее вводим команды в терминале
```
git remote add origin https://github.com/1T45git/testjupyter.git
```

Проверяем, что новый удаленный репозиторий добавлен
```
git remote -v
```
Выбираем ветку и пушимся
```
git branch -M main

git push -u origin main
```
Далее вводим свой логин Git hub, пароль пока не трогаем.

мой username: hek1412

![image.png](Git+в+юпитере+8995d786-6f79-41d6-abc2-9ddf4673a681/image5.png)

И вот тут самое интересное)

Заходим в свой Git где Ваши репозитории, не организации 1Т45 

Делаем все как на картинках для создания персонального токена доступа (классические)

![image.png](Git+в+юпитере+8995d786-6f79-41d6-abc2-9ddf4673a681/image6.png)

![image.png](Git+в+юпитере+8995d786-6f79-41d6-abc2-9ddf4673a681/image7.png)



![image.png](Git+в+юпитере+8995d786-6f79-41d6-abc2-9ddf4673a681/image8.png)



![image.png](Git+в+юпитере+8995d786-6f79-41d6-abc2-9ddf4673a681/image9.png)



![image.png](Git+в+юпитере+8995d786-6f79-41d6-abc2-9ddf4673a681/image10.png)



![image.png](Git+в+юпитере+8995d786-6f79-41d6-abc2-9ddf4673a681/image11.png)



![image.png](Git+в+юпитере+8995d786-6f79-41d6-abc2-9ddf4673a681/image12.png)

Теперь сохраняем токен у себя, если забудете или потеряете, то нужно будет создать по новой

![image.png](Git+в+юпитере+8995d786-6f79-41d6-abc2-9ddf4673a681/image13.png)

Возвращаемся в терминал и вводим токен в поле для пароля!
Если Вы создали новый репозиторий, то все должно уже быть в Git hub

![image.png](Git+в+юпитере+8995d786-6f79-41d6-abc2-9ddf4673a681/image14.png)

Проверяем

![image.png](Git+в+юпитере+8995d786-6f79-41d6-abc2-9ddf4673a681/image 15.png)



###Клонирование (если репозиторий уже создан и там лежат нужные для работы файлы)

Тут получаем ссылку на репозиторий и вводим в терминале

![image.png](Git+в+юпитере+8995d786-6f79-41d6-abc2-9ddf4673a681/image16.png)

В другом блокноте (например у себя дома) в терминале вводим
```
git clone [https://github.com/1T45git/testjupyter.git](https://github.com/1T45git/testjupyter.git)
```
 Вводим имя и тот пароль который мы сохранили

![image.png](Git+в+юпитере+8995d786-6f79-41d6-abc2-9ddf4673a681/image17.png)

Слева появилась наша папка из репозитория, можем ей пользоваться, делать коммиты и пушить обратно)
