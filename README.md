# Restaurant Reviews Sample Application - Onchain Program + Frontend

Contains Onchain program on Solana written in Vanilla Rust inside "program" directory and the frontend written in Typescript and Next.js program in the root directory.

## Prerequisites
Solana CLI, Rust, Cargo installed on the system. 

## Instructions - How to start

1. `cd program`
2. `solana config set --url devnet`
3. `cargo build-bpf `
4. `solana program deploy ./target/deploy/restaurant_reviews.so --program-id ./target/deploy/restaurant_reviews-keypair.json`
5. Copy the program id as it appears and paste into "src/pages/index.tsx" inside REVIEW_PROGRAM_ID constant
6. `cd ..` (back to root dir)
7. `npm install`
8. `npm run dev`

Have a solana wallet installed in your browser, go to "localhost:3000" and connect wallet to the application. Make sure the connected wallet has
enough SOL balance on devnet. Fill in all the fields, submit and confirm the transaction.

Reload the page to see the newly added review card on the frontend!
