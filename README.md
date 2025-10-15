contract PrivateState {
    // 'public' state variables are transparent, visible on-chain.
    public var public_balance: U256;

    // 'private' state variables are encrypted on-chain.
    // Operations on them are verified using zero-knowledge proofs (ZKPs),
    // allowing computation without revealing the underlying values.
    private var private_balance: U256;
    private var secret_message: String;

    // Example: Transfer from a private balance, proving sufficient funds without revealing amount
    public fn transfer_private(ctx: ContractContext, recipient: Address, amount: U256) {
        // In Compact, operations on `private` state variables are automatically
        // compiled into a zero-knowledge circuit by the Compact compiler.
        // The runtime then handles the generation and verification of ZKPs
        // during transaction execution.

        // Developer writes logical operations as usual:
        let current_balance = self.private_balance.get();
        require(current_balance >= amount, "Insufficient private funds");
        self.private_balance.set(ctx, current_balance - amount);

        // For cross-contract private calls, the Compact runtime facilitates
        // the secure and private transfer of value, ensuring the recipient's
        // private state is updated correctly without revealing the amount.
        // E.g., a call to recipient_contract.deposit_private(ctx, amount);
        // This is a high-level conceptual example, the underlying ZKP mechanism
        // is abstracted by the language and runtime.

        // The key takeaway is: `private` in Compact means genuinely private,
        // backed by ZKP-guaranteed confidentiality.
        // Neither the `current_balance`, `amount`, nor `secret_message` are
        // revealed on the public ledger. Only the proof of a valid state transition is.
    }
}