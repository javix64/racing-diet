# Racing-Diet

This app will use the API from [Open Food Facts](https://world.openfoodfacts.org/).

The main idea is get all the items that are on our stock, and do many recipes we can.

In the future i would like to add which recipe is better for a training-day(cardio, strength...)

Please feel free to colaborate in this project, and also if you see something wrong, just open an issue :)


## Structure

STOCK

```js
Stock={
    item:{
        expirationDate: Date,
        amount: Number,
    }
}
```

```js
Recipe={
    instructions: Array,
    portions: Number,
    preparationTime: Number,
    nutritionalScore: {
        kCal: Number, 
        fat: Number, 
        carbs: Number, 
        proteins: Number},
    ingredients: [
        {itemName: String, quantity: Number},
        ...
    ],
    variants: String,
    cookWare: [
        item1, item2]
}
```

```js
Ingredient={
    kCal: Number, 
    fat: Number, 
    carbs: Number, 
    proteins: Number,
    other: ...UNDERCONSTRUCTION
    }
```