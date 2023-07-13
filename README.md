# Variants as Products Shopify
This code snippet aims to display variants as separate items in the collection of your Shopify store. This has been tested on Dawn Theme v.7.0.1

Instructions:
1. Open your theme's code and the file `main-collection-product-grid.liquid`
2. Look for `{%- for product in collection.products -%}` and replace the existing code with the provided code, making sure to stop before the closing </ul> tag
3. Go into the Snippets directory of your code and create a new file called "card-variant"
4. Copy/paste the provided code
5. You're done !


Additionnal info: if you want to display the original product and its variants in the collection list, remove this line and its closing statement: 

 `{% if product.variants.size == 1 %}`

It's also recommended to go into your `component-card.css` to add the property `z-index: 1;` to the class `.card__badge` (otherwise the image goes in front of the Sold Out/Sale badge).
