# anecdote_bot
Этот проект нацелен на создание генератора анекдотов при помощи PyTorch на основе языковой модели ai-forever/rugpt3small_based_on_gpt2 от Сбера. Мы дообучаем её на файле с ~124000 анекдотов и генерируем новые из промптов, которые получаем при помощи Телеграм-бота, и присылаем в ответ результат.

В текущем виде проект создан для локального воспроизведения на ПК на Windows 11 ввиду ограниченного доступа к онлайн-IDE, позволяющей провести длительное и ресурсоёмкое дообучение модели без ошибок и отказов. Если у Вас есть время и возможность воспользоваться более крупной версией модели от Сбера (вариации medium, large и XL), это приветствуется и только улучшит качество итоговой модели.

Если планируется локальное воспроизведение, то не рекомендуется запускать его на видеокартах с объемом памяти меньше, чем 6 ГБ GDDR6, поскольку ровно в такой конфигурации память была занята практически полностью. Если речь о видеокартах Nvidia, большим плюсом будет наличие у неё тензорных ядер, то есть модели начиная с RTX 2060 и далее.

Качество анекдотов в исходном файле может посчитаться своеобразным, и, вероятно, существует возможность собрать базу более приличных и приемлемых анекдотов, однако в рамках данного проекта этот удобный файл с существенным объемом позиций оптимален.
