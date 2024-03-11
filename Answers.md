1. Explain the relationship between the "Product" and "Product_Category" entities from the above diagram.
ans- The relationship between the "Product" and "Product_Category" is Many-to-One(M-1). The entities indicates that multiple products can belong to a single product category, but each product is associated
      with only one product category.
     For example- let's consider a scenario where you have a "Electronics" product category. Within the "Electronics" Product category, you can have multiple products like smartphones, laptops, and cameras.
      In this case, each of these products falls into the "Electronics" category, and the relationship is many products to one product category.

2. How could you ensure that each product in the "Product" table has a valid category assigned to it?
ans- To ensure that each product in the "Product" table has a valid category assigned to it, you can use a foreign key as a constraint. A foreign key is a field in a databse is used to link to the primary key
      of another table. In this context, you can create a foreign key in the "Product" table that references the primary key of the "Product_Category" table.
     For Example- The "Product_Category" table has a primary key "id"
                  The "Product" table has a foreign key "category_id" that references the "id" in the "Product_Category" table.
           By setting up this foreign key relationship, you ensure that each value in the "category_id" column of the "Product" table corresponds to a valid entry in the "id" column of the "Product_Category" table.
           This helps maintain referential integrity and ensures that each product is associated with a valid product category. If someone tries to insert or update a product with a non-existent category_id, it
           would violate the foreign key constraint and be rejected by the database.
