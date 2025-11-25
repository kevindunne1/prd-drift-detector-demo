# PRD Drift Detector - Demo Repository

This repository contains a **sample PRD** and **GitHub Issues** to demonstrate the [PRD Drift Detector](https://github.com/kevindunne1/prd-drift-detector) tool.

## Purpose

Use this demo repo to test the PRD Drift Detector without creating your own test data.

## Contents

- **`docs/prd.md`**: Sample Product Requirements Document for an Analytics Dashboard Export feature
- **GitHub Issues**: 6 issues demonstrating various drift scenarios:
  - ✅ Delivered as planned
  - 🔄 In progress
  - ⚠️ Scope drift (PRD said X, delivered Y)
  - ❌ Missing features (not started)

## How to Use This Demo

1. Go to the [PRD Drift Detector](https://prd-drift-detector-mu1lhwua3-kevin-dunnes-projects.vercel.app)
2. Enter these details:
   - **Repository**: `kevindunne1/prd-drift-detector-demo`
   - **PRD Path**: `docs/prd.md`
   - **GitHub Token**: Your personal access token ([create one here](https://github.com/settings/tokens))
   - **Anthropic Key**: Your Claude API key ([get one here](https://console.anthropic.com/))
3. Click "Analyze PRD Drift"
4. View the results showing completion %, risk scores, and detailed drift analysis

## Expected Results

The analysis should detect:
- **Completion**: ~50-60% (some features delivered, some in progress, some missing)
- **Risk Score**: Medium-High (30-50)
- **Drift Examples**:
  - CSV export delivered as planned ✅
  - PDF export only partially complete (missing branding) ⚠️
  - Excel export missing entirely (but was out of scope) ✅
  - Dashboard refresh rate differs from spec (30s → 60s) ⚠️

## About the Tool

The PRD Drift Detector uses Claude AI to semantically match PRD requirements to GitHub Issues and detect drift between planned features and actual delivery.

Built by [Kevin Dunne](https://github.com/kevindunne1) as a portfolio demonstration of PM + technical execution.

---

**Want to try this on your own repository?** Check out the [main PRD Drift Detector repo](https://github.com/kevindunne1/prd-drift-detector) for instructions.
