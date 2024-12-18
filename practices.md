# Avoid var Keyword: A Relic of the Past
Before ES6, the var keyword was the primary way to declare variables. However, it had some quirks and limitations that often led to unexpected results and made debugging more challenging.

In modern JavaScript, we generally avoid using var and instead opt for let and const, which offer more predictable and block-scoped behavior, making your code easier to understand and maintain.

# let: Variables that can change
Use the `let` keyword to declare variables whose values you might need to change later in your code.

# const: Constants for unchanging values
If you have a value that shouldn’t change throughout your program, use the `const` keyword.

A good rule of thumb is to use `const` by default and only switch to `let` if you know you'll need to reassign the variable's value later.

# Clarity and descriptiveness
The primary goal of variable naming is to convey the purpose and content of the variable clearly. Choose names that are self-explanatory and accurately reflect the data they store.

GOOD: `firstName`, `totalPrice`, `productDescription1`
BAD: `x`, `a`, `temp`

# Use meaningful words
Avoid abbreviations or overly technical jargon that might confuse other developers.

GOOD: `customerName`, `orderStatus`, `employeeRecord`
BAD: `custNm`, `ordSt`, `empRec`

# Camel case convention
The most widely adopted naming convention for variables in JavaScript is the camel case.

GOOD: `fullName`, `dateOfBirth`, `shippingAddress`
BAD: `full_name`, `dateofbirth`, `shipping_address`

# Constants in uppercase
If you have variables that hold constant values and shouldn't be modified, declare them in uppercase with underscores separating words.

GOOD: `TAX_RATE`, `API_KEY`, `MAX_ATTEMPTS`
BAD: `taxRate`, `apiKey`, `maxAttempts`

# Avoid Single-Letter Variables
While single-letter variables might be tempting for quick iterations, they generally make code less readable.

GOOD: `counter`, `index`, `sum`
BAD (except for specific cases): `i`, `j`, `k`

# Use plurals for arrays
If your variable represents an array, use a plural name to signify that it contains multiple elements.

GOOD: `productNames`, `orderItems`, `employeeList`
BAD: `productName`, `orderItem`, `employee`

# Prefix Boolean Variables
For boolean variables, consider using prefixes like `is`, `has`, or `can` to make their purpose clear.

GOOD: `isActive`, `hasDiscount`, `canEdit`, `isLoggedIn`
BAD: `active`, `discountApplied`, `editEnabled`, `loggedIn`

# Scope-Aware Naming
If you're working with variables within specific scopes, consider incorporating prefixes or suffixes that indicate their scope.

GOOD: `globalCounter`, `localIndex`, `moduleSpecificConfig`
BAD: `counter`, `index`, `config`

# Declare Separately
It's good practice to declare each variable on its own line for better readability.

GOOD: `let isActive = false; let canEdit = true`
BAD: `let isActive = false, canEdit = true`
