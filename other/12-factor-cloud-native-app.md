# 12 факторов cloud native applications от Heroku

<hr>

## Признаки cloud native applications
* Используют декларативный формат для описания процесса установки и настройки, что сводит к минимуму затраты времени и ресурсов для новых разработчиков, подключённых к проекту
* Имеют соглашение с операционной системой, предполагающее максимальную переносимость между средами выполнения
* Подходят для развёртывания на современных облачных платформах, устраняя необходимость в серверах и системном администрировании
* Сводят к минимуму расхождения между средой разработки и средой выполнения, что позволяет использовать непрерывное развёртывание (continuous deployment) для максимальной гибкости
* Могут масштабироваться без существенных изменений в инструментах, архитектуре и практике разработки

## Двенадцать факторов

#### I. Кодовая база
Одна кодовая база, отслеживаемая в системе контроля версий, – множество развёртываний
#### II. Зависимости
Явно объявляйте и изолируйте зависимости
#### III. Конфигурация
Сохраняйте конфигурацию в среде выполнения
#### IV. Сторонние службы (Backing Services)
Считайте сторонние службы (backing services) подключаемыми ресурсами
#### V. Сборка, релиз, выполнение
Строго разделяйте стадии сборки и выполнения
#### VI. Процессы
Запускайте приложение как один или несколько процессов не сохраняющих внутреннее состояние (stateless)
#### VII. Привязка портов (Port binding)
Экспортируйте сервисы через привязку портов
#### VIII. Параллелизм
Масштабируйте приложение с помощью процессов
#### IX. Утилизируемость (Disposability)
Максимизируйте надёжность с помощью быстрого запуска и корректного завершения работы
#### X. Паритет разработки/работы приложения
Держите окружения разработки, промежуточного развёртывания (staging) и рабочего развёртывания (production) максимально похожими
#### XI. Журналирование (Logs)
Рассматривайте журнал как поток событий
#### XII. Задачи администрирования
Выполняйте задачи администрирования/управления с помощью разовых процессов