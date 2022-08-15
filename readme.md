# Just a client side validation

This is a client side validation. 

## .New 🌚
[x] Regex 
: Regular Expression.

```html
<input type="tel" id="phone" placeholder="09123456789" required pattern="[0-9]{11}">
```

`pattern="[0-9]{11}"` ensures that there are eleven characters between 0 and 9

```html
<input type="tel" id="phone" placeholder="900-111-2221" required pattern="[0-9]{3}-[0-9]{3}-[0-9]{4}">
```
`pattern="[0-9]{3}-[0-9]{3}-[0-9]{4}"` will ensure that the first 3 digits are between 0 and 9 and is preceeded with an hyphen (-) and the next 3 digits are also between 0 and 9, then also followed by an hyphen (-), then the last 4 digits are also between 0 and 9

```html
<input type="password" id="password" placeholder="Create Password" required pattern="^(?=.*\d)(?=.*[a-z])(?=.*[A-Z])(?=.[a-zA-Z]).{8,}$">
```

`pattern="^(?=.*\d)(?=.*[a-z])(?=.*[A-Z])(?=.[a-zA-Z]).{8,}$"` ensures that there is at least 1 uppercase character, 1 lowecase character and 1 number. And input is not less than 8 characters