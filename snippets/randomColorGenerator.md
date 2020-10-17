//Generates a random rgba color
const randColor = () => {
  let color = {
    r: Math.random(),
    g: Math.random(),
    b: Math.random()
  }
  //removes black color and sets it to white
  //you can also call the function again for a new color
  if (color.r == 0 && color.g == 0 && color.b == 0) {
    color = {
      r: 1,
      g: 1,
      b: 1
    }
  }
  return 'rgba(' + color.r * 255 + ',' + color.g * 255 + ',' + color.b * 255 + ')';
}
//assigns the randomly generated color to a variable
let myColor = randColor();
