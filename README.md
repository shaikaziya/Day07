1.https://github.com/rvsp/typescript-oops/blob/master/Practice/Movie.md
2.https://github.com/rvsp/typescript-oops/blob/master/Practice/class-circle.md
3.Write a “person” class to hold all the details.
4.write a class to calculate uber price.

Q 1) https://github.com/rvsp/typescript-oops/blob/master/Practice/Movie.md

A)   class Movie{
      constructor(title,studio,rating="PG"){
            this.title=title;
            this.studio=studio;
            this.ratimg=rating;         
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
   var movie=[{title:"123",studio:"south",rating:"P",title:"1234",studio:"north",rating:"PG",title:"12345",studio:"west",rating:"PG"}]
   let movie1=new Movie(movie)
   console.log("Movies rating PG  "+movie1.getPG(movie))
   var movie2=new Movie(“Casino Royale”,“Eon Productions”,“PG­13”)
   console.log(movie2)
       

Q 2) https://github.com/rvsp/typescript-oops/blob/master/Practice/class-circle.md

A)  class Circle{
    constructor(radius,color){
    this.radius=radius;
    this.color=color;
       }
    getRadius(){
          return `Geting radius of the circle is-------> ${this.radius}`
     }
    setRadius(newRadius){
         this.radius=newRadius
         return  `Geting New radius of the circle is-------> ${newRadius}`
     }
     getColor(){
         return  `Geting color-------> ${this.color}`
     }
     setColor(newcolor){
          this.color=newcolor
          return  `Geting New color-------> ${newcolor}`
     }
     toString(){
          var value=`Getting toString-------> Circle[radius=${this.radius},color=${this.color}]`
          return value
       }
     getArea(){
         var pi=3.14
         var result=pi*Math.pow(this.radius,2)
         return `Getting Circle Area------>${result}` 
       }
     getCircumference(){
         var pi=3.14
         var result=2*pi*this.radius
         return `Getting Circle Circumference------>${result}` 
       } 
    }
let radius=1.0
let color="red"
let c1=new Circle(radius,color)
console.log(c1.getRadius())
console.log(c1.setRadius(3.0))
console.log(c1.getColor())
console.log(c1.setColor("black"))
console.log(c1.toString())

let c2=new Circle(radius,color)
console.log(c2.getArea())
console.log(c2.getCircumference())


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
var datails=new Person("Aziya","1234567890","Hyderabad","01")
datails.getPerson()


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
