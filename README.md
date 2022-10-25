# Уроки по созданию блога на Evolution CMS 3

1. [Введение. Нужные программы и их настройки](/001_%D0%92%D0%B2%D0%B5%D0%B4%D0%B5%D0%BD%D0%B8%D0%B5.%20%D0%9D%D1%83%D0%B6%D0%BD%D1%8B%D0%B5%20%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D1%8B.md)
2. [Установка Evolution CMS](/002_%D0%A3%D1%81%D1%82%D0%B0%D0%BD%D0%BE%D0%B2%D0%BA%D0%B0%20Evolution%20CMS.md)
3. [Первоначальные настройки](/003_%D0%9F%D0%B5%D1%80%D0%B2%D0%BE%D0%BD%D0%B0%D1%87%D0%B0%D0%BB%D1%8C%D0%BD%D1%8B%D0%B5%20%D0%BD%D0%B0%D1%81%D1%82%D1%80%D0%BE%D0%B9%D0%BA%D0%B8.md)
4. [Структура сайта и шаблоны](/004_%D0%A1%D1%82%D1%80%D1%83%D0%BA%D1%82%D1%83%D1%80%D0%B0%20%D1%81%D0%B0%D0%B9%D1%82%D0%B0%20%D0%B8%20%D1%88%D0%B0%D0%B1%D0%BB%D0%BE%D0%BD%D1%8B.md)

5. [ТВ-параметры в Evolution CMS](/005_%D0%A2%D0%92-%D0%BF%D0%B0%D1%80%D0%B0%D0%BC%D0%B5%D1%82%D1%80%D1%8B%20%D0%B2%20Evolution%20CMS.md)

6. [Шаблон блога. Интеграция дизайна в Evolution CMS](/006_%D0%A8%D0%B0%D0%B1%D0%BB%D0%BE%D0%BD%20%D0%B1%D0%BB%D0%BE%D0%B3%D0%B0.%20%D0%98%D0%BD%D1%82%D0%B5%D0%B3%D1%80%D0%B0%D1%86%D0%B8%D1%8F%20%D0%B4%D0%B8%D0%B7%D0%B0%D0%B9%D0%BD%D0%B0%20%D0%B2%20Evolution%20CMS.md)

	
7. Контроллеры. Пакет main.
	* Отступление про MVC, пример, картинка, чёрт лысый -- не знаю пока.
	* Объяснить, что в шаблонах откуда-то надо брать данные и это "откуда-то" как раз и есть связь модели + контроллера.
	* Создадим BaseController, объясним что как, выведем условные helloworld'ы.
	* Покажем в Tracy, что доступно по умолчанию.
	* Выводим `$modx`, `$documentObject` 
	* Наследуемся от BaseController, делаем контроллеры для шаблонов. Упомянуть про дефисы в псевдониме и баги. 
	* Выводим всякое из `$documentObject` в шаблоны, чтобы отличать, где какой контроллер что отдал.

7. Навигация по сайту
	* делаем в вынесенном кусочке хидера менюшку на DLMenu в BaseController.
	* потыкаться, обратить внимание, что контента нема.
8. Выводим анонсы записей в блоге, делаем пагинацию
	* лезем в контроллер ленты блога, выводим docLister'ом
	* мутим пагинацию
	* делаем шаблончик для поста в ленте
	* хелперы. Сделаем ресайз превьюшки.
9. Оформление внутренних страниц блога
	* засовываем поля из documentObject в шаблон
	* опять же ресайз
	* похожие записи (?)
10. Сайдбар
	* если будет сайдбар, надо тут будет им заняться:  случайные посты, скажем, или ещё как-то.
11. Теги
	* ставим collection от Михаила
	* создаём шаблон для тегов и тега, контроллеры к ним
	* ставим Selector, создаём ТВ для тегов.
	* создаём в дереве теги
	* крестом и пестом прибиваем это дело друг к другу
12. Контактная страница, XML и HTML карты
	* для xml можно пакет мой
	* для html тот же DLMenu или DocLister
13. Поиск (?)
14. Наведение красоты
	* te3, шаблоны