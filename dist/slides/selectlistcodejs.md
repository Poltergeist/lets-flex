##  selectListCode

```
var items = document.querySelectorAll('.item');
items = Array.prototype.slice.call(items);

function clickHandler(event){
  var target = event.target;
  if ( target.classList.contains('active') ){
    target.classList.remove('active');
    return;
  }
  target.classList.add('active');
};

items.forEach(function(item){
  item.addEventListener('click', clickHandler)
});
```
