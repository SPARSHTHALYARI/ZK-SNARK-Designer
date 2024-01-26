# ZK-SNARK-Designer
To successfully complete the Final Challenge, you'll need to follow a series of steps involving circuit implementation, compilation, proof generation, deployment of a Solidity verifier contract, and testing. Here's a breakdown of each step along with instructions:

### 1. Write a correct circuit.circom implementation:
You need to design a circuit using the Circom language. Ensure that your circuit accurately represents the logic you want to verify. Make sure to define inputs, outputs, and any intermediate signals appropriately.

### 2. Compile the circuit to generate circuit intermediaries:
Use the Circom compiler to compile your circuit. This process generates intermediary files necessary for generating proofs. Make sure the compilation process completes without errors.

### 3. Generate a proof using inputs A=0 B=1:
With your compiled circuit and the correct inputs (A=0, B=1), generate a proof using a tool like SnarkJS or another suitable library for generating SNARK proofs. This proof demonstrates that your circuit functions correctly according to the specified inputs.

### 4. Deploy a Solidity verifier to Sepolia or Mumbai Testnet:
Write a Solidity contract that serves as a verifier for your generated proof. Deploy this verifier contract to either the Sepolia or Mumbai Testnet, depending on your preference and availability.

### 5. Call the verifyProof() method on the verifier contract and assert output is true:
Write a script or interact directly with your deployed verifier contract to call the `verifyProof()` method. Pass in the generated proof along with the inputs (A=0, B=1) to the method. Ensure that the output returned by the method is true, indicating that the proof is valid and the circuit logic holds true for the given inputs.

By completing these steps and documenting your process in the README file, you'll successfully fulfill the requirements of the Final Challenge. Make sure to test thoroughly and verify each component's functionality before finalizing your project.
