# Naming and Identifiers

# Swift Lesson 02
Lesson 02 - Naming and Identifiers

### Exercise: Putting on a Show
Your friend is done with the pet show. With your help, it was a big success. Now your friend is putting on a concert. Tickets are for sale at $10 per ticket. The room rental is $50. Making posters for the show costs $40. Help your friend figure out if the show is going to make money or lose money.

```swift
// Number Of Tickets
150

// Ticket Price
10

// Room Rental Fee
1000

// Poster Cost
40

// Total Ticket Value
150 * 10

// Total Expenses
1000 + 40

// Total Income Of Show
(150 * 10) - (1000 + 40)
```

### Exercise
Using the code above as a reference, use let statements to define constants to better solve your friend’s problem.
Add your code below. To help you get started, the constant ```numberOfTickets``` is already defined.

```swift
let numberOfTickets = 150
let ticketPrice = 10
let roomRentalFee = 50
let posterCost = 40
let totalTicketValue = numberOfTickets * ticketPrice
let totalExpenses = roomRentalFee + posterCost
let totalIncomeOfShow = totalTicketValue - totalExpenses

// The show will make money, because totalIncomeOfShow is greater than 0.
```

# Exercise: Lottery Tickets
Your friend’s entrepreneurial spirit knows no bounds. Now your friend is running the town lottery.

Another reason that naming things and only setting a value once is useful is that it lets you decide on the correct way of calculating something, then change the values and check the answers.

```swift
// Values you should edit
let ticketsSold = 1060
let ticketPrice = 2
let printingCosts = 10
let advertising = 40
```

### Exercise
You’ve done enough work for free for your friend. For this venture, your friend will give you a cut of the profits in return for your help. Your friend will give you a tenth of the profits. The jackpot is half of the total ticket sales money. Try changing the numbers above - tickets sold, ticket price, printing or advertising costs and see if you can get your cut up to 100 or more.

The calculations below are fixed, but you can change the results by changing the numbers above:

```swift
// Total takings
let totalTakings = ticketPrice * ticketsSold

// Jackpot
let jackpot = totalTakings / 2

// Expenses
let totalExpenses = printingCosts + advertising

// Profit
let profit = totalTakings - jackpot - totalExpenses

// Distribution
let programmersCut = profit / 10 // This is the answer you want to get over 100! 👉 
let friendsCut = profit - programmersCut
```

# Exercise: What Fits on Your iPhone?

In this exercise you’re going to work on figuring out the answer to the timeless question: How much stuff can I fit on my iPhone?

Unlike the previous exercises, no code will be provided. But here are a few things you’ll need to know:

* iPhone storage capacity is measured in gigabytes (GB).
* The iPhone in question has 8GB of storage.
* A gigabyte is about 1000 megabytes (MB)
* The phone already has 3GB of stuff on it
* One minute of video takes 150MB of storage

## Exercise

How many minutes of video will it take to fill the phone?
Hint: Do all of your calculations in megabytes (MB).

```swift
let phoneStorageGB = 8
let usedStorageGB = 3
let remainingPhoneStorageGB = phoneStorageGB - usedStorageGB
let remainingPhoneStorageMB = remainingPhoneStorageGB * 1000
let minuteVideoStorageMB = 150
let totalMinutesVideo = remainingPhoneStorageMB / minuteVideoStorageMB

// You will have 33 minutes of Video Left
```
# Exercise: Fixing Your Morning

There’s a lot to get done before you leave home in the morning. This exercise will help you optimize your routine.

## Exercise
Create a constant for each activity you do in the morning before leaving home: things like brushTeeth, uploadPhotos, chooseClothes, shower, goJogging, finishHomework, fixLunch, and so on. Think about how many minutes each activity usually takes, and assign that value to each constant.

```swift
let shower = 10
let clothes = 5
let brushTeeth = 2
let packStuff = 10
```

## Exercise
Find the total time of all the activities by adding up the constants. Try to adjust the values or add more activities until the total time looks reasonably close to the actual amount of time you spend getting ready on an average day.

```swift
let totalTimeMorningRoutine = shower + clothes + brushTeeth + packStuff
// 27 Minutes
```

## Exercise
Add up the constants again, but this time in separate groups: one group for things you have to do and another group for things you like to do.

If there are things you don’t have to do and don't like to do, make a third group and go ahead and sum that one, too. 

Make a new constant for each group.

```swift
let totalTimeMustDos = brushTeeth + clothes // 7
let totalTimeLikeDos = shower + packStuff // 20
let totalTimeToDos = totalTimeMustDos + totalTimeLikeDos // 27
```
See what happens to your total time spent getting ready if you tweak the durations of the different activities. How short of a shower would you have to take in order to have more time to message your friends? Or go for a longer run? How much more time would you need if you decided to spend as long as you wanted doing all the activities you like best?

Change the numbers until you’ve got a design for your ideal morning. What would have to change in order for you to be able to actually spend your morning time this way?

```swift
print("I would pack my stuff, the night before so, I can levae for Tech 7 minutes earlier")
```

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
