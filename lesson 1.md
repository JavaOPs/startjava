# Занятие первое

## Темы занятия
1. [Подготовка рабочего окружения](#1)
1. [Первая программа](#2)
1. [Ручная компиляция и запуск программы](#3)
1. [Этапы компиляции и запуска](#4)
1. [Байт-код](#5)
1. [Переменные: примитивные типы данных](#6)
1. [Ветвление: if-else](#7)
1. [Циклы: for, while, do-while](#8)
1. [Система управления версиями Git](#9)
1. [Итоговые домашние задания](#10)
1. [Опросники](#11)
1. [Общие рекомендации по выполнению домашних заданий](#12)

**На данный момент проверка домашних заданий проводится в [Telegram](https://t.me/+uSmw5Ca3RKk0OWQy) в индивидуальном режиме**

## Полезные ссылки для ознакомления с курсом
- [Видеообзор курса StartJava](https://youtu.be/vM1ygW7pKTE) (youtube)
- [Демонстрация проверки домашних заданий наставником](https://youtu.be/H_PYOW9Qq80?si=isPC3-aYYPhDWL5B) (youtube)
- [Отзывы выпускников о курсе](https://vk.com/topic-18505771_38447031?offset=100)

**Обязательно читайте книги из списка в [статье](https://topjava.ru/blog/spisok-knig-dlya-nachinayushchego-java-programmista) параллельно с изучаемыми темами**

> ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) — эта иконка означает, что рядом находится ссылка на видеоурок: нажмите на нее, чтобы посмотреть видео

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 1. <a name="1">[Подготовка рабочего окружения](https://drive.google.com/file/d/1gWrBFrly3BdXKq868Xr0QkGtpM9FCmI4/view?usp=sharing)</a>

- [Установите и настройте Java](https://topjava.ru/blog/ustanovka-i-nastroyka-java)
- Установите [Sublime Text 4](https://www.sublimetext.com/download) (с четвертого урока перейдем на IntelliJ IDEA)

**Дополнительные источники:**
- [История возникновения Java](https://topjava.ru/blog/zabytaya-istoriya-java-glazami-patrika-notona)
- [Знакомство с языком Java](https://www.youtube.com/live/QGHGR0xEcFA?si=xW98gPEVGZX_UrG5) (youtube)
- [Что такое JDK? Введение в средства разработки Java](https://topjava.ru/blog/what-is-the-jdk)
- [Что такое JRE? Введение в среду выполнения Java](https://topjava.ru/blog/what-is-the-jre)
- [Что такое JVM? Знакомство с виртуальной машиной Java](https://topjava.ru/blog/what-is-the-jvm)
- Отчеты о популярности Java-технологий:
  - [Java в 2025 году](https://habr.com/ru/companies/spring_aio/articles/933180/)
  - [State of Developer Ecosystem Report 2025](https://devecosystem-2025.jetbrains.com/ru)
  - [Java Trends Report 2025](https://www.infoq.com/articles/java-trends-report-2025/)
  - [The 2025 Developer Survey](https://survey.stackoverflow.co/2025)
  - Рейтинги популярности языков программирования: [TIOBE](https://www.tiobe.com/tiobe-index/), [PYPL](https://pypl.github.io/PYPL.html), [IEEE](https://spectrum.ieee.org/tag/top-programming-languages)

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 2. <a name="2">[Первая программа](https://drive.google.com/file/d/1anXQBZ80wvfzozUNlfhy1wtS-eS50cZi/view?usp=sharing)</a>

- Изучите статью [Java с нуля: первая программа](https://topjava.ru/blog/pervaya-programma-na-java). В ней показано создание простой программы `MyFirstApp`, а также дан подробный разбор каждой строки кода:

``` java
public class MyFirstApp {	
    public static void main(String[] args) {
        System.out.println("Write once, run anywhere");
    }
}
```

- [Настройте](https://topjava.ru/blog/nastroyka-sublime-text-dlya-java) Sublime Text для Java
- Обязательно настройте [проверку правописания](https://topjava.ru/blog/nastroyka-sublime-text-dlya-java#7) и [статический анализ кода](https://topjava.ru/blog/nastroyka-sublime-text-dlya-java#9) для Sublime Text

**Дополнительные источники:**
- [Обзор и настройка Sublime Text](https://youtu.be/xWhTf_o86Lg) (youtube) — видео дано для знакомства с возможностями редактора. Не обязательно повторять все действия автора
- [Установка плагина Terminal для Sublime Text](https://youtu.be/9cFW481D2lU) (youtube) — можно использовать этот плагин или `Terminus`

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 3. <a name="3">[Ручная компиляция и запуск программы](https://drive.google.com/file/d/1u0jyGJkFFLUwfj0c21uY2i2louNtIm_3/view?usp=sharing)</a>
- Изучите статьи:
  - ["Основы командной строки для Java-программиста"](https://topjava.ru/blog/osnovy-komandnoy-stroki-dlya-java-programmista)
  - [Компиляция и запуск Java-программ](https://topjava.ru/blog/kompilyatsiya-i-zapusk-programm-na-java)
    
Для компиляции и запуска программы необходимо в консоли перейти в директорию, в которой находится файл `MyFirstApp.java`, и выполнить по очереди следующие команды:
- `javac MyFirstApp.java` — компиляция Java-файла
- `java MyFirstApp` — запуск программы

Для однофайловых программ, начиная с Java 11, компиляция и запуск выполняются одной командой:
- `java MyFirstApp.java`

**Дополнительные источники:**
- [Getting Started with Java](https://dev.java/learn/getting-started/)
- [Введение в командную строку Windows](https://www.youtube.com/user/Iidsp/videos) (youtube)

## 4. <a name="4">Этапы компиляции и запуска</a>
Ознакомьтесь со схемой этапов компиляции и запуска Java-программы
![Frame 303](https://github.com/user-attachments/assets/a01dd0f6-b054-4bdf-99bd-aac39cb36bba)

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 5. <a name="5">[Байт-код](https://drive.google.com/file/d/19Tl7dEpPszjQfulzQBEwyn9sQL0DK3ji/view?usp=sharing)</a>
Чтобы посмотреть байт-код класса, перейдите в консоли в директорию, в которой находится файл `MyFirstApp.class`, и выполните команду:
- `javap -c -s -verbose MyFirstApp`

**Дополнительные источники:**
- [От исходников к байт-коду](https://abykov.dev/posts/java-platform-bytecode-jvm/)
- [Java байт-код «Hello world»](https://habr.com/post/264919/)
- [Байт-код Java](https://youtu.be/XZXgXjIJrYQ?si=jzwb4quAOxxTiDDa) (youtube)

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 6. <a name="6">[Переменные: примитивные типы данных](https://drive.google.com/file/d/1mrsKC-wU7NpxQiNt47rgfySsDGTwB8Wb/view?usp=sharing)</a>

**Дополнительные источники:**
- [Переменные в Java](https://youtu.be/Y__Ns7FS5lA?t=17) (youtube)
- [Creating Variables and Naming Them](https://dev.java/learn/language-basics/variables/)
- [Переменные. Типы данных](https://github.com/hvilinka/LevelUp_Java/blob/master/lectures/lecture2.md)
- [Примитивные типы данных](http://developer.alexanderklimov.ru/android/java/types.php)
- [Creating Primitive Type Variables](https://dev.java/learn/language-basics/primitive-types/)
- [Про размеры типов данных](https://youtu.be/3BmznLJAgaA?t=782)

<table align="center">
  <thead>
    <tr>
      <th align="center">Название</th>
      <th align="center">Размер,<br>байт</th>
      <th align="center">Диапазон значений</th>
      <th align="center">Описание</th>
      <th align="center">Пример</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center"><code>byte</code></td>
      <td align="center">1</td>
      <td align="center">-128 до 127</td>
      <td align="center">целое число</td>
      <td align="center"><code>byte b = -5</code></td>
    </tr>
    <tr>
      <td align="center"><code>short</code></td>
      <td align="center">2</td>
      <td align="center">-32_768 до 32_767</td>
      <td align="center">целое число</td>
      <td align="center"><code>short s = 42</code></td>
    </tr>
    <tr>
      <td align="center"><code>int</code></td>
      <td align="center">4</td>
      <td align="center">
        -2_147_483_648<br>
        до 2_147_483_647<br>
        (-2 ^ 31 до 2 ^ 31 - 1)
      </td>
      <td align="center">целое число</td>
      <td align="center"><code>int i = -12_345</code></td>
    </tr>
    <tr>
      <td align="center"><code>long</code></td>
      <td align="center">8</td>
      <td align="center">
        -9_223_372_036_854_775_808<br>
        до 9_223_372_036_854_775_807<br>
        (-2 ^ 63 до 2 ^ 63 - 1)
      </td>
      <td align="center">целое число</td>
      <td align="center"><code>long ln = 3_000_000_000L</code></td>
    </tr>
    <tr>
      <td align="center"><code>float</code></td>
      <td align="center">4</td>
      <td align="center">
        ±1.4E - 45<br>
        до ±3.4028235E + 38
      </td>
      <td align="center">вещественное число</td>
      <td align="center"><code>float f = 3.141f</code></td>
    </tr>
    <tr>
      <td align="center"><code>double</code></td>
      <td align="center">8</td>
      <td align="center">
        ±4.49E - 324<br>
        до ±1.7976931348623157E + 308
      </td>
      <td align="center">вещественное число<br>двойной точности</td>
      <td align="center"><code>double d = 3.141_592</code></td>
    </tr>
    <tr>
      <td align="center"><code>char</code></td>
      <td align="center">2</td>
      <td align="center">0 до 65_535</td>
      <td align="center">символ</td>
      <td align="center"><code>char c = 'Z'</code></td>
    </tr>
    <tr>
      <td align="center"><code>boolean</code></td>
      <td align="center">1 бит</td>
      <td align="center"><code>true</code> или <code>false</code></td>
      <td align="center">логическое значение</td>
      <td align="center"><code>boolean b = true</code></td>
    </tr>
  </tbody>
</table>

**Домашнее задание**
1. Разберитесь с [Git/GitHub](https://github.com/JavaOPs/startjava/blob/master/lesson%201.md#9)
1. Выполните все задания на тему ["Именование переменных"](https://docs.google.com/document/d/1Dv-eo8acvOVFJtUVbaWd1Mfb77Q1IiTlhepgy56qMbc/edit?usp=sharing)
1. Пришлите наставнику ссылку на удаленный репозиторий с решенными заданиями
1. После того как наставник примет предыдущие задания, выполните задания на тему ["Примитивные типы данных"](https://docs.google.com/document/d/1kJqeCC-fKWUjBjrmHJ1mjDu45SGRL39Q5vW4DmLJflA/edit?usp=sharing)

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 7. <a name="7">[Ветвление: if-else](https://drive.google.com/file/d/1r-UVn4Z9OhV-SUvJdMrC6EG_v9qowAJS/view?usp=sharing)</a>

![turpal](https://user-images.githubusercontent.com/29703461/39215173-9afa64b4-481f-11e8-9731-fa60a8439f71.jpg)

**Дополнительные источники:**
- [Оператор if-else в Java](https://youtu.be/ryR033ld_N0) (youtube)
- [Тернарный оператор](https://topjava.ru/blog/ternarnyy-operator-v-java)
- [The if-then and if-then-else Statements](https://dev.java/learn/language-basics/controlling-flow/)
- [If Statements](https://learn.java/learning/tutorials/CS12Algorithms/ifstatements/)
- [Nested If Statements](https://learn.java/learning/tutorials/CS12Algorithms/nested-if-statements/)
- [Equivalent if Statements](https://learn.java/learning/tutorials/CS12Algorithms/equivalent-if-statements/)

**Домашнее задание**
- Выполните все задания на тему ["Ветвление: if-else"](https://docs.google.com/document/d/1LZLCupFXrCmTuaT4KCUW9nKjrzaFDCCH7i5PDpWSLjI/edit?usp=sharing)
- Сдайте наставнику на проверку выполненные задания

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 8. <a name="8">Циклы: [for](https://drive.google.com/file/d/1MxaPlSwY6-Nv2zOrQGYy5lOSDjYTfnfU/view?usp=sharing), [while, do-while](https://drive.google.com/file/d/1YQHY9C1QbueWYFMRBpHFTqg1wt9N_333/view?usp=sharing)</a>
![loop](https://user-images.githubusercontent.com/29703461/39228479-100883f2-4867-11e8-9d63-5d18e455aaa2.jpeg)

**Дополнительные источники:**
- Циклы в Java [1](https://timeweb.cloud/tutorials/java/cikly-v-java-osnovy-raboty), [2](https://vertex-academy.com/tutorials/ru/cikly-v-java/)
- [Оператор while](https://youtu.be/15PjODTSTaw) (youtube)
- [Оператор for](https://youtu.be/UYbdAmgcNVc) (youtube)

**Домашнее задание**
- Выполните все задания на тему ["Циклы: for, while, do-while"](https://docs.google.com/document/d/1lHSSOzARTx6tfD-4MV-t41S5bnvdNw5hczkQPT05png/edit?usp=sharing)
- Сдайте наставнику на проверку выполненные задания

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 9. <a name="9">[Система управления версиями Git](https://drive.google.com/file/d/1IMw7DA_lodW2GueWpU1nMUmYx0pnlPGA/view?usp=sharing)</a>

Процесс работы с Git сводится к следующим шагам
![image](https://user-images.githubusercontent.com/29703461/154850409-7a618576-1105-48a1-9e32-88a34e87693b.png)

- [Установите и настройте Git/GitHub](https://topjava.ru/blog/vvedeniye-v-git-github-ustanovka-i-nastroyka)
- Изучите [базовые команды Git](https://topjava.ru/blog/vvedeniye-v-git-github-bazovyye-komandy)
 
### Настройка локального репозитория
- Создайте в удобном для вас месте директорию `startjava`, в которой будет храниться ваш код
- Создайте на GitHub репозиторий `startjava`
- Откройте консоль в директории `startjava`
- Если вы еще не настроили локальный репозиторий, выполните команды:
  - `git init` — создание локального репозитория
  - `git status` — просмотр состояния файлов
  - `git remote add origin url_на_ваш_startjava-репозиторий.git` — добавление адреса удаленного репозитория
  - `git remote -v` — проверка, что адрес репозитория добавлен

### Рекомендации по Git
- Не добавляйте в репозиторий файлы с расширением `class`
- В репозиторий можно добавлять не только Java-файлы, но и директории с кодом, например, `Lesson 1`
- Перед отправкой задания наставнику убедитесь, что все изменения закоммичены и отправлены в GitHub
- При возникновении проблем обратитесь к статье ["Ошибки использования Git"](https://topjava.ru/blog/vvedeniye-v-git-oshibki-ispolzovaniya-ch-9)

**Дополнительные источники:**
  - [Базовый курс по обучению Git](https://www.youtube.com/playlist?list=PLIU76b8Cjem5B3sufBJ_KFTpKkMEvaTQR) (youtube)
  - [Git. Быстрый старт](https://www.youtube.com/watch?v=4-NX17Ip-xQ&list=PLmRNNqEA7JoM77hOJkPrLOfJQGizCLR3P) (youtube)
  - Интерактивные Git-обучалки: [1](https://githowto.com/ru), [2](http://learngitbranching.js.org)
  - [Официальная книга по Git](https://git-scm.com/book/ru/v2)

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 10. <a name="10">[Итоговые домашние задания](https://drive.google.com/file/d/1Svgm_03td3Aj_MeVt-MBqSCv-PEhXD0A/view?usp=sharing)</a>

- Выполните все [итоговые домашние задания](https://docs.google.com/document/d/1m6y5qBMfwKjm0DIo3JYqQ9_QNyhroDvsRAirEyDEP7s/edit?usp=sharing)
- Сдайте наставнику на проверку выполненные задания

<details>
<summary>Так должна выглядеть структура ваших папок и файлов</summary>
    
![tree](https://github.com/ichimax/startjava/assets/29703461/47ca8fc6-3f00-4c24-a07d-0e2416f12eb6)
</details>

## 11. <a name="11">Опросники</a>
- [Итоговый тест](https://forms.gle/YFc2pf6qZw6jdfXM7) позволит вам проверить, насколько хорошо вы освоили пройденные в уроке темы
- В этом [опроснике](https://forms.gle/dsthsvh1tRhdJyhu9) вы сможете анонимно поделиться впечатлениями о первом уроке: что понравилось, что не понравилось, что можно улучшить. Ваши ответы помогут сделать урок лучше

## 12. <a name="12">Общие рекомендации по выполнению домашних заданий</a>

1. [Правила](https://github.com/JavaOPs/startjava/blob/master/rules.md) проверки заданий наставником
1. Ссылку на репозиторий достаточно прислать наставнику один раз. Для последующих заданий просто сообщайте, что они готовы к проверке
1. При выполнении заданий используйте только те темы, которые изучались в текущем уроке
1. Ввод с клавиатуры, методы класса `Math` или `Random` пока не используйте (но, если вы знаете про них и хотите использовать — дерзайте)

## Немного мотивации
- [Как приучить себя к дисциплине и осуществлять свои планы](https://youtu.be/wbItXmjm7tY?si=RceAgonMsijaz3KD)
- [Shia LaBeouf Motivation for Coding](https://youtu.be/J1usv2Hn-pU)
- [Мотивация для программистов](https://www.youtube.com/watch?v=NOVaNe3jx6c)
- [Речь Стива Джобса перед выпускниками Стенфорда](https://www.youtube.com/watch?v=WVz9E7o1mmk)
- [Мотивационный совет от Стива Джобса](https://www.youtube.com/watch?v=Z2qSUZ1o47U)
- [12 минут сильнейшей мотивации. Перелом сознания](https://www.youtube.com/watch?v=69MkvKrraC0)
- [Почему мне так сложно учиться программировать?](https://youtu.be/TtT8UNK0sGg)
- [Простой прием стать программистом быстрее](https://youtu.be/iw3E-Gdncwc)
