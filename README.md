# 🐝 Atividade-BeeCrowd
Objetivo: Treinar e Familiarizar com a linguagem SQL utilizando uma sequência de atividades do site BeeCrowd
---
## Atividades Nível 01
### Atividade 2603

<img width="1092" height="323" alt="Image" src="https://github.com/user-attachments/assets/9f359265-794b-4ac6-8888-a648696b8273" />

``` sql
SELECT
	name, street
FROM
	customers
WHERE
	city = 'Porto Alegre';
```

### Atividade 2607

<img width="1095" height="324" alt="Image" src="https://github.com/user-attachments/assets/405c94ed-229c-4189-a6cf-dacf06832e8e" />

``` sql
SELECT
	city
FROM
	providers
ORDER BY
	city ASC;
```

### Atividade 2608

<img width="1093" height="321" alt="Image" src="https://github.com/user-attachments/assets/f7311788-017f-4943-888b-7d357701438f" />

``` sql
SELECT
	max(price) as price,
	min(price) as price
FROM
	products;
```

### Atividade 2615

<img width="1095" height="322" alt="Image" src="https://github.com/user-attachments/assets/7fcc5b2f-b946-43fe-86ea-313de6342e31" />

``` sql
SELECT DISTINCT
	city
FROM
	customers;
```

### Atividade 2622

<img width="1094" height="312" alt="Image" src="https://github.com/user-attachments/assets/de363848-fabc-4455-b0b5-93bc2426fa69" />

``` sql
SELECT
	name
FROM
	customers
WHERE id in (SELECT id_customers FROM legal_person);
```

## Atividades Nível 02
### Atividade 2613

<img width="1095" height="317" alt="Image" src="https://github.com/user-attachments/assets/33b860b7-7ffb-4bf8-9009-a37ed4534aac" />

``` sql
SELECT
m.id,
m.name
FROM
movies m
JOIN
prices p ON m.id_prices = p.id
WHERE
p.value < 2.00;
```

### Atividade 2604

<img width="1086" height="307" alt="Image" src="https://github.com/user-attachments/assets/a91abfcc-8182-49f7-aa3e-904fe5f10ff6" />

``` sql
SELECT
	id, name
FROM
	products
WHERE
	price > 100 or price < 10;
```

## Atividades Nível 03
### Atividade 2606

<img width="1097" height="324" alt="Image" src="https://github.com/user-attachments/assets/f3d0bafe-aec5-4899-b230-af8f7e7c9c4f" />

``` sql
SELECT id, name
FROM products
WHERE id_categories IN (SELECT id FROM categories WHERE name LIKE '%super%');
```

### Atividade 2621

<img width="1216" height="349" alt="Image" src="https://github.com/user-attachments/assets/59951a79-311c-46b5-be77-aeb8c980ef71" />

``` sql
SELECT name
FROM products
WHERE amount BETWEEN 10 and 20
AND id_providers IN (SELECT id FROM providers WHERE name LIKE 'P%');
```

## Atividades Nível 04
### Atividade 2602

<img width="1094" height="318" alt="Image" src="https://github.com/user-attachments/assets/868038cc-c54f-4057-b3d9-a7344af6a380" />

``` sql
SELECT
	name
FROM
	customers
WHERE
	state = 'RS';
```
