# Interview-Questions

List of all interview questions for full stack developer

## System Design questions

1. Tell me about RESTful API [video](https://www.youtube.com/watch?v=-mN3VyJuCjM)
2. Tell me about GraphQl [video](https://www.youtube.com/watch?v=yWzKJPw_VzM)
3. RestApi vs Graphql [video](https://www.youtube.com/watch?v=yWzKJPw_VzM)
4. What happens when you type a URL into your browser? [video](https://www.youtube.com/watch?v=AlkDbnbv7dk)
5. How DNS resolution works? [answer](https://serverfault.com/questions/643506/how-does-the-http-get-method-work-in-relation-to-dns-protocol)
6. DNS over HTTP(S) [answer](https://en.wikipedia.org/wiki/DNS_over_HTTPS)
7. What is dns-prefetching [answer](https://developer.mozilla.org/en-US/docs/Web/Performance/dns-prefetch)
8. How to store passwords in the database? [video](https://www.youtube.com/watch?v=zt8Cocdy15c)
9. Why we need to add salt? Is my password less secure without salt? [answer](https://security.stackexchange.com/questions/100898/why-store-a-salt-along-side-the-hashed-password)
10. What is pepper? [answer](https://stackoverflow.com/questions/16891729/best-practices-salting-peppering-passwords)
11. What is CDN? What is Edge Server (Point of presense - not exactly the same)? [answer](https://www.youtube.com/watch?v=RI9np1LWzqw)
12. How scan to pay works? [video](https://www.youtube.com/watch?v=XS8ACikD2qs)
13. Where soap is mostly used? [answer](https://www.youtube.com/watch?v=4vLxWqE94l4)
14. Top 6 Most Popular API Architecture Styles [video](https://www.youtube.com/watch?v=4vLxWqE94l4)

## General questions

1. <div dir="rtl">איך היית רוצה להתקדם מבחינה מקצועית</div>

## JS questions

1. var vs let vs const
2. Hoisting
3. Prototype in js


### Promises


1. What the difference and results
```js
new Promise(function(resolve, reject) {
  setTimeout(() => {
    throw new Error("Whoops!");
  }, 1000);
}).catch(alert);
```

```js
new Promise(function(resolve, reject) {
  setTimeout(() => {
    reject(new Error("Whoops!"))
  }, 1000);
}).catch(alert);
```

```js
new Promise(function(resolve, reject) {
    throw new Error("Whoops!");
}).catch(alert);

```
```js
new Promise(function(resolve, reject) {
    reject(new Error("Whoops!"))
}).catch(alert);
```

<details>
There’s an "implicit try..catch" around the function code. So all <b>synchronous</b> errors are handled.

But here the error is generated not while the executor is running, but later. So the promise can’t handle it.
<summary>
Answer
</details>

### React js

1. Most common hooks in ReactJs
2. What will happen if yu use var/let instead of useState
3. Implement useMemo function
4. What is virtual dom
5. What is useCallback, when it's used and why

### Node js

1. What is middleware in Nodejs

### Web

1. How one can save data on client side
2. Post vs Pull
3. What the difference between scheme and protocol in URL? [answer](https://stackoverflow.com/a/65756683)

## Leetcode questions (from real interviews)

1. [200. Number of Islands](https://leetcode.com/problems/number-of-islands/) (_medium_) (_WIX_)
2. [706. Design HashMap](https://leetcode.com/problems/design-hashmap/) (_easy_) (_Similar Web_)
3. [843. Guess the Word](https://leetcode.com/problems/guess-the-word/) (_hard_) (_Google_)
4. [1160. Find Words That Can Be Formed by Characters](https://leetcode.com/problems/find-words-that-can-be-formed-by-characters/) (_easy_) (_WIX_)
5. [104. Maximum Depth of Binary Tree](https://leetcode.com/problems/maximum-depth-of-binary-tree/) (_easy_) (_Amazon_)
6. [520. Detect Capital
   ](https://leetcode.com/problems/detect-capital/description/) - With count of letters. (_easy_) (_Elbit_)

### GeekForGeeks Leetcode questions

1.  Given two unsorted arrays, find all pairs whose sum [link](https://www.geeksforgeeks.org/given-two-unsorted-arrays-find-pairs-whose-sum-x/?ref=ml_lbp)

## Not-language-related questions

1. יש 18 אבירים ונוכלים שיושבים סביב שולחן עגול.
   אביר תמיד דובר אמת ונוכל תמיד משקר
   כל אחד מהיושבים אמר שהוא יושב ליד אביר ונוכל
   כמה אבירים יושבים סביב השולחן?

2. sql vs nosql when to use
3. במטלה של ריאקט צריך לבנות קומפוננטת משחק זכרון של מדינות וערים שמוצגים בכפתורים, כשלוחצים על כפתור ראשון הוא אמור להיצבע בכחול וכשאר לוחצים על כפתור שני אם הכפתורים מייצגים את השילוב הנכון של ארץ ועיר בירה שני הכפתורים יצבעו בכחול ויעלמו מהמסך אם לא הם יצבעו באדום ויתהפכו שוב
4. יש 3 שעות לבנות משחק מחשב בעזרת javascript
   המשחק הוא לבנות עיגול במרכז המסך ולהשתמש בחיצים על מנת להזיז אותו ימינה שמאלה למעלה למטה.
   העיגול צריך להשאר בגבולות שהם מגדירים, וברגע שהוא מגיע לקצה עליו להפוך לאדום
5. מה קורה כשיוזר נכנס למערכת
6. בניית אפליקציית chat ב react
   מ eventים נתונים שמוכנים להבאת מידע
   הצגת מי כותב למשך 3 שניות או עד שמישהו אחר כותב

## Test questions

1. איזו סוג של טסטים אתה מכיר
2. איזה בדיקות היית כותב
