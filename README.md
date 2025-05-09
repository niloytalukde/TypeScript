1.Provide an example of using union and intersection types in TypeScript.

Ans:

intersection Example 
type person ={
    name:string,
    age : 18 
}
type voter ={
    isVoter:true
}
type voterPerson = person & voter

it's means that A person gave vote he/she fulfill the voterPerson type 

Union Example

type person ={
    name:string,
    age : boolean 
}
type voter ={
    isVoter:true
}
type student = person | voter

if a person admit to School or college he/she fulfill any type  

Explain the difference between any, unknown, and never types in TypeScript?
1.When declare a variable and declare this type any Then  user can input any type of value in this variable like string,number,boolean
2.Unknown and any type are similar  but You can't do anything with an unknown value until you assert its type
3.Use for functions that never return
