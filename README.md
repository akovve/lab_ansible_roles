# Лабораторная работа П06: Ansible Roles и CI (GitHub Actions)

## Цель работы
Создание Ansible-роли для развертывания Nginx с виртуальными хостами и настройка Continuous Integration (CI) с помощью GitHub Actions.

## Что было сделал
1. Создан новый репозиторий на GitHub и склонирован на VM-1.
2. Написана Ansible-роль `nginx_vhosts` для установки Nginx и создания виртуальных хостов (через Jinja2-шаблоны).
3. Написаны плейбук и инвентарь для запуска роли.
4. Настроены два пайплайна GitHub Actions: тестовый и проверка кода (`ansible-lint`).

---

## Исходники

**Инвентарь и Плейбук:**

> **<img width="1021" height="133" alt="image" src="https://github.com/user-attachments/assets/cbb8f9ba-c6ee-42e1-87b6-04cbe1b11e08" />**
> **<img width="977" height="390" alt="image" src="https://github.com/user-attachments/assets/fca5e7fb-a329-421f-a201-101b05ed66b3" />**

**Файлы роли (tasks, handlers, templates):**
> **<img width="1048" height="805" alt="image" src="https://github.com/user-attachments/assets/2349e125-6ba3-480e-9b19-81649bc2d2f4" />**
> **<img width="1007" height="183" alt="image" src="https://github.com/user-attachments/assets/4521215e-6041-49cc-8c3e-dbcfd26aac1b" />**
> **<img width="1047" height="291" alt="image" src="https://github.com/user-attachments/assets/0841234b-5f0a-444e-913f-d1c383aed9dd" />**

**Файлы CI (GitHub Actions):**
> **<img width="1113" height="438" alt="image" src="https://github.com/user-attachments/assets/8936831c-76e8-4b1a-983c-5aa44eb64c3a" />**
> **<img width="1034" height="398" alt="image" src="https://github.com/user-attachments/assets/baabb0dd-57d5-4972-a8ed-95ad8ce9c46b" />**

---

## Результаты

**Проверка работы Nginx:**
> **<img width="969" height="457" alt="image" src="https://github.com/user-attachments/assets/32766a8d-22e3-412b-b5d9-d36d99ca1e9d" />**
> **<img width="985" height="491" alt="image" src="https://github.com/user-attachments/assets/73cafc45-a727-4421-a9f8-e282d723e754" />**

**Успешное прохождение CI (GitHub Actions):**
> **<img width="1248" height="191" alt="image" src="https://github.com/user-attachments/assets/d894443a-515f-47d2-82f9-369098ed9179" />**

---

## Вывод
В ходе работы освоены навыки создания структурированных Ansible-ролей с шаблонами Jinja2. Настроен CI-пайплайн, который автоматически проверяет код при каждом пуше и помогает поддерживать его качество.
