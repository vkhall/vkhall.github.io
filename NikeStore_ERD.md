```mermaid 
erDiagram 
	PRODUCT |o--o| SALE : to
	PRODUCT {
		PK Product_ID
		FK Inventory_ID
		Shoe_Type
		Shoe_Style
		Color
		Size
	}
	CUSTOMER ||--|{ SALE : to
	CUSTOMER {
		PK Customer_ID
		FirstName
		LastName
		Phone_Number
	}
	SALE
	SALE {
		PK Receipt_ID
		Date
		FK Product_ID
	}
	INVENTORY |o--|{ PRODUCT : to
	INVENTORY {
		PK Inventory_ID
		FK Product_ID
	} 
``` 
