```mermaid 
erDiagram 
	PRODUCT }o--o| SALE : sold
	PRODUCT {
		string Product_ID PK
		string Inventory_ID FK
		string Shoe_Type
		string Shoe_Style
		string Color
		string Size
	}
	CUSTOMER ||--|{ SALE : buys
	CUSTOMER {
		string Customer_ID PK
		string FirstName
		string LastName
		string Phone_Number
	}
	SALE {
		string Receipt_ID PK
		string Date
		string Product_ID FK
	}
	INVENTORY |o--|{ PRODUCT : adjusted
	INVENTORY {
		string Inventory_ID PK
		string Product_ID FK
	} 
``` 
