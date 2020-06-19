# Работа с файловой системой

[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/artem-prozorov/filemanager/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/artem-prozorov/filemanager/?branch=master)
[![Build Status](https://scrutinizer-ci.com/g/artem-prozorov/filemanager/badges/build.png?b=master)](https://scrutinizer-ci.com/g/artem-prozorov/filemanager/build-status/master)
[![Code Intelligence Status](https://scrutinizer-ci.com/g/artem-prozorov/filemanager/badges/code-intelligence.svg?b=master)](https://scrutinizer-ci.com/code-intelligence)

Библиотека представляет из себя набор команд, обернутых в класс, для выполнения файловых операций. Рекомендуется использовать этот класс как синглтон на уровне системы.

Теперь файловые операции, такие как переименование, проверка на существование, получение содержимого, удаление и тд, можно осуществлять следующим образом:
```
use Prozorov\Filemanager\Manager;

$manager = new Manager();

$file = '/foo/bar';

$contents = $manager->getContents($file);
```
