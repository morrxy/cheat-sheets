# Rich Hickey's Toolkits <sup>[[source]](http://infoq.com/presentations/Simple-Made-Easy)</sup>

## What's in your Toolkit?

Complexity                    | Simplicity
----------                    | ----------
State, Objects                | Values
Methods                       | Functions, Namespaces
vars                          | Managed refs
Inheritance, switch, matching | Polymorphism a la carte
Syntax                        | Data
Imperative loops, fold        | Set functions
Actors                        | Queues
ORM                           | Declarative data manipulation
Conditionals                  | Rules
Inconsistency                 | Consistency

## The Complexity Toolkit

Construct              | Complects
---------              | ---------
State                  | Everything that touches it
Objects                | State, identity, value
Methods                | Function and state, namespace
Syntax                 | Meaning, order
Inheritance            | Types
Switch/matching        | Multiple who/what pairs
var(iable)s            | Value, time
Imperative loops, fold | what/how
Actors                 | what/who
ORM                    | OMG
Conditionals           | Why, rest of program

## The Simplicity Toolkit

Construct                     | Get it via...
---------                     | -------------
Values                        | final, persistent collections
Functions                     | a.k.a. stateless methods
Namespaces                    | language support
Data                          | Maps, arrays, sets, XML, JSON etc
Polymorphism a la carte       | Protocols, type classes
Managed refs                  | Clojure/Haskell refs
Set functions                 | Libraries
Queues                        | Libraries
Declarative data manipulation | SQL/LINQ/Datalog
Rules                         | Libraries, Prolog
Consistency                   | Transaction, values
