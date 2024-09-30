```mermaid 
erDiagram 
	PRODUCT }o--o| CUSTOMER : to
	PRODUCT {
		Product_ID PK
		Inventory_ID FK
		Shoe_Type
		Shoe_Style
		Color
		Size
	}
	CUSTOMER ||--|{ SALE : to
	CUSTOMER {
		Customer_ID PK
		FirstName
		LastName
		Phone_Number
	}
	SALE |o--|{ PRODUCT : to
	SALE {
		Receipt_ID PK
		Date
		Product_ID FK
	}
	INVENTORY {
		Inventory_ID PK
		Product_ID FK
	} 
``` 
