# Web Design for a Manufacturing Company
## AIM: 
To design a static website for a chip manufacturing company.

## DESIGN STEPS:
### Step 1: 
Requirement collection.
### Step 2:
Creating the layout using HTML and CSS.
### Step 3:
Updating the sample content.
### Step 4:
Choose the appropriate style and color scheme.
### Step 5:
Validate the layout in various browsers.
### Step 6:
Validate the HTML code.
### Step 6:
Publish the website in the given URL.

## PROGRAM:

### base.html
```
{% load static %}
<!DOCTYPE html>
<html lang="en">

<head>
    <title>Quanton Private Limited</title>
    <link rel="stylesheet" href="{% static 'css/layout.css' %}">
    <link rel="icon" href="{% static 'img/titleicon.png' %}" type="image/x-icon">

</head>

<body>
    <div class="container">
        <div class="banner">
            <b> QUANTON PRIVATE LIMITED</b>
        </div>
        <div class="menu">
            <div class="menuitem"><a href="/home">Home</a></div>
            <div class="menuitem"><a href="/products">Products</a></div>
            <div class="menuitem"><a href="/people">People</a></div>
            <div class="menuitem"><a href="/contact">Contact Us</a></div>
        </div>
        <div class="content">
            {% block content %}
            {% endblock  %}
        </div>
        <div class="footer">
            Copyright © 2020 Quanton Private Limited, Developed by Harshini.
        </div>
    </div>
</body>

</html>
```

### home.html
```
{% extends "website/base.html" %}

{% block content %}
<div class="homecontent">
    <h1>About Us</h1>
    <img src="/static/img/building2.jpeg" alt="Building">
    <div class="contenttext">
        Silicon Pvt Ltd, provides a broad range of semiconductor and infrastructure software applications that serve the
        data center, networking, software, broadband, wireless, and storage and industrial markets. Common applications
        for its products include: data center networking, home connectivity, broadband access, telecommunications
        equipment, smartphones, base stations, data center servers and storage, factory automation, power generation and
        alternative energy systems, displays, and mainframe operations and management, and application software
        development. Some of Silicon's core technologies and products include:
        <ul>
            <li>Memory Chips</li>
            <li>SATA HDD</li>
            <li>SATA SSD </li>
            <li>Broadband Modems</li>
            <li>Wifi Devices</li>
            <li>Switching Devices</li>
            <li>Optical Sensors</li>
        </ul>
    </div>
</div>
{% endblock  %}
```
### products.html
```
{% extends "website/base.html" %}

{% block content %}
<div class="productcontent">
    <h1>Our Premium Products</h1>
    <div class="productitems">
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/c1.jpg" alt="product image">
            </div>
            <div class="itemname">4GB DDRA4 laptop memory</div>
            <div class="itemprice">Price: Rs.2000.00 </div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/c2.jpg" alt="product image">
            </div>
            <div class="itemname">1TB Laptop HDD</div>
            <div class="itemprice">Price: Rs.5000.00 </div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/img1.jpg" alt="product image">
            </div>
            <div class="itemname">Wireless Mouse</div>
            <div class="itemprice">Price: Rs.1500.00 </div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/img2.jpg" alt="product image">
            </div>
            <div class="itemname">1 TB External SSD</div>
            <div class="itemprice">Price: Rs.10,000.00 </div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/img3.jpg" alt="product image">
            </div>
            <div class="itemname">Wireless Modem</div>
            <div class="itemprice">Price: Rs.1500.00 </div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/img4.jpg" alt="product image">
            </div>
            <div class="itemname">Mobile WiFi Hotspot</div>
            <div class="itemprice">Price: Rs.2000.00 </div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/img5.jpg" alt="product image">
            </div>
            <div class="itemname">Optical Fingerprint Sensor Module</div>
            <div class="itemprice">Price: Rs.1700.00 </div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/img6.jpg" alt="product image">
            </div>
            <div class="itemname">64GB Memory Card</div>
            <div class="itemprice">Price: Rs.1000.00 </div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/img7.jpg" alt="product image">
            </div>
            <div class="itemname">64GB Flash Drive</div>
            <div class="itemprice">Price: Rs.3000.00 </div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/img8.jpg" alt="product image">
            </div>
            <div class="itemname">WiFi Smart Security Camera</div>
            <div class="itemprice">Price: Rs.2900.00 </div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/img9.jpg" alt="product image">
            </div>
            <div class="itemname">4K Pen Camera</div>
            <div class="itemprice">Price: Rs.4900.00 </div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/img10.jpg" alt="product image">
            </div>
            <div class="itemname">1080p Web Camera</div>
            <div class="itemprice">Price: Rs.2000.00 </div>
        </div>
    </div>
</div>
{% endblock  %}
```

### people.html
```
{% extends "website/base.html" %}

{% block content %}
<div class="productcontent">
    <h1>Meet Our People</h1>
    <div class="productitems">
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/p1.jpg" alt="product image">
            </div>
            <div class="itemname">CEO</div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/p2.jpg" alt="product image">
            </div>
            <div class="itemname">Manufacturing Head</div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/p3.jpg" alt="product image">
            </div>
            <div class="itemname">Project Manager</div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/p4.jpg" alt="product image">
            </div>
            <div class="itemname">Senior Engineer</div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/p5.jpg" alt="product image">
            </div>
            <div class="itemname">Finance Manager</div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/p6.jpg" alt="product image">
            </div>
            <div class="itemname">HR</div>
        </div>
    </div>
</div>
{% endblock  %}
```
### contact.html
```
{% extends "website/base.html" %}

{% block content %}
<h1>Reach Us</h1>
<ul>
    <li><b>Call Us :</b> +91 9832466007</li>
    <li><b>E-mail Us :</b> quanton@company.com</li>
    <li><b>Address :</b><br>

        <br>
        <ul style="list-style-type:square;">
            <li>
                <u>London Office :</u> <br>
                10 Downing Street<br>
                London<br>
                SW1A 2AA<br>
            </li>

            
            <li><u>California Office :</u><br>
                731 East Oxford Street<br>
                Chino<br>
                CA 91710
            </li>
        </ul>
    </li>
</ul>
{% endblock  %}
```


## OUTPUT:
![output](./static/img/out1.jpg)

![output](./static/img/out2.jpg)

![output](./static/img/out3.jpg)

![output](./static/img/out4.jpg)

## CODE VALIDATION REPORT:
![output](./static/img/out5 (2).jpg)

![output](./static/img/out6 (2).jpg)

![output](./static/img/out7 (2).jpg)

![output](./static/img/out8 (2).jpg)

## RESULT:
Thus a website is designed for the chip manufacturing company and is hosted in the URL http://harshini.student.saveetha.in:8000/. HTML code is validated.