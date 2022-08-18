# Анализ перспективных игровых платформ и жанров

## Статус проекта
Завершен

## Описание проекта
Интернет-магазине «Стримчик» продает по всему миру компьютерные игры. Из открытых источников доступны исторические данные о продажах игр, оценки пользователей и экспертов, жанры и платформы (например, Xbox или PlayStation). Мне нужно выявить определяющие успешность игры закономерности. Это позволит сделать ставку на потенциально популярный продукт и спланировать рекламные кампании.
Мне предоставлены данные до 2016 года.  

## Описание данных

- Name — название игры
- Platform — платформа
- Year_of_Release — год выпуска
- Genre — жанр игры
- NA_sales — продажи в Северной Америке (миллионы проданных копий)
- EU_sales — продажи в Европе (миллионы проданных копий)
- JP_sales — продажи в Японии (миллионы проданных копий)
- Other_sales — продажи в других странах (миллионы проданных копий)
- Critic_Score — оценка критиков (максимум 100)
- User_Score — оценка пользователей (максимум 10)
- Rating — рейтинг от организации ESRB 

## Вывод

На основании упомянутых промежуточных выводов можно сформулировать следующий общий вывод:

Наиболее перспективными платформами в целом в мире в настоящий момент являются Playstation 4, Xbox One, Nintendo 3DS, PC и WiiU. Все указанные платформы находятся в середине своего жизненного цикла и останутся популярными в 2017 году.
Самые популярные игровые жанры: Shooter, Action, Sports и RPG. При этом доля рынка для жанра Shooter и Sports растет, для жанра RPG стабильна, для жанра Action снижается.
Оценки критиков (особенно высокие) позволяют с некоторой уверенностью определить будущую успешность игры. Оценки игроков могут использоваться для определения коммерческого успеха только для платформы WiiU.
В Северной Америке наибольшие продажи ожидаются для игр, выпущенных для платформ Playstation 4 и Xbox One (у Xbox One средние продажи выше, несмотря на более низкую долю рынка) в жанрах Shooter и Sports и рейтингом M.
В Европе наибольшие продажи ожидаются для игр, выпущенных для платформ Playstation 4 и Xbox One в жанрах Shooter и Sports и рейтингом M.
В Японии наибольшие продажи ожидаются для игр, выпущенных для платформ Nintendo 3DS, Playstation 4 и Playstation Vita в жанрах RPG и Action с рейтингом E.

Сводные результаты исследования представлены в таблице ниже.
<table>
         <thead>
           <tr>
             <th></th>
             <th>Северная Америка</th>
             <th>Европа</th>
             <th>Япония</th>
             <th>Мир в целом</th>
           </tr>
         </thead>
         <tbody>
           <tr>
             <th>Наиболее популярная игровая платформа</th>
             <td>Playstation 4</td>
             <td>Playstation 4</td>
             <td>Nintendo 3DS</td>
             <td>Playstation 4</td>
           </tr>
           <tr>
             <th>Доля продаж для самой популярной игровой платформы</th>
             <td>47.8%</td>
             <td>62%</td>
             <td>41.6%</td>
             <td>53.3%</td>
           </tr>
           <tr>
             <th>Дополнительные популярные игровые платформы</th>
             <td>Xbox One, WiiU</td>
             <td>Xbox One, WiiU</td>
             <td>Playstation 4, WiiU</td>
             <td>Xbox One, Nintendo 3DS</td>
           </tr>
           <tr>
             <th>Наиболее популярный игровой жанр</th>
             <td>Shooter</td>
             <td>Shooter</td>
             <td>RPG</td>
             <td>Shooter</td>
           </tr>
           <tr>
             <th>Доля продаж для самого популярного жанра</th>
             <td>36.1%</td>
             <td>31%</td>
             <td>36.6%</td>
             <td>29%</td>
           </tr>
           <tr>
             <th>Дополнительные популярные жанры</th>
             <td>Sports</td>
             <td>Sports</td>
             <td>Action</td>
             <td>Action, RPG, Sports</td>
           </tr>
           <tr>
             <th>Самый прибыльный рейтинг ESRB</th>
             <td>M</td>
             <td>M</td>
             <td>N/A</td>
             <td>M</td>
           </tr>
           <tr>
             <th>Наиболее выгодная связка "платформа-жанр"</th>
             <td>Xbox One - Shooter</td>
             <td>Playstation 4 - Shooter</td>
             <td>Nintendo 3DS - RPG</td>
             <td>Playstation 4 - Shooter</td>
           </tr>
           <tr>
             <th>Дополнительные выгодные связки "платформа-жанр"</th>
             <td>Playstation 4 - Sports, Playstation 4 - Shooter, Xbox One - Sports</td>
             <td>Playstation 4 - Sports, Xbox One - Shooter, Xbox One - Sports, Xbox One - RPG</td>
             <td>Nintendo 3DS - Action, Playstation 4 - Action</td>
             <td>Playstation 4 - Shooter, Playstation 4 - Sports, Playstation 4 - Action, Xbox One - Shooter, Xbox One - Sports, Nintendo 3DS - RPG</td>
           </tr>
         </tbody>
       </table>

## Используемые библиотеки
*pandas, numpy, scipy, matplotlib, seaborn*