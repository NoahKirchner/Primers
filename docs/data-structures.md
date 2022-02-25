# Fundamentals
{: style="border-bottom: none;margin-bottom:0"}

### Data Structures
{: style="margin-top:0"}
[Home](https://noahkirchner.github.io/Primers/) | [Github](https://github.com/NoahKirchner/Primers)
## Overview


Data structures are the various means by which information is stored, communicated and acted upon. Fundamentally
they are numerical representations of information stored in a standardized way such that the data can be 
interpreted by the computer and reconstructed for the user. This information can range from a single, one digit
number to an entire movie which can then be transferred and reconstructed to reform the original information.


In the case of computing, this occurs through a base two number system called binary. Consequentially, all
data that your computer stores and uses is represented by a one or a zero at the lowest level. Understanding
how computers interpret and store this information is crucial to advanced usage.


## Number Systems


Number systems are the various means by which numbers are represented. In normal life,
the most commonly used number system is the base ten number system, also known as decimal. It contains
numbers zero through nine, meaning that the decimal system is comprised of ten total digits. While this
may be the most common number system, it is not the only number system, and theoretically you could have
a number system that contains five digits, one hundred digits or as many or few as you can create symbols
for. In the case of computation, however, there are four primary number systems used to store and process
data.


### Decimal


Decimal is the most common number system in daily life. As previously mentioned, it is comprised
of ten digits, including zero. The number system iterates up from zero until nine, and then when 
a number is needed that is larger than nine, a one is added at the beginning of the number and the
value carries over to the left. For each time the rightmost number is iterated past nine, the left
number is iterated by one until the left number hits nine, at which point the process continues 
into the hundreths place. This idea of values carrying over is critical to understanding how alternate
number systems work.


### Binary


Binary is the number system that digital data is inevitably transformed back into before it is
manipulated by the processor. It is the purest form of data in computing and it is critical to understand.
Binary, like Decimal, operates using the same system of carrying over. The difference is that instead of nine,
the number that causes value to carry over into the next spot is a one. This gives binary two usable digits,
zero and one, and whenever the value of the right digit is iterated past one, the one carries over into the left
place. This process, just like with decimal, continues as the length in digits of the number gets larger and 
larger.


### Hexadecimal


Hexadecimal is the second most popular number system in computing because of its use in representing bytes
(more on that later). Hexadecimal, or coloquially hex, contains more potential digits than decimal does, and
those non arabic numbers are represented by the letters A through F. As the rightmost number increases past
nine, it carries on into A, B, C, D, E and F, which are equal to ten through fifteen. After a value greater
than fifteen (or F) needs to be represented, a one is added to the left place and the rightmost digit is
reset to zero.


## Digital Units


Computers store their information through the use of binary numbers. These numbers can represent anything to
characters, colour data or other abstract information. Everything on the computer is represented at the lowest
level through a binary number. While this is the form that the computer computes in, the binary data may
be abstracted into other number systems for the purposes of simplicty and user readability, such as hexadecimal
or octal formats.


### Bit


Bits are one digit binary numbers and they are the smallest digital unit. When alone, they represent a
state of either on or off, like a switch. This can be used to represent any decision which only has
two options, such as whether or not a computer is on or off or whether a person is male or female.


### Nibble


A nibble is a collection of four bits. This is rarely used today aside from for niche circumstances, such
as rounding decimals, but it is notable because each individual hexadecimal character can represent a single
nibble of data. One nibble can represent a full value of 0 to 128.


### Byte


A byte is a collection of eight bits or two nibbles. They are the primary digital unit when it comes 
to representing data, as a byte is conveniently sized to represent a single character. One individual
byte can represent a value from 0 to 255. They can be thought of as the smallest significant digital unit
due to their flexibility in what they can represent, and this is why they are the most common type you will
likely come across. A byte is represented, generally, by two hexadecimal characters.


### Word


Words are collections of bytes all combined together into one digital unit. The size of each word is dependent
on the specific processor architecture. The purpose of words is to allow bytes to give context to other bytes,
allowing them to represent far more varied and detailed types of information. Words are generally the smallest
digital units that processors will hold in memory. While processors do math using individual bits, it does it
using the context provided by the bytes and words that the bits are a part of.


### Blocks


Much as words are collections of bytes, blocks are collections of words. They are a set size, and arge used to
conveniently store and reference larger amounts of information. Processors do not operate on blocks of data
at a time, but they generally have blocks of data cached so that they can easily access the words contained
within them.


## Data Interpretation


Computers are not able to interpret abstract information. All of their operations, and by extension all
everything that the user sees, boils down to arithmetic performed on binary numbers.


### Storage


Conceptually, data stored on a drive can thought to be stored ona giant tape. Each space on this tape has
either a one or a zero on it, and these spaces are also numbered from zero to however long the tape is.
Information can be accessed starting at any point on the tape and read data from that starting point
for any specific number of spaces. This is how information is stored, both in memory and in long term storage,
and this stream of bits is also how the computer makes references to specific points of data. The one or
zero stored on the tape is the data, and the number on the tape is generally referred to as an address.


### Manipulation


Computers receive their instructions in the form of bits organized into words. These binary words, when
interpreted by the process, are capable of modifying data that is stored within memory and on the drive.
Using the analogy from before, the process can be thought to look at a set number of spaces on the tape
each time it decides to perform a new action. From there, it splits the values that it interpets up into
different temporary storage locations called registers. Some of this data is meant to be manipulated, and
other parts of the data is made to represent instructions for the processor. There is also data that is
purely meant to point to other areas in emory or storage that need to be pulled into the processor. The 
processor then performs the necessary actions using the instructions and data provided.


## Data Types


The data that programs interact with is far more abstracted than the type of data handled at the processor level.
The processor deals only with binary numbers organized into words, but through their organization and various
different standards these bits and bytes are interpreted as different types of data which represent various
flavors of information. Numbers and letters, for example, are distinct types of data, and so high level
programming language will require you to distinguish the two from each other. These data types are distinct
because at the byte level they are all represented in different ways with different standards.


### Integers


Integers represent whole numbers. Their size is limited by the maximum value that a digital unit can represent.
Generally, they come in three different sizes. Shorts, default and longs, all of which are represented
by differently sized digital units and thus all have different maximum values. By default, integers cannot
be negative. To represent a negative number, an integer needs to be "signed" with a bit at the beginning
of the byte. This decreases the maximum possible value of the integer, but also gives it an identifier
as to whether or not the number is negative or positive.


### Characters


Characters represent a single linguistic character. While this character could technically be a digit, in
most programming language you would not be able to perform arithmetic on this character because it is not
technically a number. More than one character, such as if you are attempting to write a word, would have
to be grouped together into an array (more on those later). An array of characters is generally referred
to as a character array or a string.


### Booleans

A boolean can be conceptualized as a switch. They have two values, much like a single bit. They can either
represent true or false, on or off, so on and so forth.


### Floating Point Numbers


Floating point numbers, also called floats, are numbers which contain a decimal. Like integers, they can
be classified into short or long variants, and can be signed to represent negative values. Unlike integers,
they tend to be larger and are also less accurate due to rounding errors for very specific values.


### Pointers


A pointer is a type of data that contains a memory or storage address which points to another piece of memory.
This allows you to directly reference the memory in this location, even if you do not know what is contained
there at the time.


### Arrays


Arrays are a data type that contain a list of pointers to other pieces of data. In the abstract, it can
be interpreted as a list of data. Arrays are usually only able to contain information of the same type. So
for example, an array could not contain characters and integers together. Arrays are iterable, meaning that
they can be moved through one object at a time and have an action performed on each object in sequence.







---
Noah Kirchner
