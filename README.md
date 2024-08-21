**Candy Machine UI Setup Guide**

This guide provides a detailed, step-by-step process for creating the user interface (UI) for your Candy Machine, enabling users to mint NFTs using a configured SPL token. The UI integrates the SPL token as the payment method and allows users to easily connect their Phantom wallets.

**Prerequisites**
Before you begin, make sure you have the following:

1. A properly configured Candy Machine with a `config.json` file that includes details such as price, quantity, symbol, seller fee, SPL token account, SPL token, go-live date, and creator details.
2. A Phantom wallet designated for minting.

**Steps**

1. **SPL Token Setup:**
   If you haven't already done so, follow the guidelines from Lesson Three to create your SPL token. Make sure to record the SPL token's address.

2. **Update Candy Machine Config:**
   Open the `config.json` file of your Candy Machine and update the following:
   - `splTokenAccount`: Enter the address of the SPL token account you created.
   - `splToken`: Enter the address of the SPL token.

3. **UI Setup:**
   Use the "Quick Node: Set Up a Minting Site" tutorial as a reference to create a user-friendly interface for your Candy Machine. This UI will allow users to connect their Phantom wallets and mint NFTs using the SPL token.

4. **Modify Minting Logic:**
   Adjust the minting logic of your project (as detailed in Lesson Three) to either mint NFTs directly to the connected Phantom wallet address or modify the transfer function to send minted NFTs to your designated Phantom wallet.

5. **Testing:**
   Test the entire setup by transferring or minting your SPL token to one of your Phantom accounts. Use the UI you created to mint NFTs, ensuring that users can successfully mint NFTs using the SPL token as the payment method.

**Additional Tips**

- For a more detailed implementation of Candy Machine logic, including minting functionality and token configuration, check out my Candy Machine Repository.
- The SPL token creation process follows the SPL token Program by MetaCrafters.
- Double-check that the addresses and token details in the `config.json` file match the tokens and accounts you've set up.
- Provide clear and concise instructions in your UI to guide users through connecting their Phantom wallets and minting NFTs.
- Customize your UI to fit your design preferences.

**Conclusion**

By following these steps, you'll successfully set up a Candy Machine UI that allows users to mint NFTs using the configured SPL token. Users can connect their Phantom wallets and easily use the SPL token for payment to mint NFTs through your Candy Machine. Be sure to thoroughly test everything before making it available to the public.
