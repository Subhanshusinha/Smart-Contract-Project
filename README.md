# Project- Smart Contract

# Safe Operations Contract

This project is a Solidity smart contract that demonstrates the use of `require()`, `assert()`, and `revert()` statements for performing safe arithmetic operations and handling errors.

## Description

The Safe Operations Contract provides a set of functions that perform basic arithmetic operations (addition, subtraction, and multiplication) on unsigned integers while ensuring the safety of these operations. It utilizes the `require()` statement to check for overflow and underflow conditions, and the `assert()` statement to validate internal invariants. Additionally, it includes a function that deliberately reverts with a custom error message to showcase the usage of the `revert()` statement.

## Getting Started

### Installing

1. Make sure you have a compatible Solidity compiler installed (version 0.8.0 or higher).
2. Copy the provided Solidity code into a new file (e.g., `SafeOperations.sol`).

### Executing program

To interact with the Safe Operations Contract, you will need to use a compatible Ethereum client or development environment, such as Remix IDE

1. Compile the `SafeOperations.sol` file.
2. Deploy the contract to the desired Ethereum network (e.g., local development network, testnet, or mainnet).
3. Once deployed, you can interact with the contract using its public functions:
    - `safeAdd(uint a, uint b)`: Adds two unsigned integers, reverts on overflow.
    - `safeSubtract(uint a, uint b)`: Subtracts two unsigned integers, reverts on underflow.
    - `safeMultiply(uint a, uint b)`: Multiplies two unsigned integers, reverts on overflow.
    - `deposit(uint amount)`: Adds an amount to the contract's balance, reverts on overflow.
    - `withdraw(uint amount)`: Subtracts an amount from the contract's balance, reverts if the balance is insufficient.
    - `revertWithMessage()`: A function that purposefully reverts with a custom error message.


Example deployment in Solidity:

    uint sum = safeOperations.safeAdd(10, 20);
  
    uint diff = safeOperations.safeSubtract(30, 10);
  
    uint product = safeOperations.safeMultiply(5, 6);
  
    safeOperations.deposit(100);
  
    safeOperations.withdraw(50);

## Help

If you encounter any issues or have questions, feel free to reach out to the contributors.

## Authors

  - Subhanshu sinha and - subhanshu.sinha667@gmail.com 

## License

This project is licensed under the MIT License - see the LICENSE file for details.
