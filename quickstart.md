# Quickstart Guide

This guide helps you make your first payment using the Stripe API.

## Step 1: Get API Key
Sign in to your Stripe Dashboard → Developers → API Keys.

## Step 2: Make a Payment
Example using `curl`:

```bash
curl https://api.stripe.com/v1/charges \
  -u sk_test_yourApiKey: \
  -d amount=2000 \
  -d currency=usd \
  -d "source=tok_visa" \
  -d "description=Charge for demo@example.com"
