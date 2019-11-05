# Exercise: Good Names
You’ve inherited some code from another programmer, who never had a chance to take the App Development with Swift course. All you found was a note with the following written on it:

Note:
Truck loading guide

Pallets of oranges weigh 100lbs

Pallets of watermelons weigh 200lbs

Have to load up the left then right of the truck and keep it as balanced as possible. How many on each side? Melons always go together.

``` swift
let co = 14
let cw = 3
let ow = 100
let ww = 200
let to = co * ow
let tw = cw * ww
let ttl = to + tw
let es = ttl / 2
let lhso = es / ow
let rhso = co - lhso
```

## Experiment
Rewrite the code so that it makes sense without needing a note. Use meaningful names and comments.

```swift
let countOrangePallets = 14
let countWatermelonPallets = 3
let orangePalletWeight = 100
let watermelonPalletWeight = 200
let totalOrangeWeight = countOrangePallets * orangePalletWeight // 1400
let totalWatermelonWeight = countWatermelonPallets * watermelonPalletWeight // 600
let totalWeight = totalOrangeWeight + totalWatermelonWeight // 2000
let eachSideWeight = totalWeight / 2 // 1000
let leftSideOrangePalletCount = eachSideWeight / orangePalletWeight // 10
let rightHandSideOrangePalletCount = countOrangePallets - leftSideOrangePalletCount // 4
```
