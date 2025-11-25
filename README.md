# Stablecoin

## Project Overview

This project analyzes the Ethereum stablecoin ecosystem (USDC and USDT), exploring wallet activity, transaction volume, and token flows across different entities. The analysis leverages blockchain transfer data, labeled addresses (CEX, DEX, lending, bridges, and treasury multisigs), and transaction metadata to generate insights on ecosystem behavior, wallet concentration, and transaction distribution.

## Action

Analyzed $300B+ stablecoin ecosystem on Ethereum using ERC20 transfer data. Explored wallet activity, transaction patterns, and token flows using SQL, Python, and visualization tools.

## Key skills/tools

Python (Pandas, Matplotlib/Seaborn), SQL (BigQuery/Dune), Power BI/Tableau for dashboards

## Data Sources

erc20_ethereum.evt_Transfer
Source: Ethereum blockchain (ERC20 token transfers)
Columns:
from – sending wallet address
to – receiving wallet address
value – token transfer value (in raw units; converted in queries)
evt_block_time – timestamp of the transfer
contract_address – token contract address (USDC or USDT)
labels.addresses

Source: Dune Analytics label repository
Columns:
address – Ethereum wallet or contract address
name – human-readable name of entity
category – entity category (e.g., contracts, wallets, exchanges)
blockchain – blockchain identifier


This project was done in Dune where we get the data for stablecoins and the dashboard refreshes once every 24 hours
