# TypedArray

var data =
 'iVBORw0KGgoAAAANSUhEUgAAAAUAAAAFCAYAAACN' +
 'byblAAAAHElEQVQI12P4//8/w38GIAXDIBKE0DHx' +
 'gljNBAAO9TXL0Y4OHwAAAABJRU5ErkJggg=='
var characters = atob(data);
var array = new Uint8Array(characters.length);
for (var i = 0; i < characters.length; i++) {
 array[i] = characters.charCodeAt(i);
}
