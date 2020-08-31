# Unity-Code-Convention
Документация проектов
- [Код](#код)
- [Unity проект](#unity-проект)
- [Контроль версий](#контроль-версий)
## Код
- Для классов, имен файлов, namespace'ов, методов, свойств используется **PascalCase**
- Для переменых используется **CamelCase**
- Все скрипты должны иметь **namespace** в виде **SabGames.НазваниеПроекта**
- Модификаторы доступа (*public*, *private*, *protected*), должны быть прописаны везде
- Все *private* и *protected* переменные должны начинаться со знака подчеркивания
```
private int _hp;
```
- Вместо прямого прописывания типа, следует использовать **var**
- Колбеки Unity (*Start*, *Update*, *OnEnable*, *OnDisable* и т.д.) должны быть прописаны до основных методов скрипта
## Unity проект
- Версия Unity **2019.4.9f1**
- Версия API **.NET 4.x**
- Scripting Backend **IL2CPP**
### Структура папок проекта
Все сторонние библиотеки должны помещаться в папку **3rd Party**. Никакие файлы сторонних библиотек не должны модифицироваться, если требуется модификация, файл необходимо скопировать.

Общая структура папок:
- 3rd Party
- Animations
- Editor
- Fonts
- Materials
- Meshes
- Plugins
- Prefabs
- Resources
- Scenes
- SFX
- Sprites
### Оптимизация
- По возможности, спрайты должны собираться в **Sprite Atlas** внутри Unity

### Часто используемые библиотеки
- [Dotween](http://dotween.demigiant.com/) (твины)
- [Spine](http://en.esotericsoftware.com/spine-unity-download) (анимация)
## Контроль версий
Для контроля версий используется git. Наш [сервер](http://git2.sablab.org/).
> GUI [Source Tree](https://www.sourcetreeapp.com/), [Fork](https://git-fork.com/)

- Для описания коммитов используется только английский язык
- Описание коммитов должно быть коротким
- В начале каждого описания прописывается основная цель коммита в форме инфинитива (**Add** | **Update** | **Remove** | **Fix** и т.д.)
- Используемый [Gitignore](https://github.com/github/gitignore/blob/master/Unity.gitignore) файл
- Используется [Git Flow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)
