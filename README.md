# Несколько типов цен в редакции малый бизнес 1С Битрикс Управление сайтом

Поумолчанию в 1С Битрикс в редакции малый бизнес можно создать только один тип цены.

![Image](https://raw.githubusercontent.com/BravOFF/Several_Types-_Of_Prices_Bitrix_small_business/master/bit.png)

Но оказалось есть возможность их включить в файле настровки.
Модуль каталог желательно скопиравить в ```/local/modules```, правдо тогда модуть теряет возможнось обновляться.
В файле ```/bitrix/modules/catalog/lib/config/feature.php``` или если перенесли в ```/local/``` то ```/local/modules/catalog/lib/config/feature.php``` меняем ```private static $featureList = [];``` на ```private static $featureList = ['catalog_multi_price_types' => 'CatMultiPrice'];```

![Image](https://raw.githubusercontent.com/BravOFF/Several_Types-_Of_Prices_Bitrix_small_business/master/bit2.png)

Вот и всё!
