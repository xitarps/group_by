# Group by

## Javascript:
```
function groupBy(objArray, atribute){

  find = objArray.reduce(function(total,item){

    let key = item[atribute];

    total[key] = (total[key] || []).concat(item)

    return total

  },{});

  return find
}



JSON.stringify(cars.groupBy('year'), null, 4);

```

## Ruby:
```
grouped = cars.group_by { |car| car[:brand] }



JSON.pretty_generate(grouped)

```