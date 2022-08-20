# real_estate_visits

SQL-запрос, результатом которого будет список фамилий клиентов, записанных на просмотр двух и более трехкомнатных квартир:

SELECT *

FROM view

JOIN client ON view.client_id = client.id

JOIN apartment ON view.apartment_id = apartment.id

WHERE apartment.rooms = 3;
