---
title: Nike Retailer
---
erDiagram
PRODUCT }|--|{ CUSTOMER : has
PRODUCT }
  string productName FK
  string productID PK
  string quantity
  string ratings
  string productAvailability
}
CUSTOMER }|--|| SALE : makes
CUSTOMER }
  string customerId PK
  string DOB
  string firstName
  string lastName
  string gender
  string emailAddress
  string purchaseHistory
}
SALE }|--|{ INVENTORY : needs
SALE }
  string productName FK
  string productInformation
  string saleId PK
}
INVENTORY one or more SALE : needs

## Brief Description of Entitities and their Relationships:

* Product Entity: This entity represents the Nike shoe product and has a one or more relationship to the Customer Entity.
* Customer Entity: This entity represents the consumer and has an only one to one or more relationship to the Sale Entity.
* Sale Entity: This entity represents the sale and has a one or more relationship to the Inventory Entity.
* Inventory Entity: This entity represents the retail store's Nike product inventory and has a one or more relationship to the Sale Entity.

## Relationships:

* The relationship between the Product and Customer is significant because it directly impacts a company's success by determining customer satisfaction, loyalty, and sales.
* The relationship between the Customer and the Sale is significant because it represents the core transaction that generates revenue for a business, and building a strong relationship with customers through effective sales practices can lead to repeat purchases, customer loyalty, positive word-of-mouth, and long-term business growth.
* The relationship between the Sale and the Inventory is significant because it directly impacts a business's profitability by indicating how efficiently they are managing their stock levels.
