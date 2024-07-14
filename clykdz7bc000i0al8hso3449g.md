---
title: "Box Sizing and Box Model in CSS"
datePublished: Sat Jul 13 2024 17:14:06 GMT+0000 (Coordinated Universal Time)
cuid: clykdz7bc000i0al8hso3449g
slug: box-sizing-and-box-model-in-css
tags: css, beginner, html5, difference, concepts, self-taught, html-css, box-model, box-sizing, html-tags

---

#### Box Model

The CSS Box Model is essential for web design and layout, detailing how elements are structured and spaced:

1. **Content**: The element's actual content.
    
2. **Padding**: Space between the content and border.
    
3. **Border**: Surrounds the padding and content.
    
4. **Margin**: Space outside the border, separating the element from others.
    

```xml
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Box Model Example</title>
    <style>
        .box {
            width: 200px;
            height: 100px;
            padding: 20px;
            border: 5px solid blue;
            margin: 15px;
            background-color: rgb(141, 39, 39);
        }
        .content {
            background-color: white;
            height: 100%;
        }
    </style>
</head>
<body>
    <div class="box">
        <div class="content">
            This is a box model example.
        </div>
    </div>
</body>
</html>
```

**Output**

![Output](https://cdn.hashnode.com/res/hashnode/image/upload/v1720890602991/4b932886-1fd5-4293-9463-d3b625b25e52.png align="center")

---

#### Box Sizing

The `box-sizing` property specifies how the width and height of an element are calculated:

1. **Content-box** (default):
    
    * Width and height include only the content.
        
    * Padding and border are added outside the content area.
        
2. **Border-box**:
    
    * Width and height include content, padding, and border.
        
    * Helps maintain the element's overall size.
        

#### Visual Example

* **Content-Box**: `width: 300px` means the content is 300px wide, with padding and border added outside.
    
    ```css
    .box-content {
        width: 300px;
        padding: 20px;
        border: 10px solid green;
        box-sizing: content-box; /* default */
    }
    ```
    
* **Border-Box**: `width: 300px` includes content, padding, and border.
    
    ```css
    .box-border {
        width: 300px;
        padding: 20px;
        border: 10px solid blue;
        box-sizing: border-box;
    }
    ```
    

```xml
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Box Sizing Example</title>
    <style>
        .box-content {
            width: 300px;
            padding: 20px;
            border: 10px solid green;
            margin: 10px;
            background-color: lightgray;
            box-sizing: content-box; /* default */
        }

        .box-border {
            width: 300px;
            padding: 20px;
            border: 10px solid blue;
            margin: 10px;
            background-color: lightcoral;
            box-sizing: border-box; /* includes border and padding in the width */
        }
    </style>
</head>
<body>
    <h2>Box Sizing Example</h2>
    <div class="box-content">
        Content-box: Width includes only the content.
        
    </div>
    <div class="box-border">
        Border-box: Width includes border and padding.
    </div>
</body>
</html>
```

**Output**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1720890573752/b54df2d8-1a0e-4821-999d-83212d227b2d.png align="center")

---

#### Summary

* **Box Model**: Defines element structure and spacing (content, padding, border, margin).
    
* **Box Sizing**: Determines whether width/height calculations include padding and border.