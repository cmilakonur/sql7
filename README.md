# sql7
patika.dev linkim: https://app.patika.dev/cmilakonur <br />

1- film tablosunda bulunan filmleri rating değerlerine göre gruplayınız. <br />
SELECT rating, count(*) FROM film <br />
GROUP BY rating  <br />
    
2- film tablosunda bulunan filmleri replacement_cost sütununa göre grupladığımızda film sayısı 50 den <br />
fazla olan replacement_cost değerini ve karşılık gelen film sayısını sıralayınız. <br />
SELECT replacement_cost, count(*) FROM film  <br />
GROUP BY replacement_cost <br />
HAVING count(replacement_cost) >50 <br />

3-customer tablosunda bulunan store_id değerlerine karşılık gelen müşteri sayılarını nelerdir?  <br />
SELECT store_id,COUNT(*) from customer <br />
GROUP BY store_id; <br />

4-city tablosunda bulunan şehir verilerini country_id sütununa göre gruplandırdıktan sonra en fazla şehir
sayısı barındıran country_id bilgisini ve şehir sayısını paylaşınız. <br />
SELECT country_id,COUNT(*) from city <br />
GROUP BY country_id <br />
ORDER BY COUNT(*) DESC <br />
LIMIT 1; <br />
