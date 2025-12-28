method 1:

```css
// glassmorphism affect
box-shadow: 20px 20px 50px rgba(0, 0, 0, 0.25);
border-top: 1px solid rgba(255, 255, 255, 0.5);
border-right: 1px solid rgba(255, 255, 255, 0.5);
backdrop-filter: blur (8px);
-webkit-backdrop-filter: blur(8x) ;

// glassmorphism affect v2
background: linear-gradient(135deg,
 rgba(255, 255, 255, 0.1),
 rgba(255, 255, 255, 0));
-webkit-backdrop-filter: blur (20px);
backdrop-filter: blur(20px);
box-shadow: 0 8px 32px 0 rgba(0, 0, 0, 0.37);
border: 1px solig rba(255, 255, 255, 0.18);
border-radius: 32px:
```

method 1.a:

```css
background: rgba(255, 255, 255, 0.25);
box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.37);
backdrop-filter: blur(4px);
-webkit-backdrop-filter: blur(4px);
border-radius: 10px;
border: 1px solid rgba(255, 255, 255, 0.18);
```

method 2:

```css
background: rgba(255, 255, 255, 0.2);
border-radius: 16px;
box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
backdrop-filter: blur(5px);
-webkit-backdrop-filter: blur(5px);
border: 1px solid rgba(255, 255, 255, 0.3);
```

method 3:

```css
backdrop-filter: blur(16px) saturate(180%);
-webkit-backdrop-filter: blur(16px) saturate(180%);
background-color: rgba(17, 25, 40, 0.75);
border-radius: 12px;
border: 1px solid rgba(255, 255, 255, 0.125);
```

method 4

```css
background: rgba(255, 255, 255, 0.4);
box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.37);
backdrop-filter: blur(5px);
-webkit-backdrop-filter: blur(5px);
border-radius: 10px;
border: 1px solid rgba(255, 255, 255, 0.18);
``