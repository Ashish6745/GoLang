// You can edit this code!
// Click here and start typing.
package main

import "fmt"

type person struct {
	name string
	age  int
}

func main() {
	// this is single line comment

	// This is multi-line comment
	/*
		// data types
		var a int = 2                      // this is integer type
		var b string = "hello Go-Language" // this is string type
		var c float32 = 3.22               // this is float type
		var d bool = true                  // this is boolean type
		fmt.Println(a)
		fmt.Println(b)
		fmt.Println(c)
		fmt.Println(d)
	*/

	// defining multi variables of same type on same line

	//var a, b int = 3, 4
	//fmt.Println(a, b)

	// defining multiple variables

	//var (
	//a int    = 2
	//b int    = 4
	//c bool   = true
	//d string = "GoLanguage"
	//)
	// multi-word variable
	// camecase
	//var myName = "MARK WOOD"
	// pascalcase
	//var LastName = "JosButlter"
	// snake_case
	//var my_home_town = "LOS ANGELES"

	//fmt.Println(myName)
	//fmt.Println(LastName)
	//fmt.Println(my_home_town)

	// CONSTANTS IN GO LANGUAGE

	//const Pi = 3.14
	//fmt.Println(Pi)
	// There are two types of constant in go 1] Typed and 2] Untyped
	//const a int = 1 // Typed
	//const b = 2     // Untyped
	//fmt.Println(a, b)

	// Defining multiple constants

	const (
		c int    = 4
		d string = "hello constant"
	)
	fmt.Println(c, d)

	// Arrays in GoLanguage
	//var myArray = [5]string{"mango", "apple", "banana"}
	//fmt.Println(myArray)
	// finding the length of array
	//var myArray = [6]int{1, 2, 3, 4, 5, 6}
	//fmt.Println(len(myArray))  // 6 length of array

	// Changing and adding  the element in an array

	//var cost = [5]int{1, 3, 4, 7}
	//cost[2] = 5 // element changed
	//cost[4] = 9 // element add
	//fmt.Println(cost)

	// Array initialisation

	//var arr = [5]int{}      // not intialised
	//var arr2 = [5]int{1, 2} // partially intialised
	//var arr3 = [5]int{1, 2, 3, 4, 5}
	//var str = [2]string{"mark"}
	// The default value for int is zero and string is ""
	//fmt.Println(arr)  //[0,0,0,0,0] because nothing present inside arr
	//fmt.Println(arr2) //[1,2,0,0,0] only first 2 values are there
	//fmt.Println(arr3) // [1,2,3,4,5] all values are present
	//fmt.Println(str) // for string default values is empty string

	// slice It is similar to array but more powerful and flexible
	// Note :- It works similar to the slice method in JS

	//mySlice := [4]int{1, 3, 4, 5}
	//mySlice2 := mySlice[0:3] // cutting the slice from slice1
	//fmt.Print(mySlice2)

	// Operators in GoLanguage

	// Arithmetice operators
	//var num1 int = 20
	//var num2 int = 10

	//fmt.Println(num1 + num2) // Addition operator
	//fmt.Println(num1 - num2) // Subtraction operator
	//fmt.Println(num1 * num2) // Multiplication operator
	//fmt.Println(num1 / num2) // Divison
	//fmt.Println(num1 % num2) // Modulus

	// Assignment Operators and comparison operators These operators returns true/false
	//fmt.Println(num1 == num2) // Equal to  [false]
	//fmt.Println(num1 != num2) // Not Equal [true]
	//fmt.Println(num1 > num2)  // Greater than [true]
	//fmt.Println(num1 >= num2) // Greater than or equal to [true]
	//fmt.Println(num1 < num2)  // Less than [false]
	//fmt.Println(num1 <= num2) // Less than or equal to [false]
	//num2 += 4
	//fmt.Println(num2)
	//num1 -= 5
	//fmt.Println(num1)
	//num1 *= 10
	//fmt.Println(num1)
	//num1 /= 20
	//fmt.Println(num1)

	// LOGICAL OPERATOR
	//fmt.Println(num1 > 10 && num2 < 30) // AND Operator && returns true when both conditions are true
	//fmt.Println(num1 > 10 || num2 < 20) // OR Operator || returns true when any of the one condition is true
	//fmt.Println(!(num1 > 10 || num2 < 20)) // NOT Operator reverse the result true -> false vice versa

	// IF and IF-ELSE AND ELSE-IF STATEMENTS ARE CONDITIONAL STATEMENTS
	var x int = 25
	// IF statement
	//if x > 10 {
	//	fmt.Println("x is greater than 10")
	//}

	// IF-ELSE STATEMENT
	if x > 10 {
		fmt.Println("x is greater than 20")
	} else {
		fmt.Println("x is less than 10")
	}
	// ELSE-IF STATEMENT

	if x > 10 {
		fmt.Println("X is greater than 10")
	} else if x > 20 {
		fmt.Println("x is greater than 20")
	} else {
		fmt.Println("x is negative")
	}

	// switch case in GoLanguage : In GoLanguage there is no break statement after each case only default value is there

	var day int = 1
	switch day {
	case 1:
		fmt.Println("Its monday")
	case 2:
		fmt.Println("Its Tuesday")
	case 3:
		fmt.Println("Its Wednesday")
	case 4:
		fmt.Println("Its Thrusday")
	case 5:
		fmt.Println("Its Friday")
	case 6:
		fmt.Println("Its Saturday")
	case 7:
		fmt.Println("Its Sunday")
	default:
		fmt.Println("Invalid Day")

	}

	// MULTI-CASE SWITCH STATEMENT
	switch day {
	case 1, 3, 5:
		fmt.Println("odd week day")
	case 2, 4, 6:
		fmt.Println("even week day")
	default:
		fmt.Println("Weekend day")
	}

	// FOR LOOP
	var i int
	var j int
	for i = 0; i < 10; i++ {
		fmt.Println(i)
	}
	// NESTED FOR LOOP

	for i = 1; i < 5; i++ {
		for j = 1; j < 5; j++ {
			fmt.Print("*")
		}
		fmt.Println("")
	}

	// Continue statement :- It skips the current iteration and jumps over to the next iteration

	// Break statement :- It termates or stops the iteration

	// Functions are used to use the code repeatedly

	//func add(a int, b int) int {
	//a =5
	//b = 5
	//return a + b
	//}

	//add()

	// Struct are used to create a collection of members of different types into a single variables

	//var man person
	//man.name = "John"
	//man.age = 24

	//fmt.Println(man.name)
	//fmt.Println(man.age)

	//Map are used to store date in a key value pair
	// It does not duplicate values
	// Default value of map is nill

	var a = map[int]string{1: "one", 2: "two"}
	fmt.Println(" ", a)
	// You can also define a map using Make function

	var b = make(map[int]string)
	b[1] = "mark"
	b[2] = "wood"
	fmt.Println("", b)

	// deleting a key in b Map using delete() function

	delete(b, 1)
	fmt.Println("after deletion", b)
	
	// Maps are pass by value if two maps are pointing to same hash table and if something is changed in one map then the change will be reflected on both of the maps
	
	
}
