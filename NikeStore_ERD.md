```mermaid 
erDiagram 
	PRODUCT }o--o| CUSTOMER : to
	PRODUCT {
		string Product_ID PK
		string Inventory_ID FK
		string Shoe_Type
		string Shoe_Style
		string Color
		string Size
	}
	CUSTOMER ||--|{ SALE : to
	CUSTOMER {
		string Customer_ID PK
		string FirstName
		string LastName
		string Phone_Number
	}
	SALE |o--|{ PRODUCT : to
	SALE {
		string Receipt_ID PK
		string Date
		string Product_ID FK
	}
	INVENTORY {
		string Inventory_ID PK
		string Product_ID FK
	} 
``` 
