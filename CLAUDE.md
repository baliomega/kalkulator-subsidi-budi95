# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a single-page web application for calculating fuel subsidy savings in Malaysia. The calculator helps users understand how much they save with the BUDI95 subsidy program by comparing subsidized vs non-subsidized petrol prices.

## Architecture

**Single HTML File Structure**: The entire application is contained in `budi95-calculator.html` with inline CSS and JavaScript. There is no build process or external dependencies.

**Key Components**:
- **Pricing Constants** (lines 254-256): Three price points that drive all calculations
  - `PRICE_SUBSIDIZED`: RM 1.99/L (current subsidized rate)
  - `PRICE_NON_SUBSIDIZED`: RM 2.60/L (market rate without subsidy)
  - `PRICE_OLD_RATE`: RM 2.05/L (previous rate for comparison)

- **Core Calculation Logic** (`calculateSubsidy()`, lines 268-288): Given a payment amount in RM, calculates:
  1. Liters obtainable at subsidized price
  2. What those liters would cost without subsidy
  3. Actual savings amount
  4. Comparison with old rate

## Development

**Running the Application**: Open `budi95-calculator.html` directly in any modern web browser. No server or build step required.

**Testing Changes**: Refresh the browser after editing. Use browser DevTools console to debug JavaScript.

**Language**: All UI text is in Malay (Bahasa Malaysia).

## Modifying Price Points

When subsidy rates change, update the constants at lines 254-256. The UI comparison section (lines 236-249) displays all three rates to users.

## Key Behaviors

- Results appear only when a positive amount is entered
- Quick amount buttons (RM 10-60) populate the input field
- Input accepts decimal values (e.g., RM 25.50)
- All monetary outputs formatted to 2 decimal places
- Liter calculations shown to 3 decimal places
