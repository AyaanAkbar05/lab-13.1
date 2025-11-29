Q1: Why whitelist IPs in production?

To limit access to trusted sources only. Allowing 0.0.0.0/0 exposes the database to anyone on the internet → high risk of hacking or data theft.

Q2: Purpose of dotenv?

Loads environment variables from .env into process.env. In production, variables could be managed via hosting platforms (Heroku, Vercel, AWS Secrets Manager, etc.) instead.

Q3: Debugging connection failures:

Check connection string (username, password, database name).

Verify network access (IP whitelist).

Confirm MongoDB cluster is running.

Look at console errors for detailed messages.
