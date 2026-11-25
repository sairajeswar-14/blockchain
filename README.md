# VoteSphere India

Blockchain-enabled election transparency, EPIC voter-identity verification and privacy-preserving digital ballot simulation prototype.

Independent educational prototype. Not operated, approved by or connected to the Election Commission of India. All voters, candidates and results are fictional.

## Files

- `index.html` – the working election simulation (no build step)
- `poster.html` – the project poster, served at `/poster`
- `vercel.json` – clean URLs and security headers

## Run locally

    npx serve .

Then open the printed address.

## Deploy with GitHub and Vercel

1. Create a new empty repository on GitHub.
2. In this folder run:

        git init
        git add .
        git commit -m "VoteSphere India"
        git branch -M main
        git remote add origin https://github.com/<your-username>/votesphere-india.git
        git push -u origin main

3. Open vercel.com, choose Add New, then Project, and import the repository.
4. Leave Framework Preset as Other. Leave Build Command and Output Directory empty. Click Deploy.

Every push to `main` redeploys automatically.

## Demo credentials

Administrator passwords: `super-demo`, `elect-demo`, `audit-demo`.
Fictional EPIC records are listed on the EPIC Verification page.

## Limitations

Verification uses a mock service with synthetic records. State is held in browser memory and resets on reload. Role checks run in the browser. Passwords use PBKDF2 through Web Crypto. The ledger is a local hash chain, not a deployed Solidity contract.
