# Mooch's Batteries tests in Json format
This is a json file who stack every [Mooch's](https://www.e-cigarette-forum.com/blogs/mooch.256958/) tests for many batteries.

## Listed formats :
- 14500
- 18350
- 18500
- 18650
- 20650
- 20700
- 21700
- 26650

## How to parse ?
Datas using this format :
```javascript
{
    "FORMAT": {
        "MANUFACTURER": {
            "NAME": {
                "mah": {
                    "rated": float|null,
                    "tested": float|null
                },
                "cdr": {
                    "rated": float|null,
                    "estimated": float|null
                },
                "date": string|null,
                "dnb": true|false
                }
            }
        }
    }
}
```

### mah (capacity of each batter)
- **rated** is the value rated by the manufacturer (mAh)
- **tested** is the value found by Mooch during test (mAh)

### cdr (continuous discharge rating current)
- **rated** current value rated by the manufacturer (A)
- **tested** current value found by the Mooch during test (A)

### date
- format yy/mm/dd

### dnb : do not buy
- true if Mooch tells you do not buy this item, false otherwise
