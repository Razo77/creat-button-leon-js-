let increment = document.createElement("button");
let count = document.createElement("p");
let decrement = document.createElement("button");
const body = document.getElementsByTagName("body")[0];

increment.innerHTML = "-";
count.innerHTML = "0";
decrement.innerHTML = "+";

increment.textContent = "increment";
decrement.textContent = "decrement";

let num = 0;

increment.addEventListener("click", () => {
    num++;
    count.innerHTML = num;
});

decrement.addEventListener("click", () => {
    num--;
    count.innerHTML = num;
});

body.appendChild(increment);
body.appendChild(count)
body.appendChild(decrement);

