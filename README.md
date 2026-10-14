# Awesome-Retail-Inventory-Stock-Allocation-Systems

## Top Retail Inventory Stock Allocation Systems Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Demand Forecasting, Automated Replenishment & Multi-Echelon Inventory Optimization*  

**Last updated: March 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Retail Inventory Stock Allocation Systems**. These tools help retailers and distributors decide what stock to hold where, when to reorder, and how to allocate inventory across stores, warehouses, and fulfillment centers — using probabilistic forecasting, weather signals, and multi-echelon optimization to hit service targets without drowning in excess stock.



**Examples** include Nextail, Invent Analytics, ToolsGroup, Blue Yonder, Manhattan Associates, RELEX Solutions, Celect (Nike), Impact Analytics, Slimstock, and Kinaxis (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, custom replenishment policies, and transparent forecasting — ideal for retail engineers prioritizing data sovereignty, developers building inventory pipelines, and teams avoiding per-SKU enterprise licensing.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[ToolsGroup](https://www.toolsgroup.com/)**  

  Service-driven supply chain planning platform built on **Decion**, an agentic decision intelligence system unifying demand, inventory, and replenishment planning. Specializes in **probabilistic forecasting for long-tail, intermittent, and highly seasonal demand** — modeling the full range of demand rather than a single fragile number. Features dynamic multi-echelon inventory optimization (MEIO), smart network rebalancing, margin-driven replenishment tunnels, and scenario-driven S&OP. Recognized in the Gartner Magic Quadrant for Supply Chain Planning .



- **[RELEX Solutions](https://www.relexsolutions.com/)**  

  Unified retail and supply chain planning platform with automated **store replenishment**, allocation, and inventory optimization. Achieves **99%+ availability with less inventory** (reported 30% inventory reduction). Features the **Inventory Control AI agent** that transforms strategic inventory targets into optimized actions across thousands of SKUs with real-time profit impact. Medovia (Swedish pharma wholesaler) reports **92% of order proposals used unaltered**, with availability up 1.3pp. Neighborhood Intelligence (Bed Bath & Beyond, The Container Store) uses RELEX for unified forecasting, replenishment, and allocation across 335+ stores .



- **[Blue Yonder](https://blueyonder.com/)**  

  End-to-end supply chain platform with demand forecasting, inventory optimization, and automated replenishment for retail and distribution.



- **[Manhattan Associates](https://www.manh.com/)**  

  Omnichannel supply chain commerce platform with inventory optimization, demand forecasting, and allocation capabilities.



- **[Slimstock](https://www.slimstock.com/)**  

  Inventory optimization and demand planning platform focused on reducing stock while improving service levels.



- **[Kinaxis](https://www.kinaxis.com/)**  

  Concurrent planning platform for supply chain orchestration with demand, inventory, and supply planning.



- **[Nextail](https://www.nextail.co/)**  

  AI-powered merchandise planning and inventory allocation platform for fashion retail, optimizing stock distribution across stores.



- **[Invent Analytics](https://www.inventanalytics.com/)**  

  AI-driven retail planning platform with demand forecasting, inventory optimization, and allocation.



- **[Impact Analytics](https://www.impactanalytics.ai/)**  

  AI-powered retail planning and inventory management with assortment, pricing, and replenishment optimization.



- **[Celect (Nike)](https://www.celect.com/)**  

  AI-powered inventory optimization and demand forecasting platform acquired by Nike.



## Open-Source GitHub Projects



- **[Stockcast](https://pypi.org/project/stockcast/)**  

  **The most complete open-source library for turning forecasts into inventory decisions.** A forecast is not a decision — Stockcast is the layer between the forecast and the replenishment order. Maps forecasts from any model into orders, simulates execution against historical or simulated demand, and evaluates business metrics (cost, service, waste). Features **OrderUpToPolicy** for order-up-to replenishment, **SimulationEngine** with explicit receive-decide-meet clock, **InventoryEvaluator** with fill rate and average on-hand metrics. Built from composable Lego-like pieces you can subclass. Handles **1,000 SKUs of daily order-up-to decisions in 10-12 seconds**. From VIVES University of Applied Sciences research group .



- **[supplycm](https://pypi.org/project/supplycm/)**  

  **397 supply chain management algorithms with zero external dependencies** — pure Python, standard library only. Inventory module (60 algorithms): EOQ/EPQ, newsvendor, lot-sizing, ABC/XYZ analysis. Forecasting module (50 algorithms): moving averages, exponential smoothing, **Croston** (for intermittent demand), AR/MA. Also includes MRP (BOM explosion, kanban), demand sensing (seasonality, cannibalization), simulation (Monte Carlo inventory), and supplier selection (AHP, TOPSIS). MIT licensed, Python 3.6+ .



- **[inventorylibx](https://pypi.org/project/inventorylibx/)**  

  Python library for core inventory calculations: **Economic Order Quantity (EOQ)**, **Reorder Point (ROP)**, **Safety Stock**, Total Inventory Cost, and EOQ with Bulk Discount. Includes CLI script for easy usage .



- **[backorder](https://pypi.org/project/backorder/)**  

  Lightweight, **zero-dependency** Python utility for e-commerce inventory management and backorder mitigation. Provides EOQ, Safety Stock calculation, and Reorder Point (ROP) modeling through an `InventoryModel` class. Explicitly designed as mathematical models for supply chain estimates — not a replacement for full ERP systems .



- **[inventory_optimization_simulator.py](https://zenodo.org/records/18029448)**  

  Single-file **Multi-Product EOQ Simulator** with stochastic normal demand, safety stock and reorder point calculation (~95% service level), annual cost modeling, and **quantum-inspired lateral rebalancing heuristic** simulating tunneling across inventory silos. Optional visualization with sawtooth inventory plots and donut cost breakdowns. MIT licensed .



- **[Open-Inventory-Manager](https://pkg.go.dev/github.com/SumukhaS291299/Open-Inventory-Manager)**  

  Lightweight, high-performance inventory management backend in Go with Gin and **BadgerDB** (embedded key/value database). Features async persistence, thread-safe in-memory inventory model, JSON API, supplier metadata support, and Docker multi-stage build. MIT licensed — suitable for building custom inventory services .



- **[BizzAI](https://github.com/orion-ai-community/BizzAI)**  

  Comprehensive open-source POS and inventory management system built with MERN stack. Features fast billing, custom PDF invoicing, real-time stock tracking, low-stock alerts, customer/supplier management, and Docker deployment with CI/CD pipeline. Includes seed data for development .



### Additional Strong Open-Source Options



- **GitHub Topic: inventory-optimization** — Community projects covering demand forecasting, safety stock calculators, and replenishment simulators.

- **GitHub Topic: supply-chain-management** — Broader collection including MRP engines, warehouse management, and logistics optimization.

- **Prophet + LSTM hybrid models** — Academic implementations combining trend/seasonality decomposition with deep learning residuals for SKU-store-region hierarchy forecasting. Reported mean R² improvement from 0.840 to 0.887 at monthly level in CPG retail benchmarks .

- **Weather-integrated forecasting** — Research shows weather-informed models achieve **11.5% mean sMAPE reduction** versus baseline across retail sub-industries. Grocery, casual dining, and home improvement respond to weather through distinct mechanisms (stockpiling, mobility elasticity, seasonal feasibility) .



**Frameworks for building custom systems**: Combine **Stockcast** for forecast-to-decision simulation and policy evaluation, **supplycm** for 397 classical algorithms including Croston forecasting and ABC/XYZ analysis, **inventorylibx** or **backorder** for EOQ/ROP/safety stock fundamentals, and **Open-Inventory-Manager** or **BizzAI** for the operational inventory layer. For weather-driven demand, layer external weather APIs into the forecasting pipeline before passing quantile forecasts to Stockcast's `OrderUpToPolicy`.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Retail inventory systems involve significant financial and operational decisions. Forecasts and replenishment policies must be validated against historical performance and business constraints before production deployment. Weather-driven demand patterns are category-specific and require empirical calibration .

- Self-hosted open-source solutions require proper integration with POS/ERP systems, data quality validation, and ongoing model monitoring.



---



**Made for retail planners, supply chain analysts, inventory managers, and developers building demand forecasting and replenishment platforms.**  

Let's make retail inventory allocation more open, data-driven, and stockout-resistant.
