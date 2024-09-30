```mermaid 
erDiagram 
	PRODUCT }o--o| SALE :
	PRODUCT {
		Product_ID PK
		Inventory_ID FK
		Shoe_Type
		Shoe_Style
		Color
		Size
	}
	CUSTOMER ||--|{ SALE :
	CUSTOMER {
		Customer_ID PK
		FirstName
		LastName
		Phone_Number
	}
	SALE
	SALE {
		Receipt_ID PK
		Date
		Product_ID FK
	}
	INVENTORY |o--|{ PRODUCT :
	INVENTORY {
		Inventory_ID PK
		Product_ID FK
	} 
``` 
