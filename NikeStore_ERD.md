```mermaid 
erDiagram 
	PRODUCT |o--o| SALES 
	PRODUCT {
		PK Product_ID
		FK Inventory_ID
		Shoe_Type
		Shoe_Style
		Color
		Size
	} 
	CUSTOMER ||--|{ SALES
	CUSTOMER {
		PK Customer_ID
		FirstName
		LastName
		Phone_Number
	}
	SALE ||--|{ INVENTORY
	SALE {
		PK Receipt_ID
		Date
		FK Product_ID
	} 
	INVENTORY |o--|{ PRODUCTS
	INVENTORY {
		PK Inventory_ID
		FK Product_ID
	} 
``` 
