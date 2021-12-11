
## Run Locally



Install dependencies

```bash
  npm install
```

Start the server

```bash
  npm run serve-json
```


##  Commands
http://localhost:3000/products

http://localhost:3000/reviews

<!-- Finding by id -->
http://localhost:3000/products/1
<!-- Flitering -->
http://localhost:3000/products?category=electronics
<!-- Nested Filtering -->
http://localhost:3000/products?category=electronics&discount.type=shipping
<!-- Sorting -->
http://localhost:3000/products?_sort=price
<!-- Sorting by order -->
http://localhost:3000/products?_sort=price&_order=desc
<!-- Sorting by mutliple things -->
http://localhost:3000/products?_sort=price,category&_order=desc,asc
<!-- Pagination  -->
http://localhost:3000/products?_page=1&_limit=5

<!-- Operators (< lessthan), (> greaterthan) -->
http://localhost:3000/products?price_gte=2000&price_lte=4000

<!-- Not equal to operator -->
http://localhost:3000/products?id_ne=1

<!--  Like operator  (Eg: autocomplete component) -->
http://localhost:3000/products?category_like=^f

<!-- Full text search -->
http://localhost:3000/products?q=in
<!-- Parent - child realtionship -->
http://localhost:3000/products?_embed=reviews

<!-- Parent - child individule realtionship -->
http://localhost:3000/products/1?_embed=reviews
<!-- Child - parent realtionship -->
http://localhost:3000/reviews?_expand=product
<!-- Child - parent individule realtionship -->
http://localhost:3000/reviews/1?_expand=product

<!-- Post Request -->
For that we are going to using Thunder Client Extension in VS Code

- Make an a post Request
- Inside body json Content give an data like products

 <!--Crud operations  -->
 - We can perform CURD operations by using id

 <!-- Configuration -->
 - --port 4800
 <!-- Custom routes -->
 - --routes routes.json ({"/api/v1/*":"/$1"})
 <!-- Filter -->
 "/products/:category":"/products?category=:category"

 http://localhost:4800/api/v1/products/books

 <!-- Generate Random Data Packages -->
 - faker.js
 - casual
 - chancejs


## Demo



