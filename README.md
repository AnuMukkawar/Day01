# Day01

Q1. What is the difference between statically typed and dynamically typed languages?

Ans:
A programming language is statically typed if the type of a variable is known at compile time. A language is dynamically typed if the type of a variable is checked during run-time.

Statically-Typed Languages-
        We call a language “statically-typed” if it follows type checking during compilation. So, every detail about the variables and all the data types must be known before we do the compiling process.
        In this type of language, once a variable is assigned a type, it can’t be assigned to some other variable of a different type. If we try to do so, the compiler will raise some errors, and we need to fix them. Hence, for a declared variable, the data type is fixed.
        Some examples of statically-typed languages are Java, C, C++, C#, Swift, Scala, Kotlin, Fortran, Pascal, Rust, Go, COBOL, etc.
        One great thing about statically-typed languages is that we’ll be able to fix a lot of errors even before running the program. Once we successfully compile the program, we don’t need to worry about any kinds of syntax errors. The code will be ready to be executed.
        Now the code is almost done, and the compiler knows what each data type is. Hence, it can produce an optimized machine code that uses less memory. So, the execution of the code will be faster compared to the dynamically-typed languages. These are the main advantages of statically-typed languages.
        
Dynamically-typed Languages-
        We call a language “dynamically typed” if type checking takes place while the program runs (run-time). In this type of language, there is no need to specify the data type of each variable while writing code.
        It means that you can write pretty quickly since you do not have to specify types every time. Some languages do allow you to provide type information but do not require it.
        Most modern programming languages are dynamically typed. Some examples of dynamically-typed languages are Python, Javascript, Ruby, Perl, PHP, R, Dart, Lua, Objective-C, etc.
        A dynamically-typed language has the capability to identify the type of each variable during run-time. In these languages, variables are bound to objects at run-time using assignment statements. We do not need to declare the data types of variables before we use them.
        One advantage of dynamically-typed languages is that it is easy to write code without worrying about the type of variables. The lack of a separate compilation step implies that programmers don’t have to wait for the compiler to finish before they can test the changes in code.
        The dynamic objects are having some run-time type-information(RTTI). It can be helpful to implement some pretty cool features like dynamic dispatch, down-casting, late binding, reflection, etc.
        
Statically typed languages have better performance at run-time and are faster at run-time. It is because there is no need for type checking at run-time, and the code has already been translated.

But dynamically-typed languages are comparatively faster during development time and are more flexible.


Q2. Scripting Language vs Programming Language
Ans:

Scripting languages are programming languages that don't require an explicit compilation step.

For example, in the normal case, you have to compile a C program before you can run it. But in the normal case, you don't have to compile a JavaScript program before you run it. So JavaScript is sometimes called a "scripting" language.

This line is getting more and more blurry since compilation can be so fast with modern hardware and modern compilation techniques. For instance, V8, the JavaScript engine in Google Chrome and used a lot outside of the browser as well, actually compiles the JavaScript code on the fly into machine code, rather than interpreting it. (In fact, V8's an optimizing two-phase compiler.)

Also note that whether a language is a "scripting" language or not can be more about the environment than the language. There's no reason you can't write a C interpreter and use it as a scripting language (and people have). There's also no reason you can't compile JavaScript to machine code and store that in an executable file (and people have). The language Ruby is a good example of this: The original implementation was entirely interpreted (a "scripting" language), but there are now multiple compilers for it.

Some examples of "scripting" languages (e.g., languages that are traditionally used without an explicit compilation step):
Lua,JavaScript,VBScript and VBA,Perl
And a small smattering of ones traditionally used with an explicit compilation step:
C,C++,D
Java (but note that Java is compiled to bytecode, which is then interpreted and/or recompiled at runtime)
Pascal and then you have things like Python that sit in both camps: Python is widely used without a compilation step, but the main implementation (CPython) does that by compiling to bytecode on-the-fly and then running the bytecode in a VM, and it can write that bytecode out to files (.pyc, .pyo) for use without recompiling.

Q3. Programming Paradigms

Ans:
A programming paradigm is a style, or “way,” of programming.
Some common programming paradig-
Imperative: Programming with an explicit sequence of commands that update state.
Declarative: Programming by specifying the result you want, not how to get it.
Structured: Programming with clean, goto-free, nested control structures.
Procedural: Imperative programming with procedure calls.
Functional (Applicative): Programming with function calls that avoid any global state.
Function-Level (Combinator): Programming with no variables at all.
Object-Oriented: Programming by defining objects that send messages to each other. Objects have their own internal (encapsulated) state and public interfaces. Object orientation can be:
Class-based: Objects get state and behavior based on membership in a class.
Prototype-based: Objects get behavior from a prototype object.
Event-Driven: Programming with emitters and listeners of asynchronous actions.
Flow-Driven: Programming processes communicating with each other over predefined channels.
Logic (Rule-based): Programming by specifying a set of facts and rules. An engine infers the answers to questions.
Constraint: Programming by specifying a set of constraints. An engine finds the values that meet the constraints.
Aspect-Oriented: Programming cross-cutting concerns applied transparently.
Reflective: Programming by manipulating the program elements themselves.
Array: Programming with powerful array operators that usually make loops unnecessary.

Imperative Programming- 
Control flow in imperative programming is explicit: commands show how the computation takes place, step by step. Each step affects the global state of the computation.

Structured Programming-
Structured programming is a kind of imperative programming where control flow is defined by nested loops, conditionals, and subroutines, rather than via gotos. Variables are generally local to blocks (have lexical scope).

Object Oriented Programming-
OOP is based on the sending of messages to objects. Objects respond to messages by performing operations, generally called methods. Messages can have arguments. A society of objects, each with their own local memory and own set of operations has a different feel than the monolithic processor and single shared memory feel of non object oriented languages.

One of the more visible aspects of the more pure-ish OO languages is that conditionals and loops become messages themselves, whose arguments are often blocks of executable code. 

Declarative Programming-
Control flow in declarative programming is implicit: the programmer states only what the result should look like, not how to obtain it.
No loops, no assignments, etc. Whatever engine that interprets this code is just supposed go get the desired information, and can use whatever approach it wants. (The logic and constraint paradigms are generally declarative as well.)

Functional Programming-
In functional programming, control flow is expressed by combining function calls, rather than by assigning values to variables:

Logic and Constraint Programming-
Logic programming and constraint programming are two paradigms in which programs are built by setting up relations that specify facts and inference rules, and asking whether or not something is true (i.e. specifying a goal.) Unification and backtracking to find solutions (i.e.. satisfy goals) takes place automatically.

Languages that emphasize this paradigm: Prolog, GHC, Parlog, Vulcan, Polka, Mercury, Fnil.

Languages and Paradigms
One of the characteristics of a language is its support for particular programming paradigms. For example, Smalltalk has direct support for programming in the object-oriented way, so it might be called an object-oriented language. OCaml, Lisp, Scheme, and JavaScript programs tend to make heavy use of passing functions around so they are called “functional languages” despite having variables and many imperative constructs.

There are two very important observations here:

Very few languages implement a paradigm 100%. When they do, they are pure. It is incredibly rare to have a “pure OOP” language or a “pure functional” language. A lot of languages have a few escapes; for example in OCaml, you will program with functions 90% or more of the time, but if you need state, you can get it. Another example: very few languages implement OOP the way Alan Kay envisioned it.
A lot of languages will facilitate programming in one or more paradigms. In Scala you can do imperative, object-oriented, and functional programming quite easily. If a language is purposely designed to allow programming in many paradigms is called a multi-paradigm language. If a language only accidentally supports multiple paradigms, we don’t have a special word for that.
