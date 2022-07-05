1.https://github.com/rvsp/typescript-oops/blob/master/Practice/Movie.md
2.https://github.com/rvsp/typescript-oops/blob/master/Practice/class-circle.md
3.Write a “person” class to hold all the details.
4.write a class to calculate uber price.

Q 1) https://github.com/rvsp/typescript-oops/blob/master/Practice/Movie.md

A)   class Movie{
      constructor(title,studio,rating="PG"){
            this.title=title;
            this.studio=studio;
            this.rating=rating;  
         }
         getPG(movie){
            for(var i in movie){
                if(movie[i].rating==="PG"){
                    arr.push(movie[i].title);
                      }     
                               }
            return arr;
          }
       }
   const arr=[];
   var movie=[{title:"123",studio:"south",rating:"P"},{title:"1234",studio:"north",rating:"PG"},{title:"12345",studio:"west",rating:"PG"}]
   let movie1=new Movie(movie)
   console.log("Movies where rating=PG  "+movie1.getPG(movie))
   var movie2=new Movie("Casino Royale","Eon Productions","PG13")
   console.log("Title of movie is----->"+movie2.title+"Studio of movie is----->"+ movie2.studio+"Rating of movie is------>"+ movie2.rating)

Q 2) https://github.com/rvsp/typescript-oops/blob/master/Practice/class-circle.md

A)  class Circle{
    constructor(radius,color){
    this.radius=radius;
    this.color=color;
       }
    getRadius(){
          return this.radius
     }
    setRadius(newRadius){
         this.radius=newRadius
         
         return newRadius
     }
     getColor(){
         return  this.color
     }
     setColor(newcolor){
          this.color=newcolor
          return newcolor
     }
     getArea(){
         var pi=3.14
         var result=pi*Math.pow(this.radius,2)
         return result 
       }
     getCircumference(){
         var pi=3.14
         var result=2*pi*this.radius
         return result
       } 
    }
let radius=1.0
let color="red"
let c1=new Circle(radius,color)
console.log("Geting radius of the circle is-------> "+c1.getRadius())
console.log("Seting New radius of the circle is------->"+c1.setRadius(3.0))
console.log("Geting color-------> "+c1.getColor())
console.log("Seting New color-------> "+c1.setColor("black"))

let c2=new Circle(radius,color)
console.log("Getting Circle Area------>"+c2.getArea())
console.log("Getting Circle Circumference------>"+c2.getCircumference())


Q 3) Write a “person” class to hold all the details.

a)   class Person{
            constructor(name,phoneno,address,id){
                    this.name=name;
                    this.phoneno=phoneno;
                    this.address=address;
                    this.id=id;
               }
            getPerson(){
                  console.log("you get all the details   "+"name:-"+this.name+"       phoneno:- "+this.phoneno+"    address:-"+this.address+"    id:- "+this.id)
             }
            }
var details=new Person("Aziya","1234567890","Hyderabad","01")
details.getPerson()


Q 4) write a class to calculate uber price.

A)  class Uber{
               constructor(price,kilometer){
                    this.price=price
                    this.kilometer=kilometer
                    }
                  calculate(price,kilometer){
                        return price*kilometer
                      }
      }
var totalprice=new Uber(10,5)
console.log(totalprice.calculate(10,5))
