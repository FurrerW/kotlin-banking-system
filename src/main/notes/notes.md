Initial Implementation Steps
When starting your project, I'd recommend this approach:

Create the project: Use IntelliJ IDEA or another IDE to create a new Kotlin project with Gradle or Maven
Set up the package structure: Create packages for different components (model, service, etc.)
Start with domain models: Define your core entity classes first (Account, Customer, Transaction)
Implement basic functionality: Add methods for core operations
Create a simple main function: To test your implementation as you go

Key Implementation Decisions
For the banking application, consider these initial implementation details:

Account.kt:

Start with a simple class definition with properties for account number, balance, and owner
Implement basic methods for deposit and withdrawal with validation


Customer.kt:

Create a class with properties for customer information
Add a collection to hold multiple accounts
Implement methods for account management


Bank.kt or BankService.kt:

Create the central coordinating class
Add collections to store customers and accounts
Implement methods to perform operations across accounts


Transaction.kt:

Define a class to record and represent transactions
Consider using a sealed class to represent different transaction types



Using Kotlin Features
Take advantage of Kotlin's language features to make your code more concise and robust:

Data classes: For entities like Transaction that primarily hold data
Nullable types: For fields that might not always have a value
Extension functions: To add functionality to existing classes
Collections API: For managing lists of accounts and transactions
Default parameters: For providing sensible defaults in constructors

Starting Small and Incremental Development
Begin with a minimal viable implementation that demonstrates core concepts:

Create basic Account and Customer classes
Implement a main function that creates a few accounts and performs simple operations
Verify that your basic operations work correctly
Incrementally add more features, testing as you go

Remember that the goal is to learn about classes and objects in Kotlin. Don't worry about building a complete banking system right away. Focus on getting comfortable with defining classes, creating relationships between objects, and implementing business logic.