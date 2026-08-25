# Project Spec
# Agentic Commerce AI — Project Specification

## 1. Project

Agentic Commerce AI

## 2. Buildathon

Razorpay AI Buildathon 2026

## 3. Track

AI Growth & Agentic Commerce

## 4. Problem

Small and medium-sized merchants often have product catalogs and
customer data but lack an intelligent system that can continuously
identify opportunities to increase conversions, upsells, cross-sells,
and revenue.

At the same time, customers increasingly want to shop using natural
language instead of manually browsing large product catalogs.

## 5. Proposed Solution

We are building a two-sided agentic commerce platform consisting of:

1. AI Growth Agent
2. AI Buyer

The AI Growth Agent helps merchants identify and act on opportunities
to increase sales.

The AI Buyer helps customers discover, compare, and purchase products
using natural-language requests.

The two sides are connected to demonstrate an end-to-end agentic
commerce flow.

## 6. Initial Merchant

Sports / running store.

The initial demo will use a fictional sports merchant and a synthetic
product/customer dataset.

## 7. Core User Journey

A customer says:

"I need running shoes under ₹5,000 for daily running and some socks."

The AI Buyer should:

1. Understand the customer's requirements.
2. Search the merchant's product catalog.
3. Filter products according to the requirements.
4. Compare suitable products.
5. Recommend the best option.
6. Identify relevant offers.
7. Suggest useful upsells or cross-sells.
8. Build a cart.
9. Show the final price clearly.
10. Ask for customer confirmation before payment.
11. Initiate a Razorpay test payment.
12. Create an order after successful payment.

## 8. AI Growth Agent

The AI Growth Agent helps the merchant by:

- Understanding the product catalog.
- Analyzing synthetic customer behavior data.
- Identifying upsell opportunities.
- Identifying cross-sell opportunities.
- Identifying products frequently purchased together.
- Suggesting personalized offers.
- Explaining why an offer is recommended.
- Tracking basic growth metrics.

## 9. AI Buyer

The AI Buyer is responsible for:

- Natural-language shopping requests.
- Intent extraction.
- Product discovery.
- Product filtering.
- Product comparison.
- Product recommendation.
- Offer discovery.
- Upsell/cross-sell suggestions.
- Cart creation.
- Checkout assistance.

## 10. Orchestrator

An orchestration layer will coordinate the agents and tools.

Responsibilities:

- Decide which agent/tool should act.
- Maintain conversation and transaction state.
- Validate tool inputs.
- Enforce business rules.
- Prevent unsafe payment actions.
- Record important actions.

## 11. Payment Safety

The AI must not autonomously spend money without appropriate
authorization.

Payment actions must be:

- Explainable.
- Bounded.
- Explicitly confirmed by the customer where required.
- Logged in an audit trail.
- Recoverable when failures occur.

The project will use Razorpay Test Mode.

## 12. Initial MVP

The first working MVP will contain:

- Merchant product catalog.
- Synthetic customer behavior data.
- AI Growth Agent.
- Customer AI Buyer.
- Natural-language product search.
- Product recommendation.
- Offer recommendation.
- Cart.
- Razorpay test payment.
- Order creation.
- Basic merchant analytics.
- Basic audit trail.
- Payment failure handling.

## 13. Technology

### Frontend

Next.js  
TypeScript

### Backend

Python  
FastAPI

### Database

PostgreSQL

### AI

LLM with tool/function calling.

### Payments

Razorpay Test Mode.

## 14. Initial Architecture

The detailed architecture will be designed separately in:

docs/ARCHITECTURE.md

## 15. Evaluation Goals

The project should demonstrate:

- Genuine agentic behavior.
- Useful merchant value.
- Useful customer experience.
- Explainable AI decisions.
- Safe payment handling.
- Graceful failure handling.
- Measurable business impact.
- Clean engineering.
- Reproducible setup.

## 16. Possible Future Features

These are NOT part of the initial MVP unless time allows:

- Voice shopping.
- Multi-agent negotiation.
- Advanced customer segmentation.
- AI-readable merchant catalogs.
- Automated campaign orchestration.
- Advanced personalization.
- Multiple merchant support.
