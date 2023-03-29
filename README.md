# carcularFecha

```
function CalcularFecha() {
  let today = new Date();
  let dd = today.getDate();
  let mm = today.getMonth() + 1;
  const yyyy = today.getFullYear();
  let hora = today.getHours();
  let minute = today.getMinutes();
  let segundos = today.getSeconds();
  if (dd < 10) {
    dd = "0" + dd;
  }
  if (segundos < 10) {
    segundos = "0" + segundos;
  }
  if (hora < 10) {
    hora = "0" + hora;
  }
  if (minute < 10) {
    minute = "0" + minute;
  }

  if (mm < 10) {
    mm = "0" + mm;
  }
  //2018-05-15T16:00:00-06:00
  today =
    yyyy +
    "-" +
    mm +
    "-" +
    dd +
    "T" +
    hora +
    ":" +
    minute +
    ":" +
    segundos +
    "-06:00";

  return today;
}

console.log(CalcularFecha());
```
