# CocktailDatabase
A cocktail database in JSON format

# Usage
The usage is very simple. I assume that you will create an object from this json named (for example db).

With db.***cocktail*** ( __Where of course ***cocktail*** is the name of your cocktail__ ) you can access some properties of it. 
> ***PROPERTIES***

**Ingredients** ``` with ingredients --> {ingredients:quantities}```

**Type of Glass** ``` with glass --> String```

**Decorations** ``` with decoration --> String or [Strings]```

**Category(like pre/after dinner/launch)** ``` with type --> String```

**Method(miscelating type)** ``` with method --> String```

**Long/Medium/Short Drink** ``` with category --> String```

There's also an all_ingredients property --> {alcholic,nonalcholic} 
showned after 

# SAMPLE OUTPUT

```
db.vodka_sour.ingredients 

{
  vodka: '45 ml',
  simple_syrup: '15 ml',
  lemon_juice: '30 ml',
  bitter: '3 drop',
  egg_white: '15 ml'
}
```
```
db.vodka_sour.ingredients.simple_syrup

'15 ml'
```

```
db.bloody_mary.method

'Shake & Strain'
```

```
db.all_ingredients

{
  alcholic: [
    'Vodka',
    'White_Rum',
    'Golden_Rum',
    ...]
  non_alcholic: [
    'Lemon_Juice',
    'Water',
    'Soda',
    ...]
}
