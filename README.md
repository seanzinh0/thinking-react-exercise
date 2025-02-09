# Thinking in React
How is state and props working in the application?
State and props work in this application first when we have the filter products tables, this table takes in the products array as a prop to display and filter the products,
inside the table the searchbar and product table are rendered as components passing necessary information and state as props. For the search bar the state of filter text and inStock are being passed as props
along with their setters to handle any changes made. As for the product table it is taking the products that is passed through the filtered product table to display the products and also has the state of filterTet and inStockOnly passed as props to display the filtered products.
When we get deeper into the searchbar component it is taking the state from the filtered one and uses an onchange to see what items match the ones typed as well as a checkbox to see what is in stock. Lastly we have two helper components being product row and category row,
product row takes the product as props and destructures it to display if its stocked, the name and price. We also have the category row that takes the category as props to give a row of each category. When using these two components in the product table it allows us to map each one out and use object dot notation on the products thats passed as props to show each product.
