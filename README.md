# Mooch's Batteries tests in Json format
This is a json file who stack every [Mooch's](https://www.e-cigarette-forum.com/blogs/mooch.256958/) tests for many batteries.

## Listed formats :
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

## Datas from
![18650](https://www.e-cigarette-forum.com/attachments/ac3d9019-786f-4287-9c2e-ba7f4e47a520-jpeg.942737/)

![2xxx](https://www.e-cigarette-forum.com/attachments/2a6aeae8-be9b-432a-a774-cb99414e2d41-jpeg.943265/)