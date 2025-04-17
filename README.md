# Investment-bank-trading-and-dashboard

## Objective
Build a responsive dashboard for clients and advisors to monitor stocks, execute trades, and analyze portfolios in real time.

## Tech Stack
- **Backend**: 
  - Spring Boot (Microservices)
  - Graphql API
  - Mapstruct
  - Netflix DGS
  - WebSockets (Real-time updates)
  - Kafka (Event streaming)
    
  
- **Frontend**: 
  - React.ts 
  - Chart.js (Visualisations)
  - Tanstack Query
  - ag-grid
  - Bootstrap
 
- **Other toola and platforms**: 
  - Github actions CI
  - MongoDB cloud
  - AWS ECR and EKS
  - 

## Key Features
- Live stock price updates using a market data API (e.g., Alpha Vantage, Yahoo Finance)
- Buy/Sell order placement with simulated execution
- Portfolio performance tracking (P&L, asset allocation)
- Role-based views (Clients vs. Advisors)

## Actors
- **Client**: Individual or Institutional Investor
- **Advisor**: Wealth Manager
- **Stock Market Data Provider**: e.g., Alpha Vantage, IEX Cloud
- **Order Execution Service**: Simulated or real brokerage API

## User Activities

| User Role | Actions |
|-----------|---------|
| **Client** | - View real-time stock prices<br>- Place buy/sell orders<br>- Track portfolio performance<br>- Set price alerts |
| **Advisor** | - Monitor client portfolios<br>- Execute trades on behalf of clients<br>- Generate reports<br>- Annotate trades (e.g., "Tax-Loss Harvesting") |
| **System** | - Fetch real-time market data<br>- Validate orders (balance, compliance)<br>- Simulate trade execution<br>- Send notifications |

## Key System Components

| Component            | Technology                        | Responsibility                        |
|---------------------|----------------------------------|--------------------------------------|
| **API Gateway**     | Spring Cloud Gateway             | Route requests to microservices      |
| **Market Data Service** | Spring Boot + WebSocket       | Stream real-time prices              |
| **Order Service**   | Spring Boot + Kafka              | Process buy/sell orders              |
| **Portfolio Service**| Spring Boot + PostgreSQL        | Track holdings/performance            |
| **Auth Service**    | Spring Security + JWT            | Role-based access control            |
| **Frontend**        | React.ts + Redux                 | Interactive dashboard                |

## Installation
1. **Update later
