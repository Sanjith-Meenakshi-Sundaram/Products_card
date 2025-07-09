# Product_card
## Date:9/7/2025
## Objective:

To replicate a product card layout similar to those found on real-time e-commerce platform like FlipKart using the CSS Box Model (margin, border, padding, and content).

## Tasks:

#### 1. Structure the HTML Layout:
Create a container ```<div>``` for the product card.

Add an ```<img>``` for the product image.

Include ```<h2>``` for product name, ```<p>``` for description, and a ```<span>``` or ```<div>``` for price.

Add a “Buy Now” or “Add to Cart” button.

#### 2. Apply Box Model Styling in CSS:
Use padding inside each section (image, text, button) to ensure readability.

Use margin around the card to space it from the page edges or other cards.

Add a border to outline the card.

Control width and height for consistent sizing.

#### 3. Visual Styling:
Add a background color to the card container.

Use box-shadow to simulate depth (card lifting effect).

Add border-radius for rounded corners.

#### 4. Center the Card:
Use display: flex and justify-content: center and align-items: center on the parent container.

#### 5. Bonus Enhancements:
Use a hover effect on the button (e.g., background color change).

Make the card responsive with percentage-based widths or media queries.
## HTML Code:
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Product card</title>
  <link rel="stylesheet" href="color.css" />
</head>
<body>
  <div class="wrapper">
    <div class="card">
      <img src="https://iplanet.one/cdn/shop/files/iPhone_16_Plus_Black_PDP_Image_Position_1__en-IN.jpg?v=1727248891" alt="image" />
      <h2>Apple iPhone 16</h2>
      <p>Long Lasting 18hr battery</p>
      <div class="price">₹77,000</div>
      <button>Add to Cart</button>
    </div>
    <div class="card">
      <img src="https://iplanet.one/cdn/shop/files/iPhone_16_Plus_Black_PDP_Image_Position_1__en-IN.jpg?v=1727248891" alt="image" />
      <h2>Apple iPhone 16 Plus</h2>
      <p>Long Lasting 20hr battery</p>
      <div class="price">₹90,000</div>
      <button>Add to Cart</button>
    </div>
    <div class="card">
      <img src="https://inventstore.in/wp-content/uploads/2024/09/69-scaled.webp" alt="image" />
      <h2>Apple iPhone 16 Pro Max (256 gb)</h2>
      <p>Long Lasting 22hr battery</p>
      <div class="price">₹1,12,000</div>
      <button>Add to Cart</button>
    </div>
    
  </div>
</body>
</html>
```
## CSS Code:
```
.wrapper{
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
  background-color: lightyellow;
}
.card{
    width: 280px;
    background-color: #fff;
    border: 1px solid #ddd;
    border-radius: 10px;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
    padding: 16px;
    margin: 20px;
    box-sizing: border-box;
    text-align: center;
    transition: transform 0.3s;
}
.card:hover{
    transform: translateY(-5px);
}
.card img{
    width: 100%;
    height: auto;
    border-radius: 8px;
    margin-bottom: 12px;
}
.card h2{
    font-size: 20px;
    margin: 10px 0;
    color: #333;
}
.card p{
  font-size: 0.9rem;
  color: #555;
  margin-bottom: 10px;
}
.price{
  font-size: 1.1rem;
  color: #388e3c;
  font-weight: bold;
  padding: 8px;
}
.card button{
  background-color: #ff9f00;
  color: white;
  border: none;
  padding: 10px 18px;
  border-radius: 4px;
  cursor: pointer;
  transition: background-color 0.3s;
}
.card button:hover{
  background-color: #fb641b;
}
@media (max-width: 600px) {
  .card{
    width: 90%;
    margin: 10px;
  }
}

```
## Output:
![image](https://github.com/user-attachments/assets/6dcae248-00e8-44b5-b3c4-612f631e247d)


## Result:
A product card layout similar to those found on real-time e-commerce platform like FlipKart using the CSS Box Model is replicated successfully.
