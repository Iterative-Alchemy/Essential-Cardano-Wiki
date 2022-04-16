**Lambda calculus** (also written as **_λ_\-calculus**) is a [formal system](https://en.wikipedia.org/wiki/Formal_system "Formal system") in [mathematical logic](https://en.wikipedia.org/wiki/Mathematical_logic "Mathematical logic") for expressing [computation](https://en.wikipedia.org/wiki/Computability "Computability") based on function [abstraction](https://en.wikipedia.org/wiki/Abstraction_(computer_science) "Abstraction (computer science)") and [application](https://en.wikipedia.org/wiki/Function_application "Function application") using variable [binding](https://en.wikipedia.org/wiki/Name_binding "Name binding") and [substitution](https://en.wikipedia.org/wiki/Substitution_(algebra) "Substitution (algebra)"). It is a universal [model of computation](https://en.wikipedia.org/wiki/Model_of_computation "Model of computation") that can be used to simulate any [Turing machine](https://en.wikipedia.org/wiki/Turing_machine "Turing machine"). It was introduced by the mathematician [Alonzo Church](https://en.wikipedia.org/wiki/Alonzo_Church "Alonzo Church") in the 1930s as part of his research into the [foundations of mathematics](https://en.wikipedia.org/wiki/Foundations_of_mathematics "Foundations of mathematics").

Lambda calculus consists of constructing lambda terms and performing reduction operations on them. In the simplest form of lambda calculus, terms are built using only the following rules:

| Syntax | Name | Description |
| --- | --- | --- |
| _x_ | Variable | A character or string representing a parameter or mathematical/logical value. |
| (λ_x_._M_) | Abstraction | Function definition (_M_ is a lambda term). The variable _x_ becomes [bound](https://en.wikipedia.org/wiki/Free_variables_and_bound_variables "Free variables and bound variables") in the expression. |
| (_M_ _N_) | Application | Applying a function to an argument. _M_ and _N_ are lambda terms. |

producing expressions such as: (λ_x_.λ_y_.(λ_z_.(λ_x_._z x_) (λ_y_._z y_)) (_x y_)). Parentheses can be dropped if the expression is unambiguous. For some applications, terms for logical and mathematical constants and operations may be included.

The reduction operations include:

| Operation | Name | Description |
| --- | --- | --- |
| (λ_x_._M_\[_x_\]) → (λ_y_._M_\[_y_\]) | α-conversion | Renaming the bound variables in the expression. Used to avoid [name collisions](https://en.wikipedia.org/wiki/Name_collision "Name collision"). |
| ((λ_x_._M_) _E_) → (_M_\[_x_ := _E_\]) | β-reduction | Replacing the bound variables with the argument expression in the body of the abstraction. |

If [De Bruijn indexing](https://en.wikipedia.org/wiki/De_Bruijn_index "De Bruijn index") is used, then α-conversion is no longer required as there will be no name collisions. If [repeated application](https://en.wikipedia.org/wiki/Reduction_strategy_(lambda_calculus) "Reduction strategy (lambda calculus)") of the reduction steps eventually terminates, then by the [Church–Rosser theorem](https://en.wikipedia.org/wiki/Church%E2%80%93Rosser_theorem "Church–Rosser theorem") it will produce a [β-normal form](https://en.wikipedia.org/wiki/Beta_normal_form "Beta normal form").

Variable names are not needed if using a universal lambda function, such as [Iota and Jot](https://en.wikipedia.org/wiki/Iota_and_Jot "Iota and Jot"), which can create any function behavior by calling it on itself in various combinations.

## Explanation and applications\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=1 "Edit section: Explanation and applications")\]

Lambda calculus is [Turing complete](https://en.wikipedia.org/wiki/Turing_completeness "Turing completeness"), that is, it is a universal [model of computation](https://en.wikipedia.org/wiki/Model_of_computation "Model of computation") that can be used to simulate any [Turing machine](https://en.wikipedia.org/wiki/Turing_machine "Turing machine").[\[1\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-1) Its namesake, the Greek letter lambda (λ), is used in **lambda expressions** and **lambda terms** to denote [binding](https://en.wikipedia.org/wiki/Free_variables_and_bound_variables "Free variables and bound variables") a variable in a [function](https://en.wikipedia.org/wiki/Function_(mathematics) "Function (mathematics)").

Lambda calculus may be _untyped_ or _typed_. In typed lambda calculus, functions can be applied only if they are capable of accepting the given input's "type" of data. Typed lambda calculi are _weaker_ than the untyped lambda calculus, which is the primary subject of this article, in the sense that _typed lambda calculi can express less_ than the untyped calculus can, but on the other hand typed lambda calculi allow more things to be proven; in the [simply typed lambda calculus](https://en.wikipedia.org/wiki/Simply_typed_lambda_calculus "Simply typed lambda calculus") it is, for example, a theorem that every evaluation strategy terminates for every simply typed lambda-term, whereas evaluation of untyped lambda-terms need not terminate. One reason there are many different typed lambda calculi has been the desire to do more (of what the untyped calculus can do) without giving up on being able to prove strong theorems about the calculus.

Lambda calculus has applications in many different areas in [mathematics](https://en.wikipedia.org/wiki/Mathematics "Mathematics"), [philosophy](https://en.wikipedia.org/wiki/Philosophy "Philosophy"),[\[2\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-2) [linguistics](https://en.wikipedia.org/wiki/Linguistics "Linguistics"),[\[3\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-3)[\[4\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-4) and [computer science](https://en.wikipedia.org/wiki/Computer_science "Computer science").[\[5\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-5) Lambda calculus has played an important role in the development of the [theory of programming languages](https://en.wikipedia.org/wiki/Programming_language_theory "Programming language theory"). [Functional programming languages](https://en.wikipedia.org/wiki/Functional_programming_language "Functional programming language") implement lambda calculus. Lambda calculus is also a current research topic in [category theory](https://en.wikipedia.org/wiki/Category_theory "Category theory").[\[6\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-6)

## History\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=2 "Edit section: History")\]

The lambda calculus was introduced by mathematician [Alonzo Church](https://en.wikipedia.org/wiki/Alonzo_Church "Alonzo Church") in the 1930s as part of an investigation into the [foundations of mathematics](https://en.wikipedia.org/wiki/Foundations_of_mathematics "Foundations of mathematics").[\[7\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-7)[\[a\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-8) The original system was shown to be [logically inconsistent](https://en.wikipedia.org/wiki/Consistency "Consistency") in 1935 when [Stephen Kleene](https://en.wikipedia.org/wiki/Stephen_Kleene "Stephen Kleene") and [J. B. Rosser](https://en.wikipedia.org/wiki/J._B._Rosser "J. B. Rosser") developed the [Kleene–Rosser paradox](https://en.wikipedia.org/wiki/Kleene%E2%80%93Rosser_paradox "Kleene–Rosser paradox").[\[8\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-9)[\[9\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-10)

Subsequently, in 1936 Church isolated and published just the portion relevant to computation, what is now called the untyped lambda calculus.[\[10\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-Church1936-11) In 1940, he also introduced a computationally weaker, but logically consistent system, known as the [simply typed lambda calculus](https://en.wikipedia.org/wiki/Simply_typed_lambda_calculus "Simply typed lambda calculus").[\[11\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-12)

Until the 1960s when its relation to programming languages was clarified, the lambda calculus was only a formalism. Thanks to [Richard Montague](https://en.wikipedia.org/wiki/Richard_Montague "Richard Montague") and other linguists' applications in the semantics of natural language, the lambda calculus has begun to enjoy a respectable place in both linguistics[\[12\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-mm-linguistics-13) and computer science.[\[13\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-14)

### Origin of the lambda symbol\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=3 "Edit section: Origin of the lambda symbol")\]

There is some uncertainty over the reason for Church's use of the Greek letter [lambda](https://en.wikipedia.org/wiki/Lambda "Lambda") (λ) as the notation for function-abstraction in the lambda calculus, perhaps in part due to conflicting explanations by Church himself. According to Cardone and Hindley (2006):

> By the way, why did Church choose the notation “λ”? In \[an unpublished 1964 letter to Harald Dickson\] he stated clearly that it came from the notation “![{\hat {x}}](https://wikimedia.org/api/rest_v1/media/math/render/svg/18d95a7845e4e16ffb7e18ab37a208d0ab18e0e0)” used for class-abstraction by [Whitehead and Russell](https://en.wikipedia.org/wiki/Principia_Mathematica "Principia Mathematica"), by first modifying “![{\hat {x}}](https://wikimedia.org/api/rest_v1/media/math/render/svg/18d95a7845e4e16ffb7e18ab37a208d0ab18e0e0)” to “![{\displaystyle \land x}](https://wikimedia.org/api/rest_v1/media/math/render/svg/ca6600b27eac3943a56139dd5651de2eaa9e18ef)” to distinguish function-abstraction from class-abstraction, and then changing “![\land ](https://wikimedia.org/api/rest_v1/media/math/render/svg/d6823e5a222eb3ca49672818ac3d13ec607052c4)” to “λ” for ease of printing.
> 
> This origin was also reported in \[Rosser, 1984, p.338\]. On the other hand, in his later years Church told two enquirers that the choice was more accidental: a symbol was needed and λ just happened to be chosen.

[Dana Scott](https://en.wikipedia.org/wiki/Dana_Scott "Dana Scott") has also addressed this question in various public lectures.[\[14\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-15) Scott recounts that he once posed a question about the origin of the lambda symbol to Church's son-in-law John Addison, who then wrote his father-in-law a postcard:

> Dear Professor Church,
> 
> Russell had the [iota operator](https://en.wikipedia.org/wiki/Iota_operator "Iota operator"), Hilbert had the [epsilon operator](https://en.wikipedia.org/wiki/Epsilon_operator "Epsilon operator"). Why did you choose lambda for your operator?

According to Scott, Church's entire response consisted of returning the postcard with the following annotation: "[eeny, meeny, miny, moe](https://en.wikipedia.org/wiki/Eeny,_meeny,_miny,_moe "Eeny, meeny, miny, moe")".

## Informal description\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=4 "Edit section: Informal description")\]

### Motivation\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=5 "Edit section: Motivation")\]

[Computable functions](https://en.wikipedia.org/wiki/Computable_function "Computable function") are a fundamental concept within computer science and mathematics. The lambda calculus provides a simple [semantics](https://en.wikipedia.org/wiki/Semantics#Computer_science "Semantics") for computation, enabling properties of computation to be studied formally. The lambda calculus incorporates two simplifications that make this semantics simple. The first simplification is that the lambda calculus treats functions "anonymously", without giving them explicit names. For example, the function

![{\displaystyle \operatorname {square\_sum} (x,y)=x^{2}+y^{2}}](https://wikimedia.org/api/rest_v1/media/math/render/svg/6020e0858d923aa15ab308584dac8af2d003b879)

can be rewritten in _anonymous form_ as

![{\displaystyle (x,y)\mapsto x^{2}+y^{2}}](https://wikimedia.org/api/rest_v1/media/math/render/svg/89bf7c479bc1935d1ddd0519cde149591d0e541b)

(which is read as "a [tuple](https://en.wikipedia.org/wiki/Tuple "Tuple") of x and y is [mapped](https://en.wikipedia.org/wiki/Map_(mathematics) "Map (mathematics)") to ![{\textstyle x^{2}+y^{2}}](https://wikimedia.org/api/rest_v1/media/math/render/svg/2acda359ee232e747298436227bc8bee4ef82203)"). Similarly, the function

![\operatorname {id} (x)=x](https://wikimedia.org/api/rest_v1/media/math/render/svg/e64f26d868eb6952a36c600035ede967568c973f)

can be rewritten in anonymous form as

![x \mapsto x](https://wikimedia.org/api/rest_v1/media/math/render/svg/033c0ae81eaf4c65cbb0759d7aa2c4f434c00f02)

where the input is simply mapped to itself.

The second simplification is that the lambda calculus only uses functions of a single input. An ordinary function that requires two inputs, for instance the ![{\textstyle \operatorname {square\_sum} }](https://wikimedia.org/api/rest_v1/media/math/render/svg/b1452ce7cbdc7fd26d4b880eddf9b28d0c4965a7) function, can be reworked into an equivalent function that accepts a single input, and as output returns _another_ function, that in turn accepts a single input. For example,

![{\displaystyle (x,y)\mapsto x^{2}+y^{2}}](https://wikimedia.org/api/rest_v1/media/math/render/svg/89bf7c479bc1935d1ddd0519cde149591d0e541b)

can be reworked into

![{\displaystyle x\mapsto (y\mapsto x^{2}+y^{2})}](https://wikimedia.org/api/rest_v1/media/math/render/svg/012fc8f19ed14bf232ee8deefe4ae84dc507875d)

This method, known as [currying](https://en.wikipedia.org/wiki/Currying "Currying"), transforms a function that takes multiple arguments into a chain of functions each with a single argument.

[Function application](https://en.wikipedia.org/wiki/Function_application "Function application") of the ![{\textstyle \operatorname {square\_sum} }](https://wikimedia.org/api/rest_v1/media/math/render/svg/b1452ce7cbdc7fd26d4b880eddf9b28d0c4965a7) function to the arguments (5, 2), yields at once

![{\textstyle ((x,y)\mapsto x^{2}+y^{2})(5,2)}](https://wikimedia.org/api/rest_v1/media/math/render/svg/928ef499250ddf3fae99e9a0e7e81bd4aa57e3b9)

![{\textstyle =5^{2}+2^{2}}](https://wikimedia.org/api/rest_v1/media/math/render/svg/80c505b7a93daffe13a057837fb7071280cda48f)

![{\textstyle =29}](https://wikimedia.org/api/rest_v1/media/math/render/svg/d026d595296c5d7351c05ffd86b0ffec19fe88b1),

whereas evaluation of the curried version requires one more step

![{\textstyle {\Bigl (}{\bigl (}x\mapsto (y\mapsto x^{2}+y^{2}){\bigr )}(5){\Bigr )}(2)}](https://wikimedia.org/api/rest_v1/media/math/render/svg/951bcb4894272800f3c7e53a20b4fbc1f7c5331d)

![{\textstyle =(y\mapsto 5^{2}+y^{2})(2)}](https://wikimedia.org/api/rest_v1/media/math/render/svg/9e02299d716372384546a46e1ad5cdc117f32949) // the definition of ![x](https://wikimedia.org/api/rest_v1/media/math/render/svg/87f9e315fd7e2ba406057a97300593c4802b53e4) has been used with ![5](https://wikimedia.org/api/rest_v1/media/math/render/svg/29483407999b8763f0ea335cf715a6a5e809f44b) in the inner expression. This is like β-reduction.

![{\textstyle =5^{2}+2^{2}}](https://wikimedia.org/api/rest_v1/media/math/render/svg/80c505b7a93daffe13a057837fb7071280cda48f) // the definition of ![y](https://wikimedia.org/api/rest_v1/media/math/render/svg/b8a6208ec717213d4317e666f1ae872e00620a0d) has been used with ![2](https://wikimedia.org/api/rest_v1/media/math/render/svg/901fc910c19990d0dbaaefe4726ceb1a4e217a0f). Again, similar to β-reduction.

![{\textstyle =29}](https://wikimedia.org/api/rest_v1/media/math/render/svg/d026d595296c5d7351c05ffd86b0ffec19fe88b1)

to arrive at the same result.

### The lambda calculus\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=6 "Edit section: The lambda calculus")\]

The lambda calculus consists of a language of **lambda terms**, which are defined by a certain formal syntax, and a set of transformation rules, which allow manipulation of the lambda terms. These transformation rules can be viewed as an [equational theory](https://en.wikipedia.org/wiki/Equational_theory "Equational theory") or as an [operational definition](https://en.wikipedia.org/wiki/Operational_definition "Operational definition").

As described above, all functions in the lambda calculus are anonymous functions, having no names. They only accept one input variable, with [currying](https://en.wikipedia.org/wiki/Currying "Currying") used to implement functions with several variables.

#### Lambda terms\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=7 "Edit section: Lambda terms")\]

The syntax of the lambda calculus defines some expressions as valid lambda calculus expressions and some as invalid, just as some strings of characters are valid [C](https://en.wikipedia.org/wiki/C_(programming_language) "C (programming language)") programs and some are not. A valid lambda calculus expression is called a "lambda term".

The following three rules give an [inductive definition](https://en.wikipedia.org/wiki/Inductive_definition "Inductive definition") that can be applied to build all syntactically valid lambda terms:

Nothing else is a lambda term. Thus a lambda term is valid if and only if it can be obtained by repeated application of these three rules. However, some parentheses can be omitted according to certain rules. For example, the outermost parentheses are usually not written. See _[Notation](https://en.wikipedia.org/wiki/Lambda_calculus#Notation)_, below.

An **abstraction** ![\lambda x.t](https://wikimedia.org/api/rest_v1/media/math/render/svg/6c340da553f36c8832a4a6aff7d235dd2acb760a) is a definition of an anonymous function that is capable of taking a single input x and substituting it into the expression t. It thus defines an anonymous function that takes x and returns t. For example, ![\lambda x.x^{2}+2](https://wikimedia.org/api/rest_v1/media/math/render/svg/775066d410c7fa3072ddad801ac74ad2f0d51bc8) is an abstraction for the function ![f(x)=x^{2}+2](https://wikimedia.org/api/rest_v1/media/math/render/svg/36b2fad9afa6bfc8ab4f81a413ebf4e9ba7f9117) using the term ![x^{2}+2](https://wikimedia.org/api/rest_v1/media/math/render/svg/a4c90c2a3ab4bc8c2b353d3dc65962bc35020469) for t. The definition of a function with an abstraction merely "sets up" the function but does not invoke it. The abstraction [binds](https://en.wikipedia.org/wiki/Free_variables_and_bound_variables "Free variables and bound variables") the variable x in the term t.

An **application** ts represents the application of a function t to an input s, that is, it represents the act of calling function t on input s to produce ![t(s)](https://wikimedia.org/api/rest_v1/media/math/render/svg/abde739dff178e6e78929b3ce6870ec81e3f2d98).

There is no concept in lambda calculus of variable declaration. In a definition such as ![\lambda x.x+y](https://wikimedia.org/api/rest_v1/media/math/render/svg/d2d683052bfe9bfd6b91fa645a2d5210d596a969) (i.e. ![f(x)=x+y](https://wikimedia.org/api/rest_v1/media/math/render/svg/62f1b4363757a5a6b04d28f679be66ccdcc958cc)), the lambda calculus treats y as a variable that is not yet defined. The abstraction ![\lambda x.x+y](https://wikimedia.org/api/rest_v1/media/math/render/svg/d2d683052bfe9bfd6b91fa645a2d5210d596a969) is syntactically valid, and represents a function that adds its input to the yet-unknown y.

Bracketing may be used and may be needed to disambiguate terms. For example, ![\lambda x.((\lambda x.x)x)](https://wikimedia.org/api/rest_v1/media/math/render/svg/7aa284718745826bd142338fc1e6110582f46583) and ![(\lambda x.(\lambda x.x))x](https://wikimedia.org/api/rest_v1/media/math/render/svg/70591fccd68750f2742e11104d56e124f0a2106f) denote different terms (although they coincidentally reduce to the same value). Here, the first example defines a function whose lambda term is the result of applying x to the child function, while the second example is the application of the outermost function to the input x, which returns the child function. Therefore, both examples evaluate to the [identity function](https://en.wikipedia.org/wiki/Identity_function "Identity function") ![\lambda x.x](https://wikimedia.org/api/rest_v1/media/math/render/svg/537ec33b43915b93dec1c98e433ec7a68bcab6a3).

#### Functions that operate on functions\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=8 "Edit section: Functions that operate on functions")\]

In lambda calculus, functions are taken to be '[first class values](https://en.wikipedia.org/wiki/First-class_object "First-class object")', so functions may be used as the inputs, or be returned as outputs from other functions.

For example, ![\lambda x.x](https://wikimedia.org/api/rest_v1/media/math/render/svg/537ec33b43915b93dec1c98e433ec7a68bcab6a3) represents the [identity function](https://en.wikipedia.org/wiki/Identity_function "Identity function"), ![x \mapsto x](https://wikimedia.org/api/rest_v1/media/math/render/svg/033c0ae81eaf4c65cbb0759d7aa2c4f434c00f02), and ![(\lambda x.x)y](https://wikimedia.org/api/rest_v1/media/math/render/svg/b0843fde0f55684a922242d745e75e0764bf9b85) represents the identity function applied to ![y](https://wikimedia.org/api/rest_v1/media/math/render/svg/b8a6208ec717213d4317e666f1ae872e00620a0d). Further, ![(\lambda x.y)](https://wikimedia.org/api/rest_v1/media/math/render/svg/8a6b3722955a98e2eb07402e0380da6d7739a5da) represents the **constant function** ![{\displaystyle x\mapsto y}](https://wikimedia.org/api/rest_v1/media/math/render/svg/eb2452f2d32e5424f3db361de033fd49a73f9dcc), the function that always returns ![y](https://wikimedia.org/api/rest_v1/media/math/render/svg/b8a6208ec717213d4317e666f1ae872e00620a0d), no matter the input. In lambda calculus, function application is regarded as [left-associative](https://en.wikipedia.org/wiki/Operator_associativity "Operator associativity"), so that ![stx](https://wikimedia.org/api/rest_v1/media/math/render/svg/473aae76f793dd8a9acac4583cfea7af033751c0) means ![(st)x](https://wikimedia.org/api/rest_v1/media/math/render/svg/37df60654b0c688f880a89e008bd71eb6cb4fd2e).

There are several notions of "equivalence" and "reduction" that allow lambda terms to be "reduced" to "equivalent" lambda terms.

#### Alpha equivalence\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=9 "Edit section: Alpha equivalence")\]

A basic form of equivalence, definable on lambda terms, is alpha equivalence. It captures the intuition that the particular choice of a bound variable, in an abstraction, does not (usually) matter. For instance, ![\lambda x.x](https://wikimedia.org/api/rest_v1/media/math/render/svg/537ec33b43915b93dec1c98e433ec7a68bcab6a3) and ![\lambda y.y](https://wikimedia.org/api/rest_v1/media/math/render/svg/6491d675717cbe434705e447484c1e267743c672) are alpha-equivalent lambda terms, and they both represent the same function (the identity function). The terms ![x](https://wikimedia.org/api/rest_v1/media/math/render/svg/87f9e315fd7e2ba406057a97300593c4802b53e4) and ![y](https://wikimedia.org/api/rest_v1/media/math/render/svg/b8a6208ec717213d4317e666f1ae872e00620a0d) are not alpha-equivalent, because they are not bound in an abstraction. In many presentations, it is usual to identify alpha-equivalent lambda terms.

The following definitions are necessary in order to be able to define β-reduction:

#### Free variables\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=10 "Edit section: Free variables")\]

(free variables in lambda Notation and its Calculus are comparable to [linear algebra and mathematical concepts of the same name](https://en.wikipedia.org/wiki/Free_variables_and_bound_variables "Free variables and bound variables"))

The **free variables** of a term are those variables not bound by an abstraction. The set of free variables of an expression is defined inductively:

For example, the lambda term representing the identity ![\lambda x.x](https://wikimedia.org/api/rest_v1/media/math/render/svg/537ec33b43915b93dec1c98e433ec7a68bcab6a3) has no free variables, but the function ![{\displaystyle \lambda x.yx}](https://wikimedia.org/api/rest_v1/media/math/render/svg/00b13f7b499f19ada754e7eff1dd71dd0b5a137b) has a single free variable, ![y](https://wikimedia.org/api/rest_v1/media/math/render/svg/b8a6208ec717213d4317e666f1ae872e00620a0d).

#### Capture-avoiding substitutions\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=11 "Edit section: Capture-avoiding substitutions")\]

[A systematic change in variables to avoid capture of a free variable can introduce error](https://en.wikipedia.org/wiki/SECD_machine#Landin's_contribution "SECD machine"), in a functional programming language where functions are first class citizens.[\[15\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-tfp12-16)

Suppose ![t](https://wikimedia.org/api/rest_v1/media/math/render/svg/65658b7b223af9e1acc877d848888ecdb4466560), ![s](https://wikimedia.org/api/rest_v1/media/math/render/svg/01d131dfd7673938b947072a13a9744fe997e632) and ![r](https://wikimedia.org/api/rest_v1/media/math/render/svg/0d1ecb613aa2984f0576f70f86650b7c2a132538) are lambda terms and ![x](https://wikimedia.org/api/rest_v1/media/math/render/svg/87f9e315fd7e2ba406057a97300593c4802b53e4) and ![y](https://wikimedia.org/api/rest_v1/media/math/render/svg/b8a6208ec717213d4317e666f1ae872e00620a0d) are variables. The notation ![t[x:=r]](https://wikimedia.org/api/rest_v1/media/math/render/svg/18e1a37baab228f8a6915d5f6b1cf94c48188a2a) indicates substitution of ![r](https://wikimedia.org/api/rest_v1/media/math/render/svg/0d1ecb613aa2984f0576f70f86650b7c2a132538) for ![x](https://wikimedia.org/api/rest_v1/media/math/render/svg/87f9e315fd7e2ba406057a97300593c4802b53e4) in ![t](https://wikimedia.org/api/rest_v1/media/math/render/svg/65658b7b223af9e1acc877d848888ecdb4466560) in a _capture-avoiding_ manner. This is defined so that:

For example, ![(\lambda x.x)[y:=y]=\lambda x.(x[y:=y])=\lambda x.x](https://wikimedia.org/api/rest_v1/media/math/render/svg/592caa8aa08c98d5217f7dfec3edcb5cb3521fac), and ![((\lambda x.y)x)[x:=y]=((\lambda x.y)[x:=y])(x[x:=y])=(\lambda x.y)y](https://wikimedia.org/api/rest_v1/media/math/render/svg/3b294b29a663f2b54d066505b5ddafdaab77d635).

The freshness condition (requiring that ![y](https://wikimedia.org/api/rest_v1/media/math/render/svg/b8a6208ec717213d4317e666f1ae872e00620a0d) is not in the free variables of ![r](https://wikimedia.org/api/rest_v1/media/math/render/svg/0d1ecb613aa2984f0576f70f86650b7c2a132538)) is crucial in order to ensure that substitution does not change the meaning of functions. For example, a substitution is made that ignores the freshness condition can lead to errors: ![(\lambda x.y)[y:=x]=\lambda x.(y[y:=x])=\lambda x.x](https://wikimedia.org/api/rest_v1/media/math/render/svg/28dca32bd1aaa04013520bfac21bba12df0744a5). This substitution turns the constant function ![\lambda x.y](https://wikimedia.org/api/rest_v1/media/math/render/svg/88b2e10a12e276198f384ca3f5da934bdfaedc07) into the identity ![\lambda x.x](https://wikimedia.org/api/rest_v1/media/math/render/svg/537ec33b43915b93dec1c98e433ec7a68bcab6a3) by substitution.

In general, failure to meet the freshness condition can be remedied by alpha-renaming with a suitable fresh variable. For example, switching back to our correct notion of substitution, in ![(\lambda x.y)[y:=x]](https://wikimedia.org/api/rest_v1/media/math/render/svg/0e113a57c201a6477f5bad7a114f70fe6a378858) the abstraction can be renamed with a fresh variable ![z](https://wikimedia.org/api/rest_v1/media/math/render/svg/bf368e72c009decd9b6686ee84a375632e11de98), to obtain ![(\lambda z.y)[y:=x]=\lambda z.(y[y:=x])=\lambda z.x](https://wikimedia.org/api/rest_v1/media/math/render/svg/7275d0fbddf5e54be2666eb5cb6b7baacaf00d24), and the meaning of the function is preserved by substitution.

#### β-reduction\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=12 "Edit section: β-reduction")\]

The β-reduction rule states that an application of the form ![(\lambda x.t)s](https://wikimedia.org/api/rest_v1/media/math/render/svg/56eb16cb15bc2d59d009c0b86ecd37e9ce6f7991) reduces to the term ![t[x:=s]](https://wikimedia.org/api/rest_v1/media/math/render/svg/c69396d99d4f60dbe54641cf62b9864b0a2251e1). The notation ![(\lambda x.t)s\to t[x:=s]](https://wikimedia.org/api/rest_v1/media/math/render/svg/8b3ec6af9a3a97d2362dd9473b3b00f414b5323e) is used to indicate that ![(\lambda x.t)s](https://wikimedia.org/api/rest_v1/media/math/render/svg/56eb16cb15bc2d59d009c0b86ecd37e9ce6f7991) β-reduces to ![t[x:=s]](https://wikimedia.org/api/rest_v1/media/math/render/svg/c69396d99d4f60dbe54641cf62b9864b0a2251e1). For example, for every ![s](https://wikimedia.org/api/rest_v1/media/math/render/svg/01d131dfd7673938b947072a13a9744fe997e632), ![(\lambda x.x)s\to x[x:=s]=s](https://wikimedia.org/api/rest_v1/media/math/render/svg/02262c02953e5da0468ebf98f4b38327229bd4c9). This demonstrates that ![\lambda x.x](https://wikimedia.org/api/rest_v1/media/math/render/svg/537ec33b43915b93dec1c98e433ec7a68bcab6a3) really is the identity. Similarly, ![(\lambda x.y)s\to y[x:=s]=y](https://wikimedia.org/api/rest_v1/media/math/render/svg/de42f8231c1e95fb1556e6aee11c40d0000ea008), which demonstrates that ![\lambda x.y](https://wikimedia.org/api/rest_v1/media/math/render/svg/88b2e10a12e276198f384ca3f5da934bdfaedc07) is a constant function.

The lambda calculus may be seen as an idealized version of a functional programming language, like [Haskell](https://en.wikipedia.org/wiki/Haskell_(programming_language) "Haskell (programming language)") or [Standard ML](https://en.wikipedia.org/wiki/Standard_ML "Standard ML"). Under this view, β-reduction corresponds to a computational step. This step can be repeated by additional β-reductions until there are no more applications left to reduce. In the untyped lambda calculus, as presented here, this reduction process may not terminate. For instance, consider the term ![\Omega =(\lambda x.xx)(\lambda x.xx)](https://wikimedia.org/api/rest_v1/media/math/render/svg/3bfe87ff478d8ea96e37b17523c091fa9812a4ee). Here ![(\lambda x.xx)(\lambda x.xx)\to (xx)[x:=\lambda x.xx]=(x[x:=\lambda x.xx])(x[x:=\lambda x.xx])=(\lambda x.xx)(\lambda x.xx)](https://wikimedia.org/api/rest_v1/media/math/render/svg/ba84bd0baf6c5c33e59226aa42474b36e3046231). That is, the term reduces to itself in a single β-reduction, and therefore the reduction process will never terminate.

Another aspect of the untyped lambda calculus is that it does not distinguish between different kinds of data. For instance, it may be desirable to write a function that only operates on numbers. However, in the untyped lambda calculus, there is no way to prevent a function from being applied to [truth values](https://en.wikipedia.org/wiki/Truth_value "Truth value"), strings, or other non-number objects.

## Formal definition\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=13 "Edit section: Formal definition")\]

### Definition\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=14 "Edit section: Definition")\]

Lambda expressions are composed of:

-   variables _v_1, _v_2, ...;
-   the abstraction symbols λ (lambda) and . (dot);
-   parentheses ().

The set of lambda expressions, Λ, can be [defined inductively](https://en.wikipedia.org/wiki/Recursive_definition "Recursive definition"):

1.  If _x_ is a variable, then _x_ ∈ Λ.
2.  If _x_ is a variable and _M_ ∈ Λ, then (λ_x_._M_) ∈ Λ.
3.  If _M_, _N_ ∈ Λ, then (_M N_) ∈ Λ.

Instances of rule 2 are known as _abstractions_ and instances of rule 3 are known as _applications_.[\[16\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-17)[\[17\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-18)

### Notation\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=15 "Edit section: Notation")\]

To keep the notation of lambda expressions uncluttered, the following conventions are usually applied:

-   Outermost parentheses are dropped: _M_ _N_ instead of (_M_ _N_).
-   Applications are assumed to be left associative: _M_ _N_ _P_ may be written instead of ((_M_ _N_) _P_).[\[18\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-lambda-bound-19)
-   The body of an abstraction extends [as far right as possible](https://en.wikipedia.org/wiki/Regular_expression#Lazy_matching "Regular expression"): λ_x_._M N_ means λ_x_.(_M N_) and not (λ_x_._M_) _N_.
-   A sequence of abstractions is contracted: λ_x_.λ_y_.λ_z_._N_ is abbreviated as λ_xyz_._N_.[\[19\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-Selinger-20)[\[18\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-lambda-bound-19)

### Free and bound variables\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=16 "Edit section: Free and bound variables")\]

The abstraction operator, λ, is said to bind its variable wherever it occurs in the body of the abstraction. Variables that fall within the scope of an abstraction are said to be _bound_. In an expression λ_x_._M_, the part λ_x_ is often called _binder_, as a hint that the variable _x_ is getting bound by appending λ_x_ to _M_. All other variables are called _free_. For example, in the expression λ_y_._x x y_, _y_ is a bound variable and _x_ is a free variable. Also a variable is bound by its nearest abstraction. In the following example the single occurrence of _x_ in the expression is bound by the second lambda: λ_x_._y_ (λ_x_._z x_).

The set of _free variables_ of a lambda expression, _M_, is denoted as FV(_M_) and is defined by recursion on the structure of the terms, as follows:

1.  FV(_x_) = {_x_}, where _x_ is a variable.
2.  FV(λ_x_._M_) = FV(_M_) \\ {_x_}.
3.  FV(_M N_) = FV(_M_) ∪ FV(_N_).[\[20\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-BarendregtBarendsen-21)

An expression that contains no free variables is said to be _closed_. Closed lambda expressions are also known as _combinators_ and are equivalent to terms in [combinatory logic](https://en.wikipedia.org/wiki/Combinatory_logic "Combinatory logic").

## Reduction\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=17 "Edit section: Reduction")\]

The meaning of lambda expressions is defined by how expressions can be reduced.[\[21\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-22)

There are three kinds of reduction:

-   **α-conversion**: changing bound variables;
-   **β-reduction**: applying functions to their arguments;
-   **η-reduction**: which captures a notion of extensionality.

We also speak of the resulting equivalences: two expressions are _α-equivalent_, if they can be α-converted into the same expression. β-equivalence and η-equivalence are defined similarly.

The term _redex_, short for _reducible expression_, refers to subterms that can be reduced by one of the reduction rules. For example, (λ_x_._M_) _N_ is a β-redex in expressing the substitution of _N_ for _x_ in _M_. The expression to which a redex reduces is called its _reduct_; the reduct of (λ_x_._M_) _N_ is _M_\[_x_ := _N_\].

If _x_ is not free in _M_, λ_x_._M x_ is also an η-redex, with a reduct of _M_.

### α-conversion\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=18 "Edit section: α-conversion")\]

α-conversion, sometimes known as α-renaming,[\[22\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-23) allows bound variable names to be changed. For example, α-conversion of λ_x_._x_ might yield λ_y_._y_. Terms that differ only by α-conversion are called _α-equivalent_. Frequently, in uses of lambda calculus, α-equivalent terms are considered to be equivalent.

The precise rules for α-conversion are not completely trivial. First, when α-converting an abstraction, the only variable occurrences that are renamed are those that are bound to the same abstraction. For example, an α-conversion of λ_x_.λ_x_._x_ could result in λ_y_.λ_x_._x_, but it could _not_ result in λ_y_.λ_x_._y_. The latter has a different meaning from the original. This is analogous to the programming notion of [variable shadowing](https://en.wikipedia.org/wiki/Variable_shadowing "Variable shadowing").

Second, α-conversion is not possible if it would result in a variable getting captured by a different abstraction. For example, if we replace _x_ with _y_ in λ_x_.λ_y_._x_, we get λ_y_.λ_y_._y_, which is not at all the same.

In programming languages with static scope, α-conversion can be used to make [name resolution](https://en.wikipedia.org/wiki/Name_resolution_(programming_languages) "Name resolution (programming languages)") simpler by ensuring that no variable name [masks](https://en.wikipedia.org/wiki/Variable_shadowing "Variable shadowing") a name in a containing [scope](https://en.wikipedia.org/wiki/Scope_(programming) "Scope (programming)") (see [α-renaming to make name resolution trivial](https://en.wikipedia.org/wiki/Name_resolution_(programming_languages)#Alpha_renaming_to_make_name_resolution_trivial "Name resolution (programming languages)")).

In the [De Bruijn index](https://en.wikipedia.org/wiki/De_Bruijn_index "De Bruijn index") notation, any two α-equivalent terms are syntactically identical.

#### Substitution\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=19 "Edit section: Substitution")\]

Substitution, written _M_\[_V_ := _N_\], is the process of replacing all _free_ occurrences of the variable _V_ in the expression _M_ with expression _N_. Substitution on terms of the lambda calculus is defined by recursion on the structure of terms, as follows (note: x and y are only variables while M and N are any lambda expression):

_x_\[_x_ := _N_\] = _N_

_y_\[_x_ := _N_\] = _y_, if _x_ ≠ _y_

(_M_1 _M_2)\[_x_ := _N_\] = _M_1\[_x_ := _N_\] _M_2\[_x_ := _N_\]

(λ_x_._M_)\[_x_ := _N_\] = λ_x_._M_

(λ_y_._M_)\[_x_ := _N_\] = λ_y_.(_M_\[_x_ := _N_\]), if _x_ ≠ _y_ and _y_ ∉ FV(_N_)

To substitute into an abstraction, it is sometimes necessary to α-convert the expression. For example, it is not correct for (λ_x_._y_)\[_y_ := _x_\] to result in λ_x_._x_, because the substituted _x_ was supposed to be free but ended up being bound. The correct substitution in this case is λ_z_._x_, up to α-equivalence. Substitution is defined uniquely up to α-equivalence.

### β-reduction\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=20 "Edit section: β-reduction")\]

β-reduction captures the idea of function application. β-reduction is defined in terms of substitution: the β-reduction of (λ_V_._M_) _N_ is _M_\[_V_ := _N_\].

For example, assuming some encoding of 2, 7, ×, we have the following β-reduction: (λ_n_._n_ × 2) 7 → 7 × 2.

β-reduction can be seen to be the same as the concept of _local reducibility_ in [natural deduction](https://en.wikipedia.org/wiki/Natural_deduction "Natural deduction"), via the [Curry–Howard isomorphism](https://en.wikipedia.org/wiki/Curry%E2%80%93Howard_isomorphism "Curry–Howard isomorphism").

### η-reduction\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=21 "Edit section: η-reduction")\]

η-reduction expresses the idea of [extensionality](https://en.wikipedia.org/wiki/Extensionality "Extensionality"), which in this context is that two functions are the same [if and only if](https://en.wikipedia.org/wiki/If_and_only_if "If and only if") they give the same result for all arguments. η-reduction converts between λ_x_._f_ _x_ and _f_ whenever _x_ does not appear free in _f_.

η-reduction can be seen to be the same as the concept of _local completeness_ in [natural deduction](https://en.wikipedia.org/wiki/Natural_deduction "Natural deduction"), via the [Curry–Howard isomorphism](https://en.wikipedia.org/wiki/Curry%E2%80%93Howard_isomorphism "Curry–Howard isomorphism").

## Normal forms and confluence\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=22 "Edit section: Normal forms and confluence")\]

For the untyped lambda calculus, β-reduction as a [rewriting rule](https://en.wikipedia.org/wiki/Rewrite_system "Rewrite system") is neither [strongly normalising](https://en.wikipedia.org/wiki/Strongly_normalising "Strongly normalising") nor [weakly normalising](https://en.wikipedia.org/wiki/Weakly_normalising "Weakly normalising").

However, it can be shown that β-reduction is [confluent](https://en.wikipedia.org/wiki/Confluence_(abstract_rewriting) "Confluence (abstract rewriting)") when working up to α-conversion (i.e. we consider two normal forms to be equal if it is possible to α-convert one into the other).

Therefore, both strongly normalising terms and weakly normalising terms have a unique normal form. For strongly normalising terms, any reduction strategy is guaranteed to yield the normal form, whereas for weakly normalising terms, some reduction strategies may fail to find it.

## Encoding datatypes\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=23 "Edit section: Encoding datatypes")\]

The basic lambda calculus may be used to model booleans, [arithmetic](https://en.wikipedia.org/wiki/Arithmetic "Arithmetic"), data structures and recursion, as illustrated in the following sub-sections.

### Arithmetic in lambda calculus\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=24 "Edit section: Arithmetic in lambda calculus")\]

There are several possible ways to define the [natural numbers](https://en.wikipedia.org/wiki/Natural_number "Natural number") in lambda calculus, but by far the most common are the [Church numerals](https://en.wikipedia.org/wiki/Church_numeral "Church numeral"), which can be defined as follows:

0 := λ_f_.λ_x_._x_

1 := λ_f_.λ_x_._f_ _x_

2 := λ_f_.λ_x_._f_ (_f_ _x_)

3 := λ_f_.λ_x_._f_ (_f_ (_f_ _x_))

and so on. Or using the alternative syntax presented above in _[Notation](https://en.wikipedia.org/wiki/Lambda_calculus#Notation)_:

0 := λ_fx_._x_

1 := λ_fx_._f_ _x_

2 := λ_fx_._f_ (_f_ _x_)

3 := λ_fx_._f_ (_f_ (_f_ _x_))

A Church numeral is a [higher-order function](https://en.wikipedia.org/wiki/Higher-order_function "Higher-order function")—it takes a single-argument function _f_, and returns another single-argument function. The Church numeral _n_ is a function that takes a function _f_ as argument and returns the _n_\-th composition of _f_, i.e. the function _f_ composed with itself _n_ times. This is denoted _f_(_n_) and is in fact the _n_\-th power of _f_ (considered as an operator); _f_(0) is defined to be the identity function. Such repeated compositions (of a single function _f_) obey the [laws of exponents](https://en.wikipedia.org/wiki/Laws_of_exponents "Laws of exponents"), which is why these numerals can be used for arithmetic. (In Church's original lambda calculus, the formal parameter of a lambda expression was required to occur at least once in the function body, which made the above definition of 0 impossible.)

One way of thinking about the Church numeral _n_, which is often useful when analysing programs, is as an instruction 'repeat _n_ times'. For example, using the PAIR and NIL functions defined below, one can define a function that constructs a (linked) list of _n_ elements all equal to _x_ by repeating 'prepend another _x_ element' _n_ times, starting from an empty list. The lambda term is

λ_n_.λ_x_._n_ (PAIR _x_) NIL

By varying what is being repeated, and varying what argument that function being repeated is applied to, a great many different effects can be achieved.

We can define a successor function, which takes a Church numeral _n_ and returns _n_ + 1 by adding another application of _f_, where '(mf)x' means the function 'f' is applied 'm' times on 'x':

SUCC := λ_n_.λ_f_.λ_x_._f_ (_n_ _f_ _x_)

Because the _m_\-th composition of _f_ composed with the _n_\-th composition of _f_ gives the _m_+_n_\-th composition of _f_, addition can be defined as follows:

PLUS := λ_m_.λ_n_.λ_f_.λ_x_._m_ _f_ (_n_ _f_ _x_)

PLUS can be thought of as a function taking two natural numbers as arguments and returning a natural number; it can be verified that

PLUS 2 3

and

5

are β-equivalent lambda expressions. Since adding _m_ to a number _n_ can be accomplished by adding 1 _m_ times, an alternative definition is:

PLUS := λ_m_.λ_n_._m_ SUCC _n_ [\[23\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-24)

Similarly, multiplication can be defined as

MULT := λ_m_.λ_n_.λ_f_._m_ (_n_ _f_)[\[19\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-Selinger-20)

Alternatively

MULT := λ_m_.λ_n_._m_ (PLUS _n_) 0

since multiplying _m_ and _n_ is the same as repeating the add _n_ function _m_ times and then applying it to zero. Exponentiation has a rather simple rendering in Church numerals, namely

POW := λ_b_.λ_e_._e_ _b_[\[20\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-BarendregtBarendsen-21)

The predecessor function defined by PRED _n_ = _n_ − 1 for a positive integer _n_ and PRED 0 = 0 is considerably more difficult. The formula

PRED := λ_n_.λ_f_.λ_x_._n_ (λ_g_.λ_h_._h_ (_g_ _f_)) (λ_u_._x_) (λ_u_._u_)

can be validated by showing inductively that if _T_ denotes (λ_g_.λ_h_._h_ (_g_ _f_)), then T(_n_)(λ_u_._x_) = (λ_h_._h_(_f_(_n_−1)(_x_))) for _n_ > 0. Two other definitions of PRED are given below, one using [conditionals](https://en.wikipedia.org/wiki/Lambda_calculus#Logic_and_predicates) and the other using [pairs](https://en.wikipedia.org/wiki/Lambda_calculus#Pairs). With the predecessor function, subtraction is straightforward. Defining

SUB := λ_m_.λ_n_._n_ PRED _m_,

SUB _m_ _n_ yields _m_ − _n_ when _m_ > _n_ and 0 otherwise.

### Logic and predicates\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=25 "Edit section: Logic and predicates")\]

By convention, the following two definitions (known as Church booleans) are used for the boolean values TRUE and FALSE:

TRUE := λ_x_.λ_y_._x_

FALSE := λ_x_.λ_y_._y_

(Note that FALSE is equivalent to the Church numeral zero defined above)

Then, with these two lambda terms, we can define some logic operators (these are just possible formulations; other expressions are equally correct):

AND := λ_p_.λ_q_._p_ _q_ _p_

OR := λ_p_.λ_q_._p_ _p_ _q_

NOT := λ_p_._p_ FALSE TRUE

IFTHENELSE := λ_p_.λ_a_.λ_b_._p_ _a_ _b_

We are now able to compute some logic functions, for example:

AND TRUE FALSE

≡ (λ_p_.λ_q_._p_ _q_ _p_) TRUE FALSE →β TRUE FALSE TRUE

≡ (λ_x_.λ_y_._x_) FALSE TRUE →β FALSE

and we see that AND TRUE FALSE is equivalent to FALSE.

A _predicate_ is a function that returns a boolean value. The most fundamental predicate is ISZERO, which returns TRUE if its argument is the Church numeral 0, and FALSE if its argument is any other Church numeral:

ISZERO := λ_n_._n_ (λ_x_.FALSE) TRUE

The following predicate tests whether the first argument is less-than-or-equal-to the second:

LEQ := λ_m_.λ_n_.ISZERO (SUB _m_ _n_),

and since _m_ = _n_, if LEQ _m_ _n_ and LEQ _n_ _m_, it is straightforward to build a predicate for numerical equality.

The availability of predicates and the above definition of TRUE and FALSE make it convenient to write "if-then-else" expressions in lambda calculus. For example, the predecessor function can be defined as:

PRED := λ_n_._n_ (λ_g_.λ_k_.ISZERO (_g_ 1) _k_ (PLUS (_g_ _k_) 1)) (λ_v_.0) 0

which can be verified by showing inductively that _n_ (λ_g_.λ_k_.ISZERO (_g_ 1) _k_ (PLUS (_g_ _k_) 1)) (λ_v_.0) is the add _n_ − 1 function for _n_ > 0.

### Pairs\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=26 "Edit section: Pairs")\]

A pair (2-tuple) can be defined in terms of TRUE and FALSE, by using the [Church encoding for pairs](https://en.wikipedia.org/wiki/Church_encoding#Church_pairs "Church encoding"). For example, PAIR encapsulates the pair (_x_,_y_), FIRST returns the first element of the pair, and SECOND returns the second.

PAIR := λ_x_.λ_y_.λ_f_._f_ _x_ _y_

FIRST := λ_p_._p_ TRUE

SECOND := λ_p_._p_ FALSE

NIL := λ_x_.TRUE

NULL := λ_p_._p_ (λ_x_.λ_y_.FALSE)

A linked list can be defined as either NIL for the empty list, or the PAIR of an element and a smaller list. The predicate NULL tests for the value NIL. (Alternatively, with NIL := FALSE, the construct _l_ (λ_h_.λ_t_.λ_z_.deal\_with\_head\__h_\_and\_tail\__t_) (deal\_with\_nil) obviates the need for an explicit NULL test).

As an example of the use of pairs, the shift-and-increment function that maps (_m_, _n_) to (_n_, _n_ + 1) can be defined as

Φ := λ_x_.PAIR (SECOND _x_) (SUCC (SECOND _x_))

which allows us to give perhaps the most transparent version of the predecessor function:

PRED := λ_n_.FIRST (_n_ Φ (PAIR 0 0)).

## Additional programming techniques\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=27 "Edit section: Additional programming techniques")\]

There is a considerable body of [programming idioms](https://en.wikipedia.org/wiki/Programming_idiom "Programming idiom") for lambda calculus. Many of these were originally developed in the context of using lambda calculus as a foundation for [programming language semantics](https://en.wikipedia.org/wiki/Semantics_(computer_science) "Semantics (computer science)"), effectively using lambda calculus as a [low-level programming language](https://en.wikipedia.org/wiki/Low-level_programming_language "Low-level programming language"). Because several programming languages include the lambda calculus (or something very similar) as a fragment, these techniques also see use in practical programming, but may then be perceived as obscure or foreign.

### Named constants\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=28 "Edit section: Named constants")\]

In lambda calculus, a [library](https://en.wikipedia.org/wiki/Library_(computing) "Library (computing)") would take the form of a collection of previously defined functions, which as lambda-terms are merely particular constants. The pure lambda calculus does not have a concept of named constants since all atomic lambda-terms are variables, but one can emulate having named constants by setting aside a variable as the name of the constant, using abstraction to bind that variable in the main body, and apply that abstraction to the intended definition. Thus to use _f_ to mean _M_ (some explicit lambda-term) in _N_ (another lambda-term, the "main program"), one can say

(λ_f_._N_) _M_

Authors often introduce [syntactic sugar](https://en.wikipedia.org/wiki/Syntactic_sugar "Syntactic sugar"), such as let, to permit writing the above in the more intuitive order

let _f_ =_M_ in _N_

By chaining such definitions, one can write a lambda calculus "program" as zero or more function definitions, followed by one lambda-term using those functions that constitutes the main body of the program.

A notable restriction of this let is that the name _f_ is not defined in _M_, since _M_ is outside the scope of the abstraction binding _f_; this means a recursive function definition cannot be used as the _M_ with let. The more advanced letrec syntactic sugar construction that allows writing recursive function definitions in that naive style instead additionally employs fixed-point combinators.

### Recursion and fixed points\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=29 "Edit section: Recursion and fixed points")\]

[Recursion](https://en.wikipedia.org/wiki/Recursion "Recursion") is the definition of a function using the function itself. Lambda calculus cannot express this as directly as some other notations: all functions are anonymous in lambda calculus, so we can't refer to a value which is yet to be defined, inside the lambda term defining that same value. However, recursion can still be achieved by arranging for a lambda expression to receive itself as its argument value, for example in  (λ_x_._x_ _x_) _E_.

Consider the [factorial](https://en.wikipedia.org/wiki/Factorial "Factorial") function F(_n_) recursively defined by

F(_n_) = 1, if _n_ = 0; else _n_ × F(_n_ − 1).

In the lambda expression which is to represent this function, a _parameter_ (typically the first one) will be assumed to receive the lambda expression itself as its value, so that calling it – applying it to an argument – will amount to recursion. Thus to achieve recursion, the intended-as-self-referencing argument (called _r_ here) must always be passed to itself within the function body, at a call point:

G := λ_r_. λ_n_.(1, if _n_ = 0; else _n_ × (_r_ _r_ (_n_−1)))

with  _r_ _r_ _x_ = F _x_ = G _r_ _x_  to hold, so  _r_ = G  and

F := G G = (λ_x_._x_ _x_) G

The self-application achieves replication here, passing the function's lambda expression on to the next invocation as an argument value, making it available to be referenced and called there.

This solves it but requires re-writing each recursive call as self-application. We would like to have a generic solution, without a need for any re-writes:

G := λ_r_. λ_n_.(1, if _n_ = 0; else _n_ × (_r_ (_n_−1)))

with  _r_ _x_ = F _x_ = G _r_ _x_  to hold, so  _r_ = G _r_ =: FIX G  and

F := FIX G  where  FIX _g_ := (_r_ where _r_ = _g_ _r_) = _g_ (FIX _g_)

so that  FIX G = G (FIX G) = (λ_n_.(1, if _n_ = 0; else _n_ × ((FIX G) (_n_−1))))

Given a lambda term with first argument representing recursive call (e.g. G here), the _fixed-point_ combinator FIX will return a self-replicating lambda expression representing the recursive function (here, F). The function does not need to be explicitly passed to itself at any point, for the self-replication is arranged in advance, when it is created, to be done each time it is called. Thus the original lambda expression (FIX G) is re-created inside itself, at call-point, achieving [self-reference](https://en.wikipedia.org/wiki/Self-reference "Self-reference").

In fact, there are many possible definitions for this FIX operator, the simplest of them being:

**Y** := λ_g_.(λ_x_._g_ (_x_ _x_)) (λ_x_._g_ (_x_ _x_))

In the lambda calculus, **Y** _g_  is a fixed-point of _g_, as it expands to:

**Y** _g_

(λ_h_.(λ_x_._h_ (_x_ _x_)) (λ_x_._h_ (_x_ _x_))) _g_

(λ_x_._g_ (_x_ _x_)) (λ_x_._g_ (_x_ _x_))

_g_ ((λ_x_._g_ (_x_ _x_)) (λ_x_._g_ (_x_ _x_)))

_g_ (**Y** _g_)

Now, to perform our recursive call to the factorial function, we would simply call (**Y** G) _n_,  where _n_ is the number we are calculating the factorial of. Given _n_ = 4, for example, this gives:

(**Y** G) 4

G (**Y** G) 4

(λ_r_.λ_n_.(1, if _n_ = 0; else _n_ × (_r_ (_n_−1)))) (**Y** G) 4

(λ_n_.(1, if _n_ = 0; else _n_ × ((**Y** G) (_n_−1)))) 4

1, if 4 = 0; else 4 × ((**Y** G) (4−1))

4 × (G (**Y** G) (4−1))

4 × ((λ_n_.(1, if _n_ = 0; else _n_ × ((**Y** G) (_n_−1)))) (4−1))

4 × (1, if 3 = 0; else 3 × ((**Y** G) (3−1)))

4 × (3 × (G (**Y** G) (3−1)))

4 × (3 × ((λ_n_.(1, if _n_ = 0; else _n_ × ((**Y** G) (_n_−1)))) (3−1)))

4 × (3 × (1, if 2 = 0; else 2 × ((**Y** G) (2−1))))

4 × (3 × (2 × (G (**Y** G) (2−1))))

4 × (3 × (2 × ((λ_n_.(1, if _n_ = 0; else _n_ × ((**Y** G) (_n_−1)))) (2−1))))

4 × (3 × (2 × (1, if 1 = 0; else 1 × ((**Y** G) (1−1)))))

4 × (3 × (2 × (1 × (G (**Y** G) (1−1)))))

4 × (3 × (2 × (1 × ((λ_n_.(1, if _n_ = 0; else _n_ × ((**Y** G) (_n_−1)))) (1−1)))))

4 × (3 × (2 × (1 × (1, if 0 = 0; else 0 × ((**Y** G) (0−1))))))

4 × (3 × (2 × (1 × (1))))

24

Every recursively defined function can be seen as a fixed point of some suitably defined function closing over the recursive call with an extra argument, and therefore, using **Y**, every recursively defined function can be expressed as a lambda expression. In particular, we can now cleanly define the subtraction, multiplication and comparison predicate of natural numbers recursively.

### Standard terms\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=30 "Edit section: Standard terms")\]

Certain terms have commonly accepted names:[\[24\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-25)[\[25\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-26)[\[26\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-27)

**I** := λ_x_._x_

**S** := λ_x_.λ_y_.λ_z_._x_ _z_ (_y_ _z_)

**K** := λ_x_.λ_y_._x_

**B** := λ_x_.λ_y_.λ_z_._x_ (_y_ _z_)

**C** := λ_x_.λ_y_.λ_z_._x_ _z_ _y_

**W** := λ_x_.λ_y_._x_ _y_ _y_

**ω** or **Δ** := λ_x_._x_ _x_

**Ω** := **ω ω**

**I** is the identity function. **SK** and **BCKW** form complete [combinator calculus](https://en.wikipedia.org/wiki/Combinator_calculus "Combinator calculus") systems that can express any lambda term - see [the next section](https://en.wikipedia.org/wiki/Lambda_calculus#Abstraction_elimination). **Ω** is **Y** **I**, the smallest term that has no normal form. **Y** is standard and defined [above](https://en.wikipedia.org/wiki/Lambda_calculus#Y). TRUE and FALSE defined [above](https://en.wikipedia.org/wiki/Lambda_calculus#Logic_and_predicates) are commonly abbreviated as **T** and **F**.

### Abstraction elimination\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=31 "Edit section: Abstraction elimination")\]

If _N_ is a lambda-term without abstraction, but possibly containing named constants ([combinators](https://en.wikipedia.org/wiki/Combinatory_logic "Combinatory logic")), then there exists a lambda-term _T_(_x_,_N_) which is equivalent to λ_x_._N_ but lacks abstraction (except as part of the named constants, if these are considered non-atomic). This can also be viewed as anonymising variables, as _T_(_x_,_N_) removes all occurrences of _x_ from _N_, while still allowing argument values to be substituted into the positions where _N_ contains an _x_. The conversion function _T_ can be defined by:

_T_(_x_, _x_) := **I**

_T_(_x_, _N_) := **K** _N_ if _x_ is not free in _N_.

_T_(_x_, _M_ _N_) := **S** _T_(_x_, _M_) _T_(_x_, _N_)

In either case, a term of the form _T_(_x_,_N_) _P_ can reduce by having the initial combinator **I**, **K**, or **S** grab the argument _P_, just like β-reduction of (λ_x_._N_) _P_ would do. **I** returns that argument. **K** throws the argument away, just like (λ_x_._N_) would do if _x_ has no free occurrence in _N_. **S** passes the argument on to both subterms of the application, and then applies the result of the first to the result of the second.

The combinators **B** and **C** are similar to **S**, but pass the argument on to only one subterm of an application (**B** to the "argument" subterm and **C** to the "function" subterm), thus saving a subsequent **K** if there is no occurrence of _x_ in one subterm. In comparison to **B** and **C**, the **S** combinator actually conflates two functionalities: rearranging arguments, and duplicating an argument so that it may be used in two places. The **W** combinator does only the latter, yielding the [B, C, K, W system](https://en.wikipedia.org/wiki/B,_C,_K,_W_system "B, C, K, W system") as an alternative to [SKI combinator calculus](https://en.wikipedia.org/wiki/SKI_combinator_calculus "SKI combinator calculus").

## Typed lambda calculus\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=32 "Edit section: Typed lambda calculus")\]

A **typed lambda calculus** is a typed [formalism](https://en.wikipedia.org/wiki/Formalism_(mathematics) "Formalism (mathematics)") that uses the lambda-symbol (![\lambda ](https://wikimedia.org/api/rest_v1/media/math/render/svg/b43d0ea3c9c025af1be9128e62a18fa74bedda2a)) to denote anonymous function abstraction. In this context, types are usually objects of a syntactic nature that are assigned to lambda terms; the exact nature of a type depends on the calculus considered (see [Kinds of typed lambda calculi](https://en.wikipedia.org/wiki/Typed_lambda_calculus#Kinds_of_typed_lambda_calculi "Typed lambda calculus")). From a certain point of view, typed lambda calculi can be seen as refinements of the [untyped lambda calculus](https://en.wikipedia.org/wiki/Untyped_lambda_calculus "Untyped lambda calculus") but from another point of view, they can also be considered the more fundamental theory and _untyped lambda calculus_ a special case with only one type.[\[27\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-28)

Typed lambda calculi are foundational [programming languages](https://en.wikipedia.org/wiki/Programming_languages "Programming languages") and are the base of typed [functional programming languages](https://en.wikipedia.org/wiki/Functional_programming_languages "Functional programming languages") such as [ML](https://en.wikipedia.org/wiki/ML_programming_language "ML programming language") and [Haskell](https://en.wikipedia.org/wiki/Haskell_(programming_language) "Haskell (programming language)") and, more indirectly, typed [imperative programming](https://en.wikipedia.org/wiki/Imperative_programming "Imperative programming") languages. Typed lambda calculi play an important role in the design of [type systems](https://en.wikipedia.org/wiki/Type_systems "Type systems") for programming languages; here typability usually captures desirable properties of the program, e.g. the program will not cause a memory access violation.

Typed lambda calculi are closely related to [mathematical logic](https://en.wikipedia.org/wiki/Mathematical_logic "Mathematical logic") and [proof theory](https://en.wikipedia.org/wiki/Proof_theory "Proof theory") via the [Curry–Howard isomorphism](https://en.wikipedia.org/wiki/Curry%E2%80%93Howard_isomorphism "Curry–Howard isomorphism") and they can be considered as the [internal language](https://en.wikipedia.org/wiki/Internal_language "Internal language") of classes of [categories](https://en.wikipedia.org/wiki/Category_theory "Category theory"), e.g. the simply typed lambda calculus is the language of [Cartesian closed categories](https://en.wikipedia.org/wiki/Cartesian_closed_category "Cartesian closed category") (CCCs).

## Reduction strategies\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=33 "Edit section: Reduction strategies")\]

Whether a term is normalising or not, and how much work needs to be done in normalising it if it is, depends to a large extent on the reduction strategy used. Common lambda calculus reduction strategies include:[\[28\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-29)

Normal order

The leftmost, outermost redex is always reduced first. That is, whenever possible the arguments are substituted into the body of an abstraction before the arguments are reduced.

Applicative order

The leftmost, innermost redex is always reduced first. Intuitively this means a function's arguments are always reduced before the function itself. Applicative order always attempts to apply functions to normal forms, even when this is not possible.

Full β-reductions

Any redex can be reduced at any time. This means essentially the lack of any particular reduction strategy—with regard to reducibility, "all bets are off".

Weak reduction strategies do not reduce under lambda abstractions:

Call by value

A redex is reduced only when its right hand side has reduced to a value (variable or abstraction). Only the outermost redexes are reduced.

Call by name

As normal order, but no reductions are performed inside abstractions. For example, λ_x_.(λ_x_._x_)_x_ is in normal form according to this strategy, although it contains the redex (λ_x_._x_)_x_.

Strategies with sharing reduce computations that are "the same" in parallel:

Optimal reduction

As normal order, but computations that have the same label are reduced simultaneously.

Call by need

As call by name (hence weak), but function applications that would duplicate terms instead name the argument, which is then reduced only "when it is needed".

## Computability\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=34 "Edit section: Computability")\]

There is no algorithm that takes as input any two lambda expressions and outputs TRUE or FALSE depending on whether one expression reduces to the other.[\[10\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-Church1936-11) More precisely, no [computable function](https://en.wikipedia.org/wiki/Computable_function "Computable function") can [decide](https://en.wikipedia.org/wiki/Decision_problem "Decision problem") the question. This was historically the first problem for which undecidability could be proven. As usual for such a proof, _computable_ means computable by any [model of computation](https://en.wikipedia.org/wiki/Model_of_computation "Model of computation") that is [Turing complete](https://en.wikipedia.org/wiki/Turing_complete "Turing complete"). In fact computability can itself be defined via the lambda calculus: a function _F_: **N** → **N** of natural numbers is a computable function if and only if there exists a lambda expression _f_ such that for every pair of _x_, _y_ in **N**, _F_(_x_)=_y_ if and only if _f_ _x_ =β _y_,  where _x_ and _y_ are the Church numerals corresponding to _x_ and _y_, respectively and =β meaning equivalence with β-reduction. See the [Church–Turing thesis](https://en.wikipedia.org/wiki/Church%E2%80%93Turing_thesis "Church–Turing thesis") for other approaches to defining computability and their equivalence.

Church's proof of uncomputability first reduces the problem to determining whether a given lambda expression has a [normal form](https://en.wikipedia.org/wiki/Beta_normal_form "Beta normal form"). Then he assumes that this predicate is computable, and can hence be expressed in lambda calculus. Building on earlier work by Kleene and constructing a [Gödel numbering](https://en.wikipedia.org/wiki/G%C3%B6del_numbering "Gödel numbering") for lambda expressions, he constructs a lambda expression _e_ that closely follows the proof of [Gödel's first incompleteness theorem](https://en.wikipedia.org/wiki/G%C3%B6del%27s_incompleteness_theorems "Gödel's incompleteness theorems"). If _e_ is applied to its own Gödel number, a contradiction results.

## Complexity\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=35 "Edit section: Complexity")\]

The notion of [computational complexity](https://en.wikipedia.org/wiki/Computational_complexity_theory "Computational complexity theory") for the lambda calculus is a bit tricky, because the cost of a β-reduction may vary depending on how it is implemented.[\[29\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-30) To be precise, one must somehow find the location of all of the occurrences of the bound variable _V_ in the expression _E_, implying a time cost, or one must keep track of the locations of free variables in some way, implying a space cost. A naïve search for the locations of _V_ in _E_ is [_O_(_n_)](https://en.wikipedia.org/wiki/Big_O_notation "Big O notation") in the length _n_ of _E_. [Director strings](https://en.wikipedia.org/wiki/Director_string "Director string") were an early approach that traded this time cost for a quadratic space usage.[\[30\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-31) More generally this has led to the study of systems that use [explicit substitution](https://en.wikipedia.org/wiki/Explicit_substitution "Explicit substitution").

In 2014 it was shown that the number of β-reduction steps taken by normal order reduction to reduce a term is a _reasonable_ time cost model, that is, the reduction can be simulated on a Turing machine in time polynomially proportional to the number of steps.[\[31\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-32) This was a long-standing open problem, due to _size explosion_, the existence of lambda terms which grow exponentially in size for each β-reduction. The result gets around this by working with a compact shared representation. The result makes clear that the amount of space needed to evaluate a lambda term is not proportional to the size of the term during reduction. It is not currently known what a good measure of space complexity would be.[\[32\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-Reasonable-33)

An unreasonable model does not necessarily mean inefficient. [Optimal reduction](https://en.wikipedia.org/wiki/Reduction_strategy#Optimal_reduction "Reduction strategy") reduces all computations with the same label in one step, avoiding duplicated work, but the number of parallel β-reduction steps to reduce a given term to normal form is approximately linear in the size of the term. This is far too small to be a reasonable cost measure, as any Turing machine may be encoded in the lambda calculus in size linearly proportional to the size of the Turing machine. The true cost of reducing lambda terms is not due to β-reduction per se but rather the handling of the duplication of redexes during β-reduction.[\[33\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-Asperti-34) It is not known if optimal reduction implementations are reasonable when measured with respect to a reasonable cost model such as the number of leftmost-outermost steps to normal form, but it has been shown for fragments of the lambda calculus that the optimal reduction algorithm is efficient and has at most a quadratic overhead compared to leftmost-outermost.[\[32\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-Reasonable-33) In addition the BOHM prototype implementation of optimal reduction outperformed both [Caml Light](https://en.wikipedia.org/wiki/Caml "Caml") and [Haskell](https://en.wikipedia.org/wiki/Haskell_(programming_language) "Haskell (programming language)") on pure lambda terms.[\[33\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-Asperti-34)

## Lambda calculus and programming languages\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=36 "Edit section: Lambda calculus and programming languages")\]

As pointed out by [Peter Landin](https://en.wikipedia.org/wiki/Peter_Landin "Peter Landin")'s 1965 paper "A Correspondence between ALGOL 60 and Church's Lambda-notation",[\[34\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-35) sequential [procedural programming](https://en.wikipedia.org/wiki/Procedural_programming "Procedural programming") languages can be understood in terms of the lambda calculus, which provides the basic mechanisms for procedural abstraction and procedure (subprogram) application.

### Anonymous functions\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=37 "Edit section: Anonymous functions")\]

For example, in [Lisp](https://en.wikipedia.org/wiki/Lisp_(programming_language) "Lisp (programming language)") the "square" function can be expressed as a lambda expression as follows:

The above example is an expression that evaluates to a first-class function. The symbol `lambda` creates an anonymous function, given a list of parameter names, `(x)` – just a single argument in this case, and an expression that is evaluated as the body of the function, `(* x x)`. Anonymous functions are sometimes called lambda expressions.

For example, [Pascal](https://en.wikipedia.org/wiki/Pascal_(programming_language) "Pascal (programming language)") and many other imperative languages have long supported passing [subprograms](https://en.wikipedia.org/wiki/Subprograms "Subprograms") as [arguments](https://en.wikipedia.org/wiki/Arguments "Arguments") to other subprograms through the mechanism of [function pointers](https://en.wikipedia.org/wiki/Function_pointers "Function pointers"). However, function pointers are not a sufficient condition for functions to be [first class](https://en.wikipedia.org/wiki/First-class_function "First-class function") datatypes, because a function is a first class datatype if and only if new instances of the function can be created at run-time. And this run-time creation of functions is supported in [Smalltalk](https://en.wikipedia.org/wiki/Smalltalk "Smalltalk"), [JavaScript](https://en.wikipedia.org/wiki/JavaScript "JavaScript") and [Wolfram Language](https://en.wikipedia.org/wiki/Wolfram_Language "Wolfram Language"), and more recently in [Scala](https://en.wikipedia.org/wiki/Scala_(programming_language) "Scala (programming language)"), [Eiffel](https://en.wikipedia.org/wiki/Eiffel_(programming_language) "Eiffel (programming language)") ("agents"), [C#](https://en.wikipedia.org/wiki/C_Sharp_(programming_language) "C Sharp (programming language)") ("delegates") and [C++11](https://en.wikipedia.org/wiki/C%2B%2B11 "C++11"), among others.

### Parallelism and concurrency\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=38 "Edit section: Parallelism and concurrency")\]

The [Church–Rosser](https://en.wikipedia.org/wiki/Church%E2%80%93Rosser_theorem "Church–Rosser theorem") property of the lambda calculus means that evaluation (β-reduction) can be carried out in _any order_, even in parallel. This means that various [nondeterministic evaluation strategies](https://en.wikipedia.org/wiki/Evaluation_strategy#Nondeterministic_strategies "Evaluation strategy") are relevant. However, the lambda calculus does not offer any explicit constructs for [parallelism](https://en.wikipedia.org/wiki/Parallel_computing "Parallel computing"). One can add constructs such as [Futures](https://en.wikipedia.org/wiki/Futures_and_promises "Futures and promises") to the lambda calculus. Other [process calculi](https://en.wikipedia.org/wiki/Process_calculi "Process calculi") have been developed for describing communication and concurrency.

## Semantics\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=39 "Edit section: Semantics")\]

The fact that lambda calculus terms act as functions on other lambda calculus terms, and even on themselves, led to questions about the semantics of the lambda calculus. Could a sensible meaning be assigned to lambda calculus terms? The natural semantics was to find a set _D_ isomorphic to the function space _D_ → _D_, of functions on itself. However, no nontrivial such _D_ can exist, by [cardinality](https://en.wikipedia.org/wiki/Cardinality "Cardinality") constraints because the set of all functions from _D_ to _D_ has greater cardinality than _D_, unless _D_ is a [singleton set](https://en.wikipedia.org/wiki/Singleton_set "Singleton set").

In the 1970s, [Dana Scott](https://en.wikipedia.org/wiki/Dana_Scott "Dana Scott") showed that if only [continuous functions](https://en.wikipedia.org/wiki/Scott_continuity "Scott continuity") were considered, a set or [domain](https://en.wikipedia.org/wiki/Domain_theory "Domain theory") _D_ with the required property could be found, thus providing a [model](https://en.wikipedia.org/wiki/Model_theory "Model theory") for the lambda calculus.

This work also formed the basis for the [denotational semantics](https://en.wikipedia.org/wiki/Denotational_semantics "Denotational semantics") of programming languages.

## Variations and extensions\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=40 "Edit section: Variations and extensions")\]

These extensions are in the [lambda cube](https://en.wikipedia.org/wiki/Lambda_cube "Lambda cube"):

-   [Typed lambda calculus](https://en.wikipedia.org/wiki/Typed_lambda_calculus "Typed lambda calculus") – Lambda calculus with typed variables (and functions)
-   [System F](https://en.wikipedia.org/wiki/System_F "System F") – A typed lambda calculus with type-variables
-   [Calculus of constructions](https://en.wikipedia.org/wiki/Calculus_of_constructions "Calculus of constructions") – A typed lambda calculus with [types](https://en.wikipedia.org/wiki/Type_system "Type system") as first-class values

These [formal systems](https://en.wikipedia.org/wiki/Formal_system "Formal system") are extensions of lambda calculus that are not in the lambda cube:

-   [Binary lambda calculus](https://en.wikipedia.org/wiki/Binary_lambda_calculus "Binary lambda calculus") – A version of lambda calculus with binary I/O, a binary encoding of terms, and a designated universal machine.
-   [Lambda-mu calculus](https://en.wikipedia.org/wiki/Lambda-mu_calculus "Lambda-mu calculus") – An extension of the lambda calculus for treating [classical logic](https://en.wikipedia.org/wiki/Classical_logic "Classical logic")

These formal systems are variations of lambda calculus:

-   [Kappa calculus](https://en.wikipedia.org/wiki/Kappa_calculus "Kappa calculus") – A first-order analogue of lambda calculus

These formal systems are related to lambda calculus:

-   [Combinatory logic](https://en.wikipedia.org/wiki/Combinatory_logic "Combinatory logic") – A notation for mathematical logic without variables
-   [SKI combinator calculus](https://en.wikipedia.org/wiki/SKI_combinator_calculus "SKI combinator calculus") – A computational system based on the **[S](https://en.wikipedia.org/wiki/Lambda_calculus#S)**, **[K](https://en.wikipedia.org/wiki/Lambda_calculus#K)** and **[I](https://en.wikipedia.org/wiki/Lambda_calculus#I)** combinators, equivalent to lambda calculus, but reducible without variable substitutions

## See also\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=41 "Edit section: See also")\]

-   [Applicative computing systems](https://en.wikipedia.org/wiki/Applicative_computing_systems "Applicative computing systems") – Treatment of [objects](https://en.wikipedia.org/wiki/Object_(computer_science) "Object (computer science)") in the style of the lambda calculus
-   [Cartesian closed category](https://en.wikipedia.org/wiki/Cartesian_closed_category "Cartesian closed category") – A setting for lambda calculus in [category theory](https://en.wikipedia.org/wiki/Category_theory "Category theory")
-   [Categorical abstract machine](https://en.wikipedia.org/wiki/Categorical_abstract_machine "Categorical abstract machine") – A [model of computation](https://en.wikipedia.org/wiki/Model_of_computation "Model of computation") applicable to lambda calculus
-   [Curry–Howard isomorphism](https://en.wikipedia.org/wiki/Curry%E2%80%93Howard_isomorphism "Curry–Howard isomorphism") – The formal correspondence between programs and [proofs](https://en.wikipedia.org/wiki/Mathematical_proof "Mathematical proof")
-   [De Bruijn index](https://en.wikipedia.org/wiki/De_Bruijn_index "De Bruijn index") – notation disambiguating alpha conversions
-   [De Bruijn notation](https://en.wikipedia.org/wiki/De_Bruijn_notation "De Bruijn notation") – notation using postfix modification functions
-   [Deductive lambda calculus](https://en.wikipedia.org/wiki/Deductive_lambda_calculus "Deductive lambda calculus") – The consideration of the problems associated with considering lambda calculus as a [Deductive system](https://en.wikipedia.org/wiki/Deductive_system "Deductive system").
-   [Domain theory](https://en.wikipedia.org/wiki/Domain_theory "Domain theory") – Study of certain [posets](https://en.wikipedia.org/wiki/Partially_ordered_sets "Partially ordered sets") giving [denotational semantics](https://en.wikipedia.org/wiki/Denotational_semantics "Denotational semantics") for lambda calculus
-   [Evaluation strategy](https://en.wikipedia.org/wiki/Evaluation_strategy "Evaluation strategy") – Rules for the evaluation of expressions in [programming languages](https://en.wikipedia.org/wiki/Programming_language "Programming language")
-   [Explicit substitution](https://en.wikipedia.org/wiki/Explicit_substitution "Explicit substitution") – The theory of substitution, as used in [β-reduction](https://en.wikipedia.org/wiki/Lambda_calculus#%CE%B2-reduction)
-   [Functional programming](https://en.wikipedia.org/wiki/Functional_programming "Functional programming")
-   [Harrop formula](https://en.wikipedia.org/wiki/Harrop_formula "Harrop formula") – A kind of constructive logical formula such that proofs are lambda terms
-   [Interaction nets](https://en.wikipedia.org/wiki/Interaction_nets "Interaction nets")
-   [Kleene–Rosser paradox](https://en.wikipedia.org/wiki/Kleene%E2%80%93Rosser_paradox "Kleene–Rosser paradox") – A demonstration that some form of lambda calculus is inconsistent
-   [Knights of the Lambda Calculus](https://en.wikipedia.org/wiki/Knights_of_the_Lambda_Calculus "Knights of the Lambda Calculus") – A semi-fictional organization of LISP and [Scheme](https://en.wikipedia.org/wiki/Scheme_(programming_language) "Scheme (programming language)") [hackers](https://en.wikipedia.org/wiki/Hacker_(programmer_subculture) "Hacker (programmer subculture)")
-   [Krivine machine](https://en.wikipedia.org/wiki/Krivine_machine "Krivine machine") – An abstract machine to interpret call-by-name in lambda calculus
-   [Lambda calculus definition](https://en.wikipedia.org/wiki/Lambda_calculus_definition "Lambda calculus definition") – Formal definition of the lambda calculus.
-   [Let expression](https://en.wikipedia.org/wiki/Let_expression "Let expression") – An expression closely related to an abstraction.
-   [Minimalism (computing)](https://en.wikipedia.org/wiki/Minimalism_(computing) "Minimalism (computing)")
-   [Rewriting](https://en.wikipedia.org/wiki/Rewriting "Rewriting") – Transformation of formulæ in formal systems
-   [SECD machine](https://en.wikipedia.org/wiki/SECD_machine "SECD machine") – A [virtual machine](https://en.wikipedia.org/wiki/Virtual_machine "Virtual machine") designed for the lambda calculus
-   [Scott–Curry theorem](https://en.wikipedia.org/wiki/Scott%E2%80%93Curry_theorem "Scott–Curry theorem") – A theorem about sets of lambda terms
-   _[To Mock a Mockingbird](https://en.wikipedia.org/wiki/To_Mock_a_Mockingbird "To Mock a Mockingbird")_ – An introduction to [combinatory logic](https://en.wikipedia.org/wiki/Combinatory_logic "Combinatory logic")
-   [Universal Turing machine](https://en.wikipedia.org/wiki/Universal_Turing_machine "Universal Turing machine") – A formal computing machine that is equivalent to lambda calculus
-   [Unlambda](https://en.wikipedia.org/wiki/Unlambda "Unlambda") – An [esoteric](https://en.wikipedia.org/wiki/Esoteric_programming_language "Esoteric programming language") functional programming language based on combinatory logic

## Notes\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=42 "Edit section: Notes")\]

1.  **[^](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-8 "Jump up")** For a full history, see Cardone and Hindley's "History of Lambda-calculus and Combinatory Logic" (2006).

## References\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=43 "Edit section: References")\]

1.  **[^](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-1 "Jump up")** [Turing, Alan M.](https://en.wikipedia.org/wiki/Alan_Turing "Alan Turing") (December 1937). "Computability and λ-Definability". _The Journal of Symbolic Logic_. **2** (4): 153–163. [doi](https://en.wikipedia.org/wiki/Doi_(identifier) "Doi (identifier)"):[10.2307/2268280](https://doi.org/10.2307%2F2268280). [JSTOR](https://en.wikipedia.org/wiki/JSTOR_(identifier) "JSTOR (identifier)") [2268280](https://www.jstor.org/stable/2268280).
2.  **[^](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-2 "Jump up")** [Coquand, Thierry](https://en.wikipedia.org/wiki/Thierry_Coquand "Thierry Coquand") (8 February 2006). Zalta, Edward N. (ed.). ["Type Theory"](http://plato.stanford.edu/archives/sum2013/entries/type-theory/). _The Stanford Encyclopedia of Philosophy_ (Summer 2013 ed.). Retrieved November 17, 2020.
3.  **[^](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-3 "Jump up")** Moortgat, Michael (1988). [_Categorial Investigations: Logical and Linguistic Aspects of the Lambek Calculus_](https://books.google.com/books?id=9CdFE9X_FCoC). Foris Publications. [ISBN](https://en.wikipedia.org/wiki/ISBN_(identifier) "ISBN (identifier)") [9789067653879](https://en.wikipedia.org/wiki/Special:BookSources/9789067653879 "Special:BookSources/9789067653879").
4.  **[^](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-4 "Jump up")** Bunt, Harry; Muskens, Reinhard, eds. (2008). [_Computing Meaning_](https://books.google.com/books?id=nyFa5ngYThMC). Springer. [ISBN](https://en.wikipedia.org/wiki/ISBN_(identifier) "ISBN (identifier)") [978-1-4020-5957-5](https://en.wikipedia.org/wiki/Special:BookSources/978-1-4020-5957-5 "Special:BookSources/978-1-4020-5957-5").
5.  **[^](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-5 "Jump up")** [Mitchell, John C.](https://en.wikipedia.org/wiki/John_C._Mitchell "John C. Mitchell") (2003). [_Concepts in Programming Languages_](https://books.google.com/books?id=7Uh8XGfJbEIC&pg=PA57). Cambridge University Press. p. 57. [ISBN](https://en.wikipedia.org/wiki/ISBN_(identifier) "ISBN (identifier)") [978-0-521-78098-8](https://en.wikipedia.org/wiki/Special:BookSources/978-0-521-78098-8 "Special:BookSources/978-0-521-78098-8")..
6.  **[^](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-6 "Jump up")** [Pierce, Benjamin C.](https://en.wikipedia.org/wiki/Benjamin_C._Pierce "Benjamin C. Pierce") _Basic Category Theory for Computer Scientists_. p. 53.
7.  **[^](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-7 "Jump up")** [Church, Alonzo](https://en.wikipedia.org/wiki/Alonzo_Church "Alonzo Church") (1932). "A set of postulates for the foundation of logic". _Annals of Mathematics_. Series 2. **33** (2): 346–366. [doi](https://en.wikipedia.org/wiki/Doi_(identifier) "Doi (identifier)"):[10.2307/1968337](https://doi.org/10.2307%2F1968337). [JSTOR](https://en.wikipedia.org/wiki/JSTOR_(identifier) "JSTOR (identifier)") [1968337](https://www.jstor.org/stable/1968337).
8.  **[^](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-9 "Jump up")** [Kleene, Stephen C.](https://en.wikipedia.org/wiki/Stephen_Kleene "Stephen Kleene"); [Rosser, J. B.](https://en.wikipedia.org/wiki/J._B._Rosser "J. B. Rosser") (July 1935). "The Inconsistency of Certain Formal Logics". _The Annals of Mathematics_. **36** (3): 630. [doi](https://en.wikipedia.org/wiki/Doi_(identifier) "Doi (identifier)"):[10.2307/1968646](https://doi.org/10.2307%2F1968646). [JSTOR](https://en.wikipedia.org/wiki/JSTOR_(identifier) "JSTOR (identifier)") [1968646](https://www.jstor.org/stable/1968646).
9.  **[^](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-10 "Jump up")** [Church, Alonzo](https://en.wikipedia.org/wiki/Alonzo_Church "Alonzo Church") (December 1942). "Review of Haskell B. Curry, _The Inconsistency of Certain Formal Logics_". _The Journal of Symbolic Logic_. **7** (4): 170–171. [doi](https://en.wikipedia.org/wiki/Doi_(identifier) "Doi (identifier)"):[10.2307/2268117](https://doi.org/10.2307%2F2268117). [JSTOR](https://en.wikipedia.org/wiki/JSTOR_(identifier) "JSTOR (identifier)") [2268117](https://www.jstor.org/stable/2268117).
10.  ^ [Jump up to: _**a**_](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-Church1936_11-0) [_**b**_](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-Church1936_11-1) [Church, Alonzo](https://en.wikipedia.org/wiki/Alonzo_Church "Alonzo Church") (1936). "An unsolvable problem of elementary number theory". _American Journal of Mathematics_. **58** (2): 345–363. [doi](https://en.wikipedia.org/wiki/Doi_(identifier) "Doi (identifier)"):[10.2307/2371045](https://doi.org/10.2307%2F2371045). [JSTOR](https://en.wikipedia.org/wiki/JSTOR_(identifier) "JSTOR (identifier)") [2371045](https://www.jstor.org/stable/2371045).
11.  **[^](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-12 "Jump up")** [Church, Alonzo](https://en.wikipedia.org/wiki/Alonzo_Church "Alonzo Church") (1940). "A Formulation of the Simple Theory of Types". _Journal of Symbolic Logic_. **5** (2): 56–68. [doi](https://en.wikipedia.org/wiki/Doi_(identifier) "Doi (identifier)"):[10.2307/2266170](https://doi.org/10.2307%2F2266170). [JSTOR](https://en.wikipedia.org/wiki/JSTOR_(identifier) "JSTOR (identifier)") [2266170](https://www.jstor.org/stable/2266170).
12.  **[^](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-mm-linguistics_13-0 "Jump up")** Partee, B. B. H.; [ter Meulen, A.](https://en.wikipedia.org/wiki/Alice_ter_Meulen "Alice ter Meulen"); Wall, R. E. (1990). [_Mathematical Methods in Linguistics_](https://books.google.com/books?id=qV7TUuaYcUIC&pg=PA317). Springer. [ISBN](https://en.wikipedia.org/wiki/ISBN_(identifier) "ISBN (identifier)") [9789027722454](https://en.wikipedia.org/wiki/Special:BookSources/9789027722454 "Special:BookSources/9789027722454"). Retrieved 29 Dec 2016.
13.  **[^](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-14 "Jump up")** Alma, Jesse. Zalta, Edward N. (ed.). ["The Lambda Calculus"](http://plato.stanford.edu/entries/lambda-calculus/). _The Stanford Encyclopedia of Philosophy_ (Summer 2013 ed.). Retrieved November 17, 2020.
14.  **[^](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-15 "Jump up")** Dana Scott, "[Looking Backward; Looking Forward](https://www.youtube.com/embed/uS9InrmPIoc)", Invited Talk at the Workshop in honour of Dana Scott’s 85th birthday and 50 years of domain theory, 7–8 July, FLoC 2018 (talk 7 July 2018). The relevant passage begins at [32:50](https://www.youtube.com/embed/uS9InrmPIoc?start=1970). (See also this [extract of a May 2016 talk](https://www.youtube.com/watch?time_continue=1&v=juXwu0Nqc3I) at the University of Birmingham, UK.)
15.  **[^](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-tfp12_16-0 "Jump up")** ["D. A. Turner "Some History of Functional Programming Languages" in an invited lecture **TFP12**, St Andrews University, 12 June 2012. See the section on Algol 60"](https://www.cs.kent.ac.uk/people/staff/dat/tfp12/tfp12.pdf) (PDF).
16.  **[^](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-17 "Jump up")** [Barendregt, Hendrik Pieter](https://en.wikipedia.org/wiki/Henk_Barendregt "Henk Barendregt") (1984). [_The Lambda Calculus: Its Syntax and Semantics_](https://www.elsevier.com/books/the-lambda-calculus/barendregt/978-0-444-87508-2). Studies in Logic and the Foundations of Mathematics. Vol. 103 (Revised ed.). North Holland. [ISBN](https://en.wikipedia.org/wiki/ISBN_(identifier) "ISBN (identifier)") [0-444-87508-5](https://en.wikipedia.org/wiki/Special:BookSources/0-444-87508-5 "Special:BookSources/0-444-87508-5").
17.  **[^](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-18 "Jump up")** [Corrections](ftp://ftp.cs.ru.nl/pub/CompMath.Found/ErrataLCalculus.pdf).
18.  ^ [Jump up to: _**a**_](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-lambda-bound_19-0) [_**b**_](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-lambda-bound_19-1) ["Example for Rules of Associativity"](http://www.lambda-bound.com/book/lambdacalc/node27.html). Lambda-bound.com. Retrieved 2012-06-18.
19.  ^ [Jump up to: _**a**_](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-Selinger_20-0) [_**b**_](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-Selinger_20-1) Selinger, Peter (2008), [_Lecture Notes on the Lambda Calculus_](http://www.mathstat.dal.ca/~selinger/papers/lambdanotes.pdf) (PDF), vol. 0804, Department of Mathematics and Statistics, University of Ottawa, p. 9, [arXiv](https://en.wikipedia.org/wiki/ArXiv_(identifier) "ArXiv (identifier)"):[0804.3434](https://arxiv.org/abs/0804.3434), [Bibcode](https://en.wikipedia.org/wiki/Bibcode_(identifier) "Bibcode (identifier)"):[2008arXiv0804.3434S](https://ui.adsabs.harvard.edu/abs/2008arXiv0804.3434S)
20.  ^ [Jump up to: _**a**_](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-BarendregtBarendsen_21-0) [_**b**_](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-BarendregtBarendsen_21-1) [Barendregt, Henk](https://en.wikipedia.org/wiki/Henk_Barendregt "Henk Barendregt"); Barendsen, Erik (March 2000), [_Introduction to Lambda Calculus_](ftp://ftp.cs.ru.nl/pub/CompMath.Found/lambda.pdf) (PDF)
21.  **[^](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-22 "Jump up")** [de Queiroz, Ruy J. G. B.](https://en.wikipedia.org/wiki/Ruy_de_Queiroz "Ruy de Queiroz") (1988). "A Proof-Theoretic Account of Programming and the Role of Reduction Rules". _Dialectica_. **42** (4): 265–282. [doi](https://en.wikipedia.org/wiki/Doi_(identifier) "Doi (identifier)"):[10.1111/j.1746-8361.1988.tb00919.x](https://doi.org/10.1111%2Fj.1746-8361.1988.tb00919.x).
22.  **[^](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-23 "Jump up")** Turbak, Franklyn; Gifford, David (2008), _Design concepts in programming languages_, MIT press, p. 251, [ISBN](https://en.wikipedia.org/wiki/ISBN_(identifier) "ISBN (identifier)") [978-0-262-20175-9](https://en.wikipedia.org/wiki/Special:BookSources/978-0-262-20175-9 "Special:BookSources/978-0-262-20175-9")
23.  **[^](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-24 "Jump up")** Felleisen, Matthias; Flatt, Matthew (2006), [_Programming Languages and Lambda Calculi_](https://web.archive.org/web/20090205113235/http://www.cs.utah.edu/plt/publications/pllc.pdf) (PDF), p. 26, archived from [the original](http://www.cs.utah.edu/plt/publications/pllc.pdf) (PDF) on 2009-02-05; A note (accessed 2017) at the original location suggests that the authors consider the work originally referenced to have been superseded by a book.
24.  **[^](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-25 "Jump up")** Ker, Andrew D. ["Lambda Calculus and Types"](https://www.cs.ox.ac.uk/andrew.ker/docs/lambdacalculus-lecture-notes-ht2009.pdf#page=18) (PDF). p. 6. Retrieved 14 January 2022.
25.  **[^](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-26 "Jump up")** Dezani-Ciancaglini, Mariangiola; Ghilezan, Silvia (2014). ["Preciseness of Subtyping on Intersection and Union Types"](http://www.di.unito.it/~dezani/papers/dg14.pdf#page=3) (PDF). _Rewriting and Typed Lambda Calculi_. Lecture Notes in Computer Science. **8560**: 196. [doi](https://en.wikipedia.org/wiki/Doi_(identifier) "Doi (identifier)"):[10.1007/978-3-319-08918-8\_14](https://doi.org/10.1007%2F978-3-319-08918-8_14). [hdl](https://en.wikipedia.org/wiki/Hdl_(identifier) "Hdl (identifier)"):[2318/149874](https://hdl.handle.net/2318%2F149874). [ISBN](https://en.wikipedia.org/wiki/ISBN_(identifier) "ISBN (identifier)") [978-3-319-08917-1](https://en.wikipedia.org/wiki/Special:BookSources/978-3-319-08917-1 "Special:BookSources/978-3-319-08917-1"). Retrieved 14 January 2022.
26.  **[^](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-27 "Jump up")** Forster, Yannick; Smolka, Gert (August 2019). ["Call-by-Value Lambda Calculus as a Model of Computation in Coq"](https://www.ps.uni-saarland.de/Publications/documents/ForsterSmolka_2018_Computability-JAR.pdf#page=4) (PDF). _Journal of Automated Reasoning_. **63** (2): 393–413. [doi](https://en.wikipedia.org/wiki/Doi_(identifier) "Doi (identifier)"):[10.1007/s10817-018-9484-2](https://doi.org/10.1007%2Fs10817-018-9484-2). [S2CID](https://en.wikipedia.org/wiki/S2CID_(identifier) "S2CID (identifier)") [53087112](https://api.semanticscholar.org/CorpusID:53087112). Retrieved 14 January 2022.
27.  **[^](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-28 "Jump up")** Types and Programming Languages, p. 273, Benjamin C. Pierce
28.  **[^](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-29 "Jump up")** [Pierce, Benjamin C.](https://en.wikipedia.org/wiki/Benjamin_C._Pierce "Benjamin C. Pierce") (2002). [_Types and Programming Languages_](https://www.google.com/books/edition/Types_and_Programming_Languages/ti6zoAC9Ph8C?hl=en&pg=PA56). [MIT Press](https://en.wikipedia.org/wiki/MIT_Press "MIT Press"). p. 56. [ISBN](https://en.wikipedia.org/wiki/ISBN_(identifier) "ISBN (identifier)") [0-262-16209-1](https://en.wikipedia.org/wiki/Special:BookSources/0-262-16209-1 "Special:BookSources/0-262-16209-1").
29.  **[^](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-30 "Jump up")** Frandsen, Gudmund Skovbjerg; Sturtivant, Carl (26 August 1991). ["What is an Efficient Implementation of the \\lambda-calculus?"](https://dl.acm.org/doi/10.5555/645420.652523). _Proceedings of the 5th ACM Conference on Functional Programming Languages and Computer Architecture_. Lecture Notes in Computer Science. Springer-Verlag. **523**: 289–312. [CiteSeerX](https://en.wikipedia.org/wiki/CiteSeerX_(identifier) "CiteSeerX (identifier)") [10.1.1.139.6913](https://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.139.6913). [doi](https://en.wikipedia.org/wiki/Doi_(identifier) "Doi (identifier)"):[10.1007/3540543961\_14](https://doi.org/10.1007%2F3540543961_14). [ISBN](https://en.wikipedia.org/wiki/ISBN_(identifier) "ISBN (identifier)") [9783540543961](https://en.wikipedia.org/wiki/Special:BookSources/9783540543961 "Special:BookSources/9783540543961").
30.  **[^](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-31 "Jump up")** Sinot, F.-R. (2005). ["Director Strings Revisited: A Generic Approach to the Efficient Representation of Free Variables in Higher-order Rewriting"](http://www.lsv.fr/Publis/PAPERS/PDF/sinot-jlc05.pdf) (PDF). _Journal of Logic and Computation_. **15** (2): 201–218. [doi](https://en.wikipedia.org/wiki/Doi_(identifier) "Doi (identifier)"):[10.1093/logcom/exi010](https://doi.org/10.1093%2Flogcom%2Fexi010).
31.  **[^](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-32 "Jump up")** Accattoli, Beniamino; Dal Lago, Ugo (14 July 2014). ["Beta reduction is invariant, indeed"](https://arxiv.org/pdf/1601.01233.pdf) (PDF). _Proceedings of the Joint Meeting of the Twenty-Third EACSL Annual Conference on Computer Science Logic (CSL) and the Twenty-Ninth Annual ACM/IEEE Symposium on Logic in Computer Science (LICS)_: 1–10. [arXiv](https://en.wikipedia.org/wiki/ArXiv_(identifier) "ArXiv (identifier)"):[1601.01233](https://arxiv.org/abs/1601.01233). [doi](https://en.wikipedia.org/wiki/Doi_(identifier) "Doi (identifier)"):[10.1145/2603088.2603105](https://doi.org/10.1145%2F2603088.2603105). [ISBN](https://en.wikipedia.org/wiki/ISBN_(identifier) "ISBN (identifier)") [9781450328869](https://en.wikipedia.org/wiki/Special:BookSources/9781450328869 "Special:BookSources/9781450328869"). [S2CID](https://en.wikipedia.org/wiki/S2CID_(identifier) "S2CID (identifier)") [11485010](https://api.semanticscholar.org/CorpusID:11485010).
32.  ^ [Jump up to: _**a**_](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-Reasonable_33-0) [_**b**_](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-Reasonable_33-1) Accattoli, Beniamino (October 2018). ["(In)Efficiency and Reasonable Cost Models"](https://doi.org/10.1016%2Fj.entcs.2018.10.003). _Electronic Notes in Theoretical Computer Science_. **338**: 23–43. [doi](https://en.wikipedia.org/wiki/Doi_(identifier) "Doi (identifier)"):[10.1016/j.entcs.2018.10.003](https://doi.org/10.1016%2Fj.entcs.2018.10.003).
33.  ^ [Jump up to: _**a**_](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-Asperti_34-0) [_**b**_](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-Asperti_34-1) Asperti, Andrea (16 Jan 2017). ["About the efficient reduction of lambda terms"](https://arxiv.org/pdf/1701.04240v1.pdf) (PDF). [arXiv](https://en.wikipedia.org/wiki/ArXiv_(identifier) "ArXiv (identifier)"):[1701.04240v1](https://arxiv.org/abs/1701.04240v1). Retrieved 19 August 2021.
34.  **[^](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-35 "Jump up")** [Landin, P. J.](https://en.wikipedia.org/wiki/Peter_Landin "Peter Landin") (1965). "A Correspondence between ALGOL 60 and Church's Lambda-notation". _Communications of the ACM_. **8** (2): 89–101. [doi](https://en.wikipedia.org/wiki/Doi_(identifier) "Doi (identifier)"):[10.1145/363744.363749](https://doi.org/10.1145%2F363744.363749). [S2CID](https://en.wikipedia.org/wiki/S2CID_(identifier) "S2CID (identifier)") [6505810](https://api.semanticscholar.org/CorpusID:6505810).

## Further reading\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=44 "Edit section: Further reading")\]

-   Abelson, Harold & Gerald Jay Sussman. [Structure and Interpretation of Computer Programs](https://en.wikipedia.org/wiki/Structure_and_Interpretation_of_Computer_Programs "Structure and Interpretation of Computer Programs"). [The MIT Press](https://en.wikipedia.org/wiki/The_MIT_Press "The MIT Press"). [ISBN](https://en.wikipedia.org/wiki/ISBN_(identifier) "ISBN (identifier)") [0-262-51087-1](https://en.wikipedia.org/wiki/Special:BookSources/0-262-51087-1 "Special:BookSources/0-262-51087-1").
-   [Hendrik Pieter Barendregt](https://en.wikipedia.org/wiki/Henk_Barendregt "Henk Barendregt") [_Introduction to Lambda Calculus_](http://www.cse.chalmers.se/research/group/logic/TypesSS05/Extra/geuvers.pdf).
-   [Henk Barendregt](https://en.wikipedia.org/wiki/Henk_Barendregt "Henk Barendregt"), [The Impact of the Lambda Calculus in Logic and Computer Science](https://www.jstor.org/stable/421013). The Bulletin of Symbolic Logic, Volume 3, Number 2, June 1997.
-   [Barendregt, Hendrik Pieter](https://en.wikipedia.org/wiki/Henk_Barendregt "Henk Barendregt"), _The Type Free Lambda Calculus_ pp1091–1132 of _Handbook of Mathematical Logic_, [North-Holland](https://en.wikipedia.org/wiki/North-Holland_Publishing_Company "North-Holland Publishing Company") (1977) [ISBN](https://en.wikipedia.org/wiki/ISBN_(identifier) "ISBN (identifier)") [0-7204-2285-X](https://en.wikipedia.org/wiki/Special:BookSources/0-7204-2285-X "Special:BookSources/0-7204-2285-X")
-   Cardone and Hindley, 2006. [History of Lambda-calculus and Combinatory Logic](http://www.users.waitrose.com/~hindley/SomePapers_PDFs/2006CarHin,HistlamRp.pdf). In Gabbay and Woods (eds.), _Handbook of the History of Logic_, vol. 5. Elsevier.
-   Church, Alonzo, _An unsolvable problem of elementary number theory_, [American Journal of Mathematics](https://en.wikipedia.org/wiki/American_Journal_of_Mathematics "American Journal of Mathematics"), 58 (1936), pp. 345–363. This paper contains the proof that the equivalence of lambda expressions is in general not decidable.
-   Alonzo Church, _The Calculi of Lambda-Conversion_ ([ISBN](https://en.wikipedia.org/wiki/ISBN_(identifier) "ISBN (identifier)") [978-0-691-08394-0](https://en.wikipedia.org/wiki/Special:BookSources/978-0-691-08394-0 "Special:BookSources/978-0-691-08394-0")) [\[1\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-36)
-   Frink Jr., Orrin, _Review: The Calculi of Lambda-Conversion_ [\[2\]](https://en.wikipedia.org/wiki/Lambda_calculus#cite_note-37)
-   Kleene, Stephen, _A theory of positive integers in formal logic_, [American Journal of Mathematics](https://en.wikipedia.org/wiki/American_Journal_of_Mathematics "American Journal of Mathematics"), 57 (1935), pp. 153–173 and 219–244. Contains the lambda calculus definitions of several familiar functions.
-   [Landin, Peter](https://en.wikipedia.org/wiki/Peter_Landin "Peter Landin"), _A Correspondence Between ALGOL 60 and Church's Lambda-Notation_, [Communications of the ACM](https://en.wikipedia.org/wiki/Communications_of_the_ACM "Communications of the ACM"), vol. 8, no. 2 (1965), pages 89–101. Available from the [ACM site](http://portal.acm.org/citation.cfm?id=363749&coll=portal&dl=ACM). A classic paper highlighting the importance of lambda calculus as a basis for programming languages.
-   Larson, Jim, [_An Introduction to Lambda Calculus and Scheme_](https://web.archive.org/web/20011206080336/http://www.jetcafe.org/~jim/lambda.html). A gentle introduction for programmers.
-   Schalk, A. and Simmons, H. (2005) _[An introduction to λ-calculi and arithmetic with a decent selection of exercises](https://web.archive.org/web/20080307014129/http://www.cs.man.ac.uk/~hsimmons/BOOKS/lcalculus.pdf). Notes for a course in the Mathematical Logic MSc at Manchester University._
-   [de Queiroz, Ruy J.G.B.](https://en.wikipedia.org/wiki/Ruy_de_Queiroz "Ruy de Queiroz") (2008). "On Reduction Rules, Meaning-as-Use and Proof-Theoretic Semantics". _[Studia Logica](https://en.wikipedia.org/wiki/Studia_Logica "Studia Logica")_. **90** (2): 211–247. [doi](https://en.wikipedia.org/wiki/Doi_(identifier) "Doi (identifier)"):[10.1007/s11225-008-9150-5](https://doi.org/10.1007%2Fs11225-008-9150-5). [S2CID](https://en.wikipedia.org/wiki/S2CID_(identifier) "S2CID (identifier)") [11321602](https://api.semanticscholar.org/CorpusID:11321602). A paper giving a formal underpinning to the idea of 'meaning-is-use' which, even if based on proofs, it is different from proof-theoretic semantics as in the Dummett–Prawitz tradition since it takes reduction as the rules giving meaning.
-   Hankin, Chris, _An Introduction to Lambda Calculi for Computer Scientists,_ [ISBN](https://en.wikipedia.org/wiki/ISBN_(identifier) "ISBN (identifier)") [0954300653](https://en.wikipedia.org/wiki/Special:BookSources/0954300653 "Special:BookSources/0954300653")

Monographs/textbooks for graduate students:

-   Morten Heine Sørensen, Paweł Urzyczyn, _Lectures on the Curry–Howard isomorphism_, Elsevier, 2006, [ISBN](https://en.wikipedia.org/wiki/ISBN_(identifier) "ISBN (identifier)") [0-444-52077-5](https://en.wikipedia.org/wiki/Special:BookSources/0-444-52077-5 "Special:BookSources/0-444-52077-5") is a recent monograph that covers the main topics of lambda calculus from the type-free variety, to most [typed lambda calculi](https://en.wikipedia.org/wiki/Typed_lambda_calculi "Typed lambda calculi"), including more recent developments like [pure type systems](https://en.wikipedia.org/wiki/Pure_type_system "Pure type system") and the [lambda cube](https://en.wikipedia.org/wiki/Lambda_cube "Lambda cube"). It does not cover [subtyping](https://en.wikipedia.org/wiki/Subtyping "Subtyping") extensions.
-   Pierce, Benjamin (2002), _Types and Programming Languages_, MIT Press, [ISBN](https://en.wikipedia.org/wiki/ISBN_(identifier) "ISBN (identifier)") [0-262-16209-1](https://en.wikipedia.org/wiki/Special:BookSources/0-262-16209-1 "Special:BookSources/0-262-16209-1") covers lambda calculi from a practical type system perspective; some topics like dependent types are only mentioned, but subtyping is an important topic.

_Some parts of this article are based on material from [FOLDOC](https://en.wikipedia.org/wiki/Free_On-line_Dictionary_of_Computing "Free On-line Dictionary of Computing"), used with [permission](https://en.wikipedia.org/wiki/Wikipedia:Foldoc_license "Wikipedia:Foldoc license")._

## External links\[[edit](https://en.wikipedia.org/w/index.php?title=Lambda_calculus&action=edit&section=45 "Edit section: External links")\]

-   Graham Hutton, [Lambda Calculus](https://www.youtube.com/watch?v=eis11j_iGMs), a short (12 minutes) Computerphile video on the Lambda Calculus
-   Helmut Brandl, _[Step by Step Introduction to Lambda Calculus](https://hbr.github.io/Lambda-Calculus/)_
-   ["Lambda-calculus"](https://www.encyclopediaofmath.org/index.php?title=Lambda-calculus), _[Encyclopedia of Mathematics](https://en.wikipedia.org/wiki/Encyclopedia_of_Mathematics "Encyclopedia of Mathematics")_, [EMS Press](https://en.wikipedia.org/wiki/European_Mathematical_Society "European Mathematical Society"), 2001 \[1994\]
-   Achim Jung, _[A Short Introduction to the Lambda Calculus](http://www.cs.bham.ac.uk/~axj/pub/papers/lambda-calculus.pdf)_\-([PDF](https://en.wikipedia.org/wiki/Portable_Document_Format "Portable Document Format"))
-   Dana Scott, _[A timeline of lambda calculus](http://turing100.acm.org/lambda_calculus_timeline.pdf)_\-([PDF](https://en.wikipedia.org/wiki/Portable_Document_Format "Portable Document Format"))
-   David C. Keenan, _[To Dissect a Mockingbird: A Graphical Notation for the Lambda Calculus with Animated Reduction](http://dkeenan.com/Lambda/)_
-   Raúl Rojas, _[A Tutorial Introduction to the Lambda Calculus](http://www.inf.fu-berlin.de/inst/ag-ki/rojas_home/documents/tutorials/lambda.pdf)_\-([PDF](https://en.wikipedia.org/wiki/Portable_Document_Format "Portable Document Format"))
-   Peter Selinger, _[Lecture Notes on the Lambda Calculus](http://www.mscs.dal.ca/~selinger/papers/#lambdanotes)_\-([PDF](https://en.wikipedia.org/wiki/Portable_Document_Format "Portable Document Format"))
-   L. Allison, _[Some executable λ-calculus examples](http://www.allisons.org/ll/FP/Lambda/Examples/)_
-   Georg P. Loczewski, [_The Lambda Calculus and A++_](http://www.lambda-bound.com/book/lambdacalc/lcalconl.html)
-   Bret Victor, _[Alligator Eggs: A Puzzle Game Based on Lambda Calculus](http://worrydream.com/AlligatorEggs/)_
-   _[Lambda Calculus](http://www.safalra.com/science/lambda-calculus/) [Archived](https://web.archive.org/web/20121014180848/http://safalra.com/science/lambda-calculus/) 2012-10-14 at the [Wayback Machine](https://en.wikipedia.org/wiki/Wayback_Machine "Wayback Machine")_ on [Safalra's Website](http://www.safalra.com/) [Archived](https://web.archive.org/web/20210502051230/https://safalra.com/) 2021-05-02 at the [Wayback Machine](https://en.wikipedia.org/wiki/Wayback_Machine "Wayback Machine")
-   [LCI Lambda Interpreter](https://chatziko.github.io/lci/) a simple yet powerful pure calculus interpreter
-   [Lambda Calculus links on Lambda-the-Ultimate](http://lambda-the-ultimate.org/classic/lc.html)
-   Mike Thyer, [Lambda Animator](https://web.archive.org/web/20070713173324/http://thyer.name/lambda-animator/), a graphical Java applet demonstrating alternative reduction strategies.
-   [Implementing the Lambda calculus](http://matt.might.net/articles/c++-template-meta-programming-with-lambda-calculus/) using [C++ Templates](https://en.wikipedia.org/wiki/C%2B%2B_Templates "C++ Templates")
-   Marius Buliga, [_Graphic lambda calculus_](https://web.archive.org/web/20140202195546/http://imar.ro/~mbuliga/graphic_revised.pdf)
-   [_Lambda Calculus as a Workflow Model_](https://web.archive.org/web/20160729210437/http://cs.adelaide.edu.au/~pmk/publications/wage2008.pdf) by Peter Kelly, Paul Coddington, and Andrew Wendelborn; mentions [graph reduction](https://en.wikipedia.org/wiki/Graph_reduction "Graph reduction") as a common means of evaluating lambda expressions and discusses the applicability of lambda calculus for [distributed computing](https://en.wikipedia.org/wiki/Distributed_computing "Distributed computing") (due to the [Church–Rosser](https://en.wikipedia.org/wiki/Church%E2%80%93Rosser_theorem "Church–Rosser theorem") property, which enables [parallel](https://en.wikipedia.org/wiki/Parallel_computing "Parallel computing") graph reduction for lambda expressions).
-   Shane Steinert-Threlkeld, ["Lambda Calculi"](https://web.archive.org/web/20141216225504/http://www.iep.utm.edu/lambda-calculi/), _[Internet Encyclopedia of Philosophy](https://en.wikipedia.org/wiki/Internet_Encyclopedia_of_Philosophy "Internet Encyclopedia of Philosophy")_
-   Anton Salikhmetov, [_Macro Lambda Calculus_](https://codedot.github.io/lambda/)

1.  **[^](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-36 "Jump up")** Church, Alonzo (1941). [_The Calculi of Lambda-Conversion_](https://archive.org/details/AnnalsOfMathematicalStudies6ChurchAlonzoTheCalculiOfLambdaConversionPrincetonUniversityPress1941). Princeton: Princeton University Press. Retrieved 2020-04-14.
2.  **[^](https://en.wikipedia.org/wiki/Lambda_calculus#cite_ref-37 "Jump up")** [Frink Jr., Orrin](https://en.wikipedia.org/wiki/Orrin_Frink "Orrin Frink") (1944). ["Review: _The Calculi of Lambda-Conversion_ by Alonzo Church"](https://www.ams.org/bull/1944-50-03/S0002-9904-1944-08090-7/S0002-9904-1944-08090-7.pdf) (PDF). _Bull. Amer. Math. Soc_. **50** (3): 169–172. [doi](https://en.wikipedia.org/wiki/Doi_(identifier) "Doi (identifier)"):[10.1090/s0002-9904-1944-08090-7](https://doi.org/10.1090%2Fs0002-9904-1944-08090-7).