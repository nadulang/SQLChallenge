# SQLChallenge

1. select customers.id, customers.forename, customers.surname, orders.registered, orders.payment_type, orders.status, orders.total 
 	from customers 
 	join orders on customers.id = orders.customer_id order by id; 
2.  select status, count(status) from orders group by status;
3.  select categories.id, products.name, products.description, products.image, products.price  
  from categories  
  join products on categories.id = products.cat_id order by categories.id;
4.   select  orders.id, delivery_addresses.add1  
  from delivery_addresses  
  join orders on delivery_addresses.id = orders.delivery_add_id; 
5.  select orders.id, products.name 
 from products 
 join order_items on order_items.product_id = products.id 
 join orders on order_items.order_id = orders.id order by id;
