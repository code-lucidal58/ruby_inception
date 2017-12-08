# Ruby_Novice
All you need to know to start about Ruby
 >Ruby is a general purpose language, commonly used in Rails applications.
 
 Ruby is interpreted (does not need a compiler). It is object-oriented and case-sensitive language. It does not require semicolon(:). Ruby doesn't care about whitespace. Hence no need to worry about indentations.
 Variables in Ruby are declared as:
 ```ruby
 my_number = 25
 my_boolean = true
 my_string = "Hello"
 puts my_number
 ```
 
 It supports simple mathematical operations like: + - * / % **

 There are two methods that are used to print on screen: _puts_ and _print_
. _print_ prints content as it is. _puts_ adds a new line to the content. There are no parentheses.
```ruby
print "Hello There"
puts "How are you?"
```

## Common Methods in Ruby
_.length_ is called on a string or string variable. It returns the length if the string.
```ruby
puts "Your_Name".length
```
_.reverse_ is called on a string or string variable. It returns the string in reverse order. It does not modify the original string.
```ruby
puts string_variable.reverse
```
_.downcase_ and _.upcase_ is used to return string in all lowercase and all uppercase respectively.
Multiple methods can be called in single line, one after the other.
```ruby
puts string_variable.upcase.reverse
```
_.capitalize_ capitalizes the first letter in the sentence and changes rest to lowercase.

*__Note:__* If a method is ended with exclamation mark(!), it modifies the original value of the varibale with the result.
```ruby
user_input.downcase!
```
_.include? "substring"_ checks if the variable has the substring. It returns boolean.
```ruby
if input.include? "hello"
    puts input
end
```
*__Note__*: As a general rule, Ruby methods that end with ? evaluate to the boolean values true or false.

_.gsub_ stands global substitution. It substitutes a substring with another. 
```ruby
user_input.gsub!(/s/,"th")
```
This replaces all 's' in the string to 'th'.

## Comments
Single line comments are written with hash(#) in the start. Multi-line comments start with _=begin_ and end with _=end_ .
```ruby
# This is a single line comment
=begin 
This is a
multiple line comment
=end
```

Local variables are written in all small letters separated by underscore. E.g. my_name, simon.
To get input from user, _gets.chomp_ is used.
```ruby
input1 = get.chomp
``` 
By default, Ruby adds a new line after input. _chomp_ removes that extra new line.

## String Interpolation
```ruby
monkey = "Curious"
print "I took #{monkey} to zoo"
```
Output will be: *I took Curious to zoo*
Notice, use double apostrophe(") to print the interpolated statement.

## Control Flow
_if_ and _elsif_ works in the same way as other languages.
```ruby
num = Integer(gets.chomp)
if num > 0
    print "Number is positive"
elsif num < 0
    print "Number is negative"
else
    print "Number is 0"
end
```
If elsif else block end with _end_.

The condition inside if should evaluate to _true_ for the block to be executed. In **_unless_** the condition should evaluate to _false_.
```ruby
hungry = false
unless hungry
  puts "I'm writing Ruby programs!"
else
  puts "Time to eat!"
end
```

There is another syntax of using _unless_ and _if_ which is similar to how we put conditions in our day-to-day conversations.
```ruby
jobNotDone = false
print 'Good work!!' unless jobNotDone
```

**Relational, Assigment and Comparison Operators** are same as for other common languages: = == > >= < <= !=
**Logical and Boolean operators**: && || !
Complex expressions can be created using these operators: E.g. *(x && (y || w)) && z*
Expressions in parentheses are always evaluated before anything outside parentheses.

