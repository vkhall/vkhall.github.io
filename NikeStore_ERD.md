```mermaid 
erDiagram 
	PRODUCT }o--o| SALE : creates
	PRODUCT {
		Product_ID PK
		Inventory_ID FK
		Shoe_Type
		Shoe_Style
		Color
		Size
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
