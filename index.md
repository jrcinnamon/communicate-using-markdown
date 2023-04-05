# First Header
#### Second Header
![Image of Nashville](https://media.cntraveler.com/photos/63ed72db43ca80edc4421e99/4:3/w_2668,h_2001,c_limit/Nashville_GettyImages-612679836.jpg)
SELECT region_name, COUNT(DISTINCT node_id) AS node_count, COUNT(DISTINCT customer_id) AS customer_count
FROM customer_nodes
INNER JOIN regions
USING(region_id)
GROUP BY region_name;
