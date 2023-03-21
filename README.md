# SQL-ODEV-7
film tablosunda bulunan filmleri rating değerlerine göre gruplayınız.
ÇÖZÜM: SELECT rating FROM film
GROUP BY rating

![4564553](https://user-images.githubusercontent.com/128131203/226609986-6cc03c77-09c2-4f62-b0b0-ebcb0f61c5c0.PNG)

film tablosunda bulunan filmleri replacement_cost sütununa göre grupladığımızda film sayısı 50 den fazla olan replacement_cost değerini ve karşılık gelen film sayısını sıralayınız.
ÇÖZÜM: SELECT replacement_cost, COUNT(*) FROM film
GROUP BY replacement_cost
HAVING COUNT(*) >50;

![DSFVSD](https://user-images.githubusercontent.com/128131203/226615783-2d2d5485-cc1a-466c-8881-0126e86e9449.PNG)

customer tablosunda bulunan store_id değerlerine karşılık gelen müşteri sayılarını nelerdir? 
ÇÖZÜM:select store_id, count(*) from customer
GROUP BY store_id

![fgvfdgvad](https://user-images.githubusercontent.com/128131203/226616520-561eb288-5a0d-46c4-8574-c3096ab1b194.PNG)

city tablosunda bulunan şehir verilerini country_id sütununa göre gruplandırdıktan sonra en fazla şehir sayısı barındıran country_id bilgisini ve şehir sayısını paylaşınız.
ÇÖZÜM: select country_id, count(*) from city 
GROUP BY country_id
ORDER BY count(*) desc
limit 1

![sdfgvafdzxcg](https://user-images.githubusercontent.com/128131203/226618515-b3f8f6bb-e40e-476d-a982-23f52fe1ae05.PNG)
