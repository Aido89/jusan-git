Данный репозиторий содержит скрипт для вывода моего ID на stepik.org 

#!/bin/bash
echo "ID вашего профиля на stepik.org:"
curl -s https://stepik.org/api/users/me/ | grep -oP '(?<=id":)\d+'
