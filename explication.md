### Closures no React

```js

function Comment() {

  const [likes, setLikes] = useState(0);

  funtion addLike() {
    setLikes(likes + 1);
  }
}

Comment(props, 0)
```

## Sempre que for atualizar uma informação que vá receber um valor dela mesmo,

## é preciso fazer atualiazação padrão funções.

Ex:

function handleLikeComment() {
setLikeCount((state) => {
return state + 1;
})
}
function handleLikeComment() {
setLikeCount((state) => {
return state + 1;
})
}

- Dessa forma a cada click no aplaudir, irá somar duplicado.

---

## Typescript

`` Js
function sumAge(users) {
const sum = 0;

for (const user of users) {
sum += user.age;
}

return sum;
}

`` Typescript

interface User {
name: string;
bio: string;
age: number;
}

function sumAge(users: user[]) {
let sum = 0;

for (const user of users) {
sum += user.age:

}

return sum;
}

const sumOfAllUserAges = sumAge([
{
name: 'Jeison,
bio: 'Dev',
age: '37',
}
])
