# MCDA Integration Guide

Use the [Multi-Criteria Decision Analysis (MCDA) Framework](https://svenwillrich.de/mcda/) by Dr. Sven-Erik Willrich to perform quantitative analysis on your cloud deployment decision.

## About the MCDA Tool

> This Multi-Criteria Decision Analysis (MCDA) tool was designed and developed by Dr. Sven-Erik Willrich — a professional-grade decision analysis framework built on rigorous quantitative methods, designed to transform complex multi-criteria decisions into structured, transparent, and defensible outcomes.
>
> — [Dr. Sven-Erik Willrich, MCDA Framework](https://svenwillrich.de/mcda/)

## Quick Start

### Step 1: Download the Configuration File

Download the pre-configured MCDA configuration file: [mcda-cloud-deployment.csv](./mcda-cloud-deployment.csv)

This file contains all 14 criteria from the Cloud Deployment Decision Matrix.

### Step 2: Open the MCDA Tool

Navigate to: [https://svenwillrich.de/mcda/](https://svenwillrich.de/mcda/)

### Step 3: Upload the Configuration

1. Click on **CSV** in the upper right corner
2. Switch to **Import**
3. Select the downloaded `mcda-cloud-deployment.csv` file
4. Click on **Import 14 Criteria ...**
4. The tool will load all criteria automatically

### Step 4: Check the Scoring for the Variable Criteria

The scoring for the variable criteria **Vendor lock-in risk**, **Architectural suitability** and **Costs (TCO 3-5 years)** were predefined in the configuration file. Adjust them regarding your requirements. For more details see [Decision Matrix - Variable Criteria](../../en/src/decision-matrix.md#variable-criteria)


### Step 5: Customize Your Weights

The configuration comes with equal weights for all criteria. Adjust the weights based on your priorities:

1. In the MCDA interface, locate the **Weights** section
2. Adjust values for each criterion:
   - **Higher weight** = More important for your decision
   - **Lower weight** = Less important for your decision

**Example weight adjustments:**
- High priority on **Costs**: Set to 20
- High priority on **Security & Control**: Set to 15
- Lower priority on **Innovation**: Set to 5

### Step 6: Review Results

The MCDA tool will calculate scores for each deployment option based on your weights.