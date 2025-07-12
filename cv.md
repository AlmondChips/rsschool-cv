# **Mikhail Savenko**

## Contacts
* Discord: almondchips
* Telegram: [Me](https://t.me/AlmondChips)
* Gmail: <chips6t@gmail.com>

## Summary

My main goal is to get better at programming in particular with which I could move confidently further as a developer. For me the priority is knowledge and experience.

One of my strengths is determination and well developed problem solving skill. In addition, I work quite well in a team.

I have no work experience in software development, but I have a great desire and inspiration to learn a lot of new things and stuff, which would help me to realize my passion in a real production projects.

## Skills
- **HTML/CSS** (Basics)
- **JavaScript** (Basics)
- **Python** (Basics)
- **C#** (Basics)
- **TypeScript** (Basics)
- **React** (Basics)
- **Redux** (Basics)
- **NodeJS** (Basics)
- **NestJS** (Basics)
- **GraphiQL** (Basics)
- **Docker** (Basics)
- **TelegramAPI** (Bots\user-bots) - capable to automate basic processes in Telegram
- **Webpack**
- **Vite**
- **SQL** (Basics)
- Relational database concepts of design and developing
- **WPF** technology

## Education
 Associate Degree in Information Systems\
 Krasnodar Information and Technology College, Krasnodar, Russia\
 Graduated: June 2023\
 Specialization: Design and Development of Information Systems\
 \
 Rolling Scopes School Front-end\React: 2022-2023

## English
According to the results of the test from [EnglishDom](https://www.englishdom.com/test-your-english-level/test/) my level of English is **B2(UPPER-INTERMEDIATE)**.

## Code example
My recent solution on Codewars to the [Number Of Carries](https://www.codewars.com/kata/58a6568827f9546931000027/javascript) kata:
```javascript
function numberOfCarries(a, b) {
  const nums = arguments;
  const stringified = []

  for (i = 0; i < nums.length ; i++) {
    stringified.push(String(nums[i]).split(''))
  }

  const [range1, range2] = stringified.map(n => n.length);

  if (range1 > range2)
     return countCarries(range1, range2, stringified, 1);
  else 
     return countCarries(range2, range1, stringified, 0);


}

function countCarries(range1, range2, strArr, index) {
    let counter = 0;

    const diff = range1 - range2;
    const newVal = new Array(diff).fill(0);
    newVal.push(...strArr[index]);
    strArr[index] = newVal;

    const numArrays = strArr.map(arr => arr.map(char => Number(char)));
    for (i = range1; i >= 0 ; i--) {
      const sum = numArrays[0][i] + numArrays[1][i];
      if (sum > 9) {
        counter++;
        numArrays[index ^ 1][i-1] += Math.floor(sum / 10);
      }
    }

    return counter;
}
```

## Educational projects
[Travel project](https://rolling-scopes-school.github.io/almondchips-JSFEPRESCHOOL2022Q2/travel/)\
![изображение](https://user-images.githubusercontent.com/94008966/188714655-c32ae314-9953-4767-b516-7e6328c94a07.png)

[Momentum clone](https://almondchips-momentum.netlify.app/)\
![изображение](https://user-images.githubusercontent.com/94008966/188715554-1c99d932-39ac-4473-99db-17bc9b3de139.png)

[Online Zoo](https://rolling-scopes-school.github.io/almondchips-JSFE2022Q3/online-zoo/pages/main/)\
![изображение](https://github.com/user-attachments/assets/a7d1ce7b-861f-4ff5-8560-3d740b41e0e0)

[Bird Song](https://rolling-scopes-school.github.io/almondchips-JSFE2022Q3/songbird/)\
![изображение](https://github.com/user-attachments/assets/1e2f5ce0-83b9-4b9d-bcb6-8b9aa6581d2a)

[Gem Puzzle](https://almondchips.github.io/Gem-puzzle/Gem-Puzzle/)\
![изображение](https://github.com/user-attachments/assets/c0bcd9fe-2439-41c1-8d92-ee5bd259936b)






