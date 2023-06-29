# ADYBurnWallet 
Creates an AlwaysFails address for the ADY project.

# Requirements
- Plutus Environemnt
  - Easiest Method is to set up using the PPP instructions at https://iog-academy.gitbook.io/plutus-pioneers-program-fourth-cohort/preliminary-work/setup
- cardano-cli
  - this is used to build the payment adddress

# workflow
1. load the Burn.hs file in your Plutus Environment.
   ```
   import Burn
   ```
2. Write the validator to a plutus file.
   ```
   Burn.saveVal
   ```
   This creates a file named burn.plutus in the plutus directory
3. Execute the buildAddress.sh
   ```
   cd scripts
   ./buildAddress.sh
   ```
   This executable looks for the burn.plutus in the plutus directory and outputs the ADYBurnWallet.addr
