# Rust Raw Pointer Bug
This repository demonstrates a common error in Rust involving unsafe code and raw pointers. The code attempts to modify a vector using a raw pointer after changing the vector's length, leading to undefined behavior. The solution demonstrates a safer approach using vector indexing or other safe Rust methods.  This is a simple but important example to illustrate the risks associated with unsafe operations in Rust.

## Bug
The `bug.rs` file contains code that exhibits the undefined behavior. Running this code may lead to a program crash or unexpected results depending on the compiler and system.

## Solution
The `bugSolution.rs` file presents corrected code. It avoids the use of raw pointers directly, instead using the standard vector indexing. This approach eliminates the risks associated with the previous unsafe code, resulting in more predictable behavior and safer memory management.