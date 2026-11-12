# Data Dictionary

## customers
`customer_id` unique customer key; `age` customer age; `gender` gender label; `city` city; `state` state; `signup_date` signup date.

## products
`product_id` unique product key; `product_name` product name; `category` product category; `brand` brand; `selling_price` listed selling price; `cost_price` product cost.

## orders
`order_id` unique order key; `customer_id` customer foreign key; `order_date` transaction date; `payment_method` payment channel; `discount_pct` order discount percentage; `order_status` fulfilment status.

## order_items
`order_item_id` unique line key; `order_id` order foreign key; `product_id` product foreign key; `quantity` units; `unit_price` item selling price at transaction time.
