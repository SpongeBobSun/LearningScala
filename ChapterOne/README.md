#Chapter One

###Scala ABC

Like other script languages such as `Ruby` & `Python`, Scala has a Command-Line-Interacton interface, called `scala`. After download & install scala, type `scala` in your terminal and there you go.

![scala-cli](./img/scala-cli.png =400x150)

###Semicolons
Semicolons are not required in scala. Thus, we don't need to write a semicolon at the end of our statement. Although, a semicolon wouldn't hurt.

If you do not understand why on earth we should put a semicolon at the end of your statement, that's fine. Ignore this part please.

###Variables

####Data Types

Scala has the same data type system as Java. We can use types such as 'String', 'Byte' like we are still in Java code. But, unlike Java, there are no basic data types such as 'int', 'float'. All data types are boxed as Object.

Check out Java's auto-boxing part for more informations if you never ever used a boxed type such as `Boolean`, `Integer` in Java.

####Let there be variable

First of all, it's not required to specify a data type for a variable.

There are two ways to define a variable in scala, `val` and `var`.

Variables declared by `val` are immutable. Otherwise, variables declared by `var` are mutable. So `val` actually means value, and `var` is short for variable like other scripts.

For example,

	var greeting = "Hi there"
	println(greeting)

is okay. But

	val greeting = "Hi there"
	greeting = "Welcome to the year 3000!"
	println(greeting)

will NOT work.

####Let there be function

Wanna a function? You got it.

	def MaxOf(x: Int, y: Int):Int{
		if (x > y){
			return x
		} else {
			return y
		}
	}

Function is declared by keyword `def`. After a `def` keyword you need name your function. Also, you need declare your function's parameters by wrapping them in brackets. Then is a colon followed by the data type your function will return. Last is your function body, wrapped by curly braces.

####Let there be scripts

Now we have introduced two things, variable and function. Although we don't know what are scala's best shots yet we can still write some thing to amuse ourselves. So you may think "Command Line Interaction Interface is stupid, I want a executable script file". Fine you got it. Write some thing in a text file and run `scala your-shiny-script-file.scala` and watch out for your output.
