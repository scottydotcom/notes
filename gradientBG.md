```css
background: linear-gradient(100deg, #e2b054ff, #88c588ff, #7176a3ff, #b6d0e2, #8fa9e0ff);
background-size: 400% 400%;
animation: animate 20s ease infinite;

@keyframes animate {
  0% {
    background-position: 0 50%;
  }
  50% {
    background-position: 100% 50%;
  }
  100% {
    background-position: 0 50%;
  }
}
```