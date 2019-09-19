# **Viktar Rudzenia**

## **Contact Info**

- E-mail: ViktarRudzenia@gmail.com
- Phone number: +375(33)390-13-57
- LinkedIn account: [ViktarRudzenia](https://www.linkedin.com/in/viktarrudzenia/)
- Telegram username: @ViktarRudzenia

## **Skills**

## **Experience**

### My profile in [codewars.com](https://www.codewars.com/users/Viktarrudzenia) : [![CodeWars](https://www.codewars.com/users/Viktarrudzenia/badges/large)](https://www.codewars.com/users/Viktarrudzenia)

My completed codewars challenges you can find [here](https://github.com/Viktarrudzenia/codewars "Completed CodeWars Challenges")

## **Code example**

Last favorite task which I complete in [codewars.com](https://www.codewars.com/ "codewars.com"): [Alphabet war - Wo lo loooooo priests join the war](https://www.codewars.com/kata/59473c0a952ac9b463000064 "Alphabet war - Wo lo loooooo priests join the war")

```javascript
function alphabetWar(fight) {
  // make array
  fight = fight.split("");

  //define objects with letters which fights
  let leftSideLetters = {
    w: [4, "m"],
    p: [3, "q"],
    b: [2, "d"],
    s: [1, "z"]
  };
  let rightSideLetters = {
    m: [4, "w"],
    q: [3, "p"],
    d: [2, "b"],
    z: [1, "s"]
  };
  // define sums of right and left sides
  let sumOfLeft = 0;
  let sumOfRight = 0;

  // Searching j and t priests and do magic things :) (replace i+1 and i - 1)
  for (let i = 0; i < fight.length; i++) {
    // "Magic" for leftSide
    if (fight[i] == "t") {
      if (rightSideLetters[fight[i - 1]] != undefined && fight[i - 2] != "j") {
        fight[i - 1] = rightSideLetters[fight[i - 1]][1];
      }
      if (rightSideLetters[fight[i + 1]] != undefined && fight[i + 2] != "j") {
        fight[i + 1] = rightSideLetters[fight[i + 1]][1];
      }
    }
    // "Magic" for rightSide
    if (fight[i] == "j") {
      if (leftSideLetters[fight[i - 1]] != undefined && fight[i - 2] != "t") {
        fight[i - 1] = leftSideLetters[fight[i - 1]][1];
      }
      if (leftSideLetters[fight[i + 1]] != undefined && fight[i + 2] != "t") {
        fight[i + 1] = leftSideLetters[fight[i + 1]][1];
      }
    }
  }

  // Calculate who wins
  for (let i = 0; i < fight.length; i++) {
    if (rightSideLetters[fight[i]] != undefined) {
      sumOfRight += rightSideLetters[fight[i]][0];
    }
    if (leftSideLetters[fight[i]] != undefined) {
      sumOfLeft += leftSideLetters[fight[i]][0];
    }
  }

  // decide who win this epic battle
  if (sumOfLeft > sumOfRight) {
    return "Left side wins!";
  } else if (sumOfRight > sumOfLeft) {
    return "Right side wins!";
  } else {
    return "Let's fight again!";
  }
}
```

## **Education**

## **English**
