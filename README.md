Paytm Wallet App that enables users to perform a variety of financial transactions. Users can easily sign up and sign in to
their accounts. The app allows users to add funds to their wallet by linking their HDFC or Axis Bank accounts (on-ramp functionality) and
transferring money from these bank accounts to their wallet.
In addition to receiving funds, users can also transfer money to other users, using either their phone number or name as the recipient
identifier. The app also provides a transaction history feature, where users can view their on-ramp transactions from the linked bank
accounts to the wallet, offering a seamless tracking experience.

- Clone the repo

```jsx
git clone https://github.com/04piyush/Paytm-Wallet-App.git
```

- npm install
- Run postgres either locally or on the cloud (neon.tech)

```jsx
docker run  -e POSTGRES_PASSWORD=mysecretpassword -d -p 5432:5432 postgres
```

- Copy over all .env.example files to .env
- Update .env files everywhere with the right db url
- Go to `packages/db`
  - npx prisma migrate dev
  - npx prisma db seed
- Go to `apps/user-app` , run `npm run dev`
- Try logging in using phone - 1111111111 , password - alice (See `seed.ts`)
