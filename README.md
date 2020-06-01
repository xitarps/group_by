# Group by

```
function groupBy(objArray, atribute){

  find = objArray.reduce(function(total,item){

    let key = item[atribute];

    total[key] = (total[key] || []).concat(item)

    return total

  },{});

  return find
}

```