'''function currency(strings,...values) {
  var str = "";
  for (var i=0; i<strings.length; i++) {
    if(i>0) {
      if (typeof values[i-1] == 'number') {
        str += values[i-1].toFixed(2);
      } else {
        str += values[i-1];
      }
    }
    str += strings[i];
  }
  return str;
}

var name = 'Robert';
var orderNumber = '1234';
var total = 317.3;

var msg = currency`Hello, ${name}, your \
order (#${orderNumber}) was $${total}.`;

console.log(msg);'''
