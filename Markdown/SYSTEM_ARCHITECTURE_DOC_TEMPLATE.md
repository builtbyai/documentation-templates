---
title: System Architecture Documentation Template
created: 2025-12-28
enhanced: true
theme: indigo-violet
---

<div style="background: linear-gradient(135deg, #8b5cf6 0%, #7c3aed 100%); padding: 60px 40px; border-radius: 20px; color: white; text-align: center; margin: 40px 0; box-shadow: 0 20px 60px rgba(139, 92, 246, 0.4);">
  <h1 style="margin: 0 0 20px 0; font-size: 3em; font-weight: 800; text-shadow: 2px 2px 4px rgba(0,0,0,0.2);">🏗️ System Architecture</h1>
  <p style="font-size: 1.3em; margin: 0 0 30px 0; opacity: 0.95;">Professional Technical Documentation · Scalable Design · Enterprise Architecture</p>

  <div style="display: inline-flex; gap: 20px; flex-wrap: wrap; justify-content: center;">
    <div style="background: rgba(255,255,255,0.2); backdrop-filter: blur(10px); padding: 15px 30px; border-radius: 12px; border: 1px solid rgba(255,255,255,0.3);">
      <div style="font-size: 2em; font-weight: 700;">Enterprise</div>
      <div style="font-size: 0.9em; opacity: 0.9;">Grade System</div>
    </div>
    <div style="background: rgba(255,255,255,0.2); backdrop-filter: blur(10px); padding: 15px 30px; border-radius: 12px; border: 1px solid rgba(255,255,255,0.3);">
      <div style="font-size: 2em; font-weight: 700;">99.9%</div>
      <div style="font-size: 0.9em; opacity: 0.9;">Target Uptime</div>
    </div>
    <div style="background: rgba(255,255,255,0.2); backdrop-filter: blur(10px); padding: 15px 30px; border-radius: 12px; border: 1px solid rgba(255,255,255,0.3);">
      <div style="font-size: 2em; font-weight: 700;">Scalable</div>
      <div style="font-size: 0.9em; opacity: 0.9;">Architecture</div>
    </div>
  </div>
</div>

---

## 📑 Quick Navigation

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px; margin: 30px 0;">
  <a href="#overview" style="text-decoration: none;">
    <div style="background: linear-gradient(135deg, rgba(139, 92, 246, 0.1) 0%, rgba(124, 58, 237, 0.1) 100%); padding: 25px; border-radius: 12px; border: 2px solid #8b5cf6; transition: transform 0.2s, box-shadow 0.2s;">
      <div style="font-size: 2em; margin-bottom: 10px;">📊</div>
      <div style="color: #8b5cf6; font-weight: 700; font-size: 1.1em; margin-bottom: 8px;">Executive Overview</div>
      <div style="color: #6b7280; font-size: 0.9em;">System goals and context</div>
    </div>
  </a>

  <a href="#topology" style="text-decoration: none;">
    <div style="background: linear-gradient(135deg, rgba(139, 92, 246, 0.1) 0%, rgba(124, 58, 237, 0.1) 100%); padding: 25px; border-radius: 12px; border: 2px solid #8b5cf6; transition: transform 0.2s, box-shadow 0.2s;">
      <div style="font-size: 2em; margin-bottom: 10px;">🗺️</div>
      <div style="color: #8b5cf6; font-weight: 700; font-size: 1.1em; margin-bottom: 8px;">System Topology</div>
      <div style="color: #6b7280; font-size: 0.9em;">Architecture diagram</div>
    </div>
  </a>

  <a href="#components" style="text-decoration: none;">
    <div style="background: linear-gradient(135deg, rgba(139, 92, 246, 0.1) 0%, rgba(124, 58, 237, 0.1) 100%); padding: 25px; border-radius: 12px; border: 2px solid #8b5cf6; transition: transform 0.2s, box-shadow 0.2s;">
      <div style="font-size: 2em; margin-bottom: 10px;">🧩</div>
      <div style="color: #8b5cf6; font-weight: 700; font-size: 1.1em; margin-bottom: 8px;">Components</div>
      <div style="color: #6b7280; font-size: 0.9em;">System components matrix</div>
    </div>
  </a>

  <a href="#dataflow" style="text-decoration: none;">
    <div style="background: linear-gradient(135deg, rgba(139, 92, 246, 0.1) 0%, rgba(124, 58, 237, 0.1) 100%); padding: 25px; border-radius: 12px; border: 2px solid #8b5cf6; transition: transform 0.2s, box-shadow 0.2s;">
      <div style="font-size: 2em; margin-bottom: 10px;">🔄</div>
      <div style="color: #8b5cf6; font-weight: 700; font-size: 1.1em; margin-bottom: 8px;">Data Flow</div>
      <div style="color: #6b7280; font-size: 0.9em;">Request lifecycle</div>
    </div>
  </a>

  <a href="#security" style="text-decoration: none;">
    <div style="background: linear-gradient(135deg, rgba(139, 92, 246, 0.1) 0%, rgba(124, 58, 237, 0.1) 100%); padding: 25px; border-radius: 12px; border: 2px solid #8b5cf6; transition: transform 0.2s, box-shadow 0.2s;">
      <div style="font-size: 2em; margin-bottom: 10px;">🔒</div>
      <div style="color: #8b5cf6; font-weight: 700; font-size: 1.1em; margin-bottom: 8px;">Security</div>
      <div style="color: #6b7280; font-size: 0.9em;">Security architecture</div>
    </div>
  </a>

  <a href="#performance" style="text-decoration: none;">
    <div style="background: linear-gradient(135deg, rgba(139, 92, 246, 0.1) 0%, rgba(124, 58, 237, 0.1) 100%); padding: 25px; border-radius: 12px; border: 2px solid #8b5cf6; transition: transform 0.2s, box-shadow 0.2s;">
      <div style="font-size: 2em; margin-bottom: 10px;">⚡</div>
      <div style="color: #8b5cf6; font-weight: 700; font-size: 1.1em; margin-bottom: 8px;">Performance</div>
      <div style="color: #6b7280; font-size: 0.9em;">Metrics and targets</div>
    </div>
  </a>

  <a href="#deployment" style="text-decoration: none;">
    <div style="background: linear-gradient(135deg, rgba(139, 92, 246, 0.1) 0%, rgba(124, 58, 237, 0.1) 100%); padding: 25px; border-radius: 12px; border: 2px solid #8b5cf6; transition: transform 0.2s, box-shadow 0.2s;">
      <div style="font-size: 2em; margin-bottom: 10px;">🚀</div>
      <div style="color: #8b5cf6; font-weight: 700; font-size: 1.1em; margin-bottom: 8px;">Deployment</div>
      <div style="color: #6b7280; font-size: 0.9em;">CI/CD pipeline</div>
    </div>
  </a>

  <a href="#monitoring" style="text-decoration: none;">
    <div style="background: linear-gradient(135deg, rgba(139, 92, 246, 0.1) 0%, rgba(124, 58, 237, 0.1) 100%); padding: 25px; border-radius: 12px; border: 2px solid #8b5cf6; transition: transform 0.2s, box-shadow 0.2s;">
      <div style="font-size: 2em; margin-bottom: 10px;">📈</div>
      <div style="color: #8b5cf6; font-weight: 700; font-size: 1.1em; margin-bottom: 8px;">Monitoring</div>
      <div style="color: #6b7280; font-size: 0.9em;">Observability stack</div>
    </div>
  </a>
</div>

---

<a name="overview"></a>

## 📊 Executive Overview

<div style="background: linear-gradient(135deg, rgba(139, 92, 246, 0.05) 0%, rgba(124, 58, 237, 0.05) 100%); padding: 30px; border-radius: 14px; border: 2px solid #8b5cf6; margin: 25px 0;">
  <div style="display: grid; grid-template-columns: auto 1fr; gap: 20px; align-items: center;">
    <div style="font-size: 3em;">🏗️</div>
    <div>
      <div style="font-size: 1.5em; font-weight: 700; color: #8b5cf6; margin-bottom: 10px;">[SYSTEM_NAME]</div>
      <div style="color: #6b7280; font-size: 1.1em; margin-bottom: 15px;">[SYSTEM_TYPE] · [DEPLOYMENT_TARGET]</div>
      <div style="display: flex; gap: 15px; flex-wrap: wrap;">
        <span style="background: linear-gradient(135deg, #10b981 0%, #059669 100%); color: white; padding: 6px 14px; border-radius: 20px; font-size: 0.9em; font-weight: 600;">Status: [STATUS]</span>
        <span style="background: linear-gradient(135deg, #f59e0b 0%, #d97706 100%); color: white; padding: 6px 14px; border-radius: 20px; font-size: 0.9em; font-weight: 600;">ETA: [ETA]</span>
        <span style="background: linear-gradient(135deg, #8b5cf6 0%, #7c3aed 100%); color: white; padding: 6px 14px; border-radius: 20px; font-size: 0.9em; font-weight: 600;">Complexity: [LEVEL]</span>
      </div>
    </div>
  </div>
</div>

### 🎯 Context and Goals

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 20px; margin: 25px 0;">
  <div style="background: white; padding: 25px; border-radius: 12px; border-left: 4px solid #3b82f6; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
    <div style="color: #6b7280; font-size: 0.9em; margin-bottom: 8px; font-weight: 600;">🎯 BUSINESS GOAL</div>
    <div style="color: #1f2937; font-size: 1.1em; font-weight: 600;">[GOAL]</div>
  </div>

  <div style="background: white; padding: 25px; border-radius: 12px; border-left: 4px solid #10b981; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
    <div style="color: #6b7280; font-size: 0.9em; margin-bottom: 8px; font-weight: 600;">👥 PRIMARY USERS</div>
    <div style="color: #1f2937; font-size: 1.1em; font-weight: 600;">[USERS]</div>
  </div>

  <div style="background: white; padding: 25px; border-radius: 12px; border-left: 4px solid #8b5cf6; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
    <div style="color: #6b7280; font-size: 0.9em; margin-bottom: 8px; font-weight: 600;">📊 SUCCESS METRICS</div>
    <div style="color: #1f2937; font-size: 1.1em; font-weight: 600;">[METRICS]</div>
  </div>
</div>

---

<a name="topology"></a>

## 🗺️ System Topology

<div style="background: linear-gradient(135deg, rgba(139, 92, 246, 0.05) 0%, rgba(124, 58, 237, 0.05) 100%); padding: 30px; border-radius: 14px; border: 2px solid #8b5cf6; margin: 25px 0;">

### Architecture Overview

```mermaid
graph TD
  subgraph "🎨 Presentation Layer"
    A[Web UI<br/>React/Vue]
    B[Mobile App<br/>iOS/Android]
    C[Admin Dashboard<br/>Management]
  end

  subgraph "🌐 API Gateway Layer"
    D[API Gateway<br/>Kong/Nginx]
    E[Load Balancer<br/>HAProxy]
    F[Rate Limiter<br/>Redis]
  end

  subgraph "🔐 Security Layer"
    G[Auth Service<br/>OAuth2/JWT]
    H[WAF<br/>ModSecurity]
    I[Secret Manager<br/>Vault]
  end

  subgraph "⚙️ Business Logic Layer"
    J[User Service<br/>Node.js]
    K[Order Service<br/>Python]
    L[Payment Service<br/>Java]
    M[Notification Service<br/>Go]
  end

  subgraph "💾 Data Layer"
    N[(Primary DB<br/>PostgreSQL)]
    O[(Read Replica<br/>PostgreSQL)]
    P[(Cache<br/>Redis)]
    Q[(Message Queue<br/>RabbitMQ)]
  end

  subgraph "📊 Analytics Layer"
    R[Data Warehouse<br/>Snowflake]
    S[Analytics Engine<br/>Spark]
    T[ML Pipeline<br/>TensorFlow]
  end

  A --> D
  B --> D
  C --> D
  D --> E
  E --> F
  F --> G
  G --> H
  H --> J
  H --> K
  H --> L
  H --> M
  J --> N
  K --> N
  L --> N
  M --> Q
  N --> O
  J --> P
  K --> P
  N --> R
  R --> S
  S --> T
```

### 🎯 Layer Responsibilities

<table style="width: 100%; border-collapse: collapse; box-shadow: 0 4px 15px rgba(0,0,0,0.1); border-radius: 10px; overflow: hidden; margin: 25px 0;">
  <thead>
    <tr style="background: linear-gradient(135deg, #8b5cf6 0%, #7c3aed 100%); color: white;">
      <th style="padding: 15px; text-align: left; font-weight: 600;">Layer</th>
      <th style="padding: 15px; text-align: left; font-weight: 600;">Responsibility</th>
      <th style="padding: 15px; text-align: center; font-weight: 600;">Technology</th>
      <th style="padding: 15px; text-align: right; font-weight: 600;">Scale</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background: #faf5ff;">
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff; font-weight: 600;">🎨 Presentation</td>
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff;">User interface, rendering, client-side logic</td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #e9d5ff;">React, Vue, Mobile</td>
      <td style="padding: 12px; text-align: right; border-bottom: 1px solid #e9d5ff;">100K users</td>
    </tr>
    <tr style="background: white;">
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff; font-weight: 600;">🌐 API Gateway</td>
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff;">Routing, load balancing, rate limiting</td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #e9d5ff;">Kong, Nginx</td>
      <td style="padding: 12px; text-align: right; border-bottom: 1px solid #e9d5ff;">10K RPS</td>
    </tr>
    <tr style="background: #faf5ff;">
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff; font-weight: 600;">🔐 Security</td>
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff;">Authentication, authorization, secrets</td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #e9d5ff;">OAuth2, JWT, Vault</td>
      <td style="padding: 12px; text-align: right; border-bottom: 1px solid #e9d5ff;">5K auth/s</td>
    </tr>
    <tr style="background: white;">
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff; font-weight: 600;">⚙️ Business Logic</td>
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff;">Core business operations, workflows</td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #e9d5ff;">Microservices</td>
      <td style="padding: 12px; text-align: right; border-bottom: 1px solid #e9d5ff;">8K RPS</td>
    </tr>
    <tr style="background: #faf5ff;">
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff; font-weight: 600;">💾 Data</td>
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff;">Persistence, caching, messaging</td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #e9d5ff;">PostgreSQL, Redis</td>
      <td style="padding: 12px; text-align: right; border-bottom: 1px solid #e9d5ff;">10TB data</td>
    </tr>
    <tr style="background: white;">
      <td style="padding: 12px; font-weight: 600;">📊 Analytics</td>
      <td style="padding: 12px;">Data processing, ML, insights</td>
      <td style="padding: 12px; text-align: center;">Spark, TensorFlow</td>
      <td style="padding: 12px; text-align: right;">50TB processed</td>
    </tr>
  </tbody>
</table>

</div>

---

<a name="components"></a>

## 🧩 Component Responsibility Matrix

<table style="width: 100%; border-collapse: collapse; box-shadow: 0 4px 15px rgba(0,0,0,0.1); border-radius: 10px; overflow: hidden; margin: 25px 0;">
  <thead>
    <tr style="background: linear-gradient(135deg, #8b5cf6 0%, #7c3aed 100%); color: white;">
      <th style="padding: 15px; text-align: left; font-weight: 600;">Component</th>
      <th style="padding: 15px; text-align: left; font-weight: 600;">Function</th>
      <th style="padding: 15px; text-align: left; font-weight: 600;">Dependencies</th>
      <th style="padding: 15px; text-align: right; font-weight: 600;">Scale Target</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background: #faf5ff;">
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff; font-weight: 600;">API Gateway</td>
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff;">Request routing, authentication, rate limiting</td>
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff;">Auth Service, Load Balancer</td>
      <td style="padding: 12px; text-align: right; border-bottom: 1px solid #e9d5ff; color: #10b981; font-weight: 700;">10,000 RPS</td>
    </tr>
    <tr style="background: white;">
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff; font-weight: 600;">User Service</td>
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff;">User profiles, preferences, session management</td>
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff;">Primary DB, Redis Cache</td>
      <td style="padding: 12px; text-align: right; border-bottom: 1px solid #e9d5ff; color: #10b981; font-weight: 700;">5,000 users</td>
    </tr>
    <tr style="background: #faf5ff;">
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff; font-weight: 600;">Order Service</td>
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff;">Order processing, inventory, fulfillment</td>
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff;">Payment Service, Message Queue</td>
      <td style="padding: 12px; text-align: right; border-bottom: 1px solid #e9d5ff; color: #10b981; font-weight: 700;">1,000 orders/min</td>
    </tr>
    <tr style="background: white;">
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff; font-weight: 600;">Payment Service</td>
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff;">Payment processing, refunds, billing</td>
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff;">External Payment Gateway</td>
      <td style="padding: 12px; text-align: right; border-bottom: 1px solid #e9d5ff; color: #10b981; font-weight: 700;">500 transactions/min</td>
    </tr>
    <tr style="background: #faf5ff;">
      <td style="padding: 12px; font-weight: 600;">Notification Service</td>
      <td style="padding: 12px;">Email, SMS, push notifications</td>
      <td style="padding: 12px;">Message Queue, External APIs</td>
      <td style="padding: 12px; text-align: right; color: #10b981; font-weight: 700;">2,000 notifications/min</td>
    </tr>
  </tbody>
</table>

### 📦 Component Details

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 20px; margin: 25px 0;">
  <div style="background: white; padding: 25px; border-radius: 12px; border-left: 4px solid #3b82f6; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
    <div style="font-size: 1.8em; margin-bottom: 10px;">🌐</div>
    <div style="color: #3b82f6; font-weight: 700; font-size: 1.2em; margin-bottom: 10px;">API Gateway</div>
    <div style="color: #6b7280; font-size: 0.95em; line-height: 1.6;">
      <strong>Technology:</strong> Kong/Nginx<br/>
      <strong>Replicas:</strong> 5 instances<br/>
      <strong>CPU:</strong> 4 cores<br/>
      <strong>Memory:</strong> 8GB
    </div>
  </div>

  <div style="background: white; padding: 25px; border-radius: 12px; border-left: 4px solid #10b981; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
    <div style="font-size: 1.8em; margin-bottom: 10px;">👤</div>
    <div style="color: #10b981; font-weight: 700; font-size: 1.2em; margin-bottom: 10px;">User Service</div>
    <div style="color: #6b7280; font-size: 0.95em; line-height: 1.6;">
      <strong>Technology:</strong> Node.js<br/>
      <strong>Replicas:</strong> 3 instances<br/>
      <strong>CPU:</strong> 2 cores<br/>
      <strong>Memory:</strong> 4GB
    </div>
  </div>

  <div style="background: white; padding: 25px; border-radius: 12px; border-left: 4px solid #f59e0b; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
    <div style="font-size: 1.8em; margin-bottom: 10px;">📦</div>
    <div style="color: #f59e0b; font-weight: 700; font-size: 1.2em; margin-bottom: 10px;">Order Service</div>
    <div style="color: #6b7280; font-size: 0.95em; line-height: 1.6;">
      <strong>Technology:</strong> Python<br/>
      <strong>Replicas:</strong> 4 instances<br/>
      <strong>CPU:</strong> 4 cores<br/>
      <strong>Memory:</strong> 8GB
    </div>
  </div>

  <div style="background: white; padding: 25px; border-radius: 12px; border-left: 4px solid #8b5cf6; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
    <div style="font-size: 1.8em; margin-bottom: 10px;">💳</div>
    <div style="color: #8b5cf6; font-weight: 700; font-size: 1.2em; margin-bottom: 10px;">Payment Service</div>
    <div style="color: #6b7280; font-size: 0.95em; line-height: 1.6;">
      <strong>Technology:</strong> Java<br/>
      <strong>Replicas:</strong> 3 instances<br/>
      <strong>CPU:</strong> 4 cores<br/>
      <strong>Memory:</strong> 8GB
    </div>
  </div>
</div>

---

<a name="dataflow"></a>

## 🔄 Data Flow & Request Lifecycle

<div style="background: linear-gradient(135deg, rgba(139, 92, 246, 0.05) 0%, rgba(124, 58, 237, 0.05) 100%); padding: 30px; border-radius: 14px; border: 2px solid #8b5cf6; margin: 25px 0;">

### Request Flow Sequence

```mermaid
sequenceDiagram
    participant U as 👤 User
    participant LB as ⚖️ Load Balancer
    participant G as 🌐 Gateway
    participant A as 🔐 Auth Service
    participant S as ⚙️ Business Service
    participant C as 💾 Cache
    participant D as 🗄️ Database
    participant Q as 📬 Message Queue
    participant N as 📧 Notification

    U->>LB: HTTP Request
    LB->>G: Route to Gateway
    G->>A: Validate Token
    A-->>G: Token Valid ✅
    G->>S: Execute Business Logic

    alt Cache Hit
        S->>C: Check Cache
        C-->>S: Return Cached Data
    else Cache Miss
        S->>D: Query Database
        D-->>S: Return Data
        S->>C: Update Cache
    end

    S->>Q: Publish Event
    Q->>N: Process Notification
    N-->>U: Send Email/SMS

    S-->>G: Response Data
    G-->>LB: Format Response
    LB-->>U: HTTP Response 200 OK

    Note over U,N: Average Response Time: 145ms
```

### 📊 Request Lifecycle Stages

<table style="width: 100%; border-collapse: collapse; box-shadow: 0 4px 15px rgba(0,0,0,0.1); border-radius: 10px; overflow: hidden; margin: 25px 0;">
  <thead>
    <tr style="background: linear-gradient(135deg, #8b5cf6 0%, #7c3aed 100%); color: white;">
      <th style="padding: 15px; text-align: left; font-weight: 600;">Stage</th>
      <th style="padding: 15px; text-align: left; font-weight: 600;">Action</th>
      <th style="padding: 15px; text-align: center; font-weight: 600;">Latency</th>
      <th style="padding: 15px; text-align: right; font-weight: 600;">Status</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background: #faf5ff;">
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff; font-weight: 600;">1. Load Balancer</td>
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff;">Route incoming request to available gateway</td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #e9d5ff;">~5ms</td>
      <td style="padding: 12px; text-align: right; border-bottom: 1px solid #e9d5ff;"><span style="color: #10b981; font-weight: 600;">✅ Active</span></td>
    </tr>
    <tr style="background: white;">
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff; font-weight: 600;">2. Authentication</td>
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff;">Validate JWT token, check permissions</td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #e9d5ff;">~15ms</td>
      <td style="padding: 12px; text-align: right; border-bottom: 1px solid #e9d5ff;"><span style="color: #10b981; font-weight: 600;">✅ Active</span></td>
    </tr>
    <tr style="background: #faf5ff;">
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff; font-weight: 600;">3. Business Logic</td>
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff;">Execute service logic, process request</td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #e9d5ff;">~80ms</td>
      <td style="padding: 12px; text-align: right; border-bottom: 1px solid #e9d5ff;"><span style="color: #10b981; font-weight: 600;">✅ Active</span></td>
    </tr>
    <tr style="background: white;">
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff; font-weight: 600;">4. Data Access</td>
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff;">Query cache or database for data</td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #e9d5ff;">~30ms</td>
      <td style="padding: 12px; text-align: right; border-bottom: 1px solid #e9d5ff;"><span style="color: #10b981; font-weight: 600;">✅ Active</span></td>
    </tr>
    <tr style="background: #faf5ff;">
      <td style="padding: 12px; font-weight: 600;">5. Response</td>
      <td style="padding: 12px;">Format and return response to client</td>
      <td style="padding: 12px; text-align: center;">~15ms</td>
      <td style="padding: 12px; text-align: right;"><span style="color: #10b981; font-weight: 600;">✅ Active</span></td>
    </tr>
  </tbody>
</table>

</div>

### 📋 Data Contracts & API Specifications

<table style="width: 100%; border-collapse: collapse; box-shadow: 0 4px 15px rgba(0,0,0,0.1); border-radius: 10px; overflow: hidden; margin: 25px 0;">
  <thead>
    <tr style="background: linear-gradient(135deg, #8b5cf6 0%, #7c3aed 100%); color: white;">
      <th style="padding: 15px; text-align: left; font-weight: 600;">API Endpoint</th>
      <th style="padding: 15px; text-align: center; font-weight: 600;">Method</th>
      <th style="padding: 15px; text-align: left; font-weight: 600;">Request Schema</th>
      <th style="padding: 15px; text-align: left; font-weight: 600;">Response Schema</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background: #faf5ff;">
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff; font-weight: 600;">/v1/users</td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #e9d5ff;"><span style="background: #3b82f6; color: white; padding: 4px 10px; border-radius: 6px; font-size: 0.85em;">GET</span></td>
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff;"><code>[QUERY_PARAMS]</code></td>
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff;"><code>[USER_LIST_RESPONSE]</code></td>
    </tr>
    <tr style="background: white;">
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff; font-weight: 600;">/v1/orders</td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #e9d5ff;"><span style="background: #10b981; color: white; padding: 4px 10px; border-radius: 6px; font-size: 0.85em;">POST</span></td>
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff;"><code>[ORDER_CREATE_REQUEST]</code></td>
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff;"><code>[ORDER_ID_RESPONSE]</code></td>
    </tr>
    <tr style="background: #faf5ff;">
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff; font-weight: 600;">/v1/payments</td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #e9d5ff;"><span style="background: #10b981; color: white; padding: 4px 10px; border-radius: 6px; font-size: 0.85em;">POST</span></td>
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff;"><code>[PAYMENT_REQUEST]</code></td>
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff;"><code>[PAYMENT_CONFIRMATION]</code></td>
    </tr>
    <tr style="background: white;">
      <td style="padding: 12px; font-weight: 600;">/v1/users/{id}</td>
      <td style="padding: 12px; text-align: center;"><span style="background: #f59e0b; color: white; padding: 4px 10px; border-radius: 6px; font-size: 0.85em;">PUT</span></td>
      <td style="padding: 12px;"><code>[USER_UPDATE_REQUEST]</code></td>
      <td style="padding: 12px;"><code>[USER_RESPONSE]</code></td>
    </tr>
  </tbody>
</table>

---

<a name="security"></a>

## 🔒 Security Architecture

<div style="background: linear-gradient(135deg, rgba(239, 68, 68, 0.05) 0%, rgba(220, 38, 38, 0.05) 100%); padding: 30px; border-radius: 14px; border: 2px solid #ef4444; margin: 25px 0;">

### Security Checklist

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 15px; margin: 20px 0;">
  <div style="background: white; padding: 20px; border-radius: 10px; border-left: 4px solid #10b981;">
    <div style="display: flex; align-items: center; gap: 10px; margin-bottom: 10px;">
      <span style="font-size: 1.5em;">✅</span>
      <span style="color: #10b981; font-weight: 700; font-size: 1.1em;">JWT Token Authentication</span>
    </div>
    <div style="color: #6b7280; font-size: 0.9em;">Stateless authentication with 15-minute expiry</div>
  </div>

  <div style="background: white; padding: 20px; border-radius: 10px; border-left: 4px solid #10b981;">
    <div style="display: flex; align-items: center; gap: 10px; margin-bottom: 10px;">
      <span style="font-size: 1.5em;">✅</span>
      <span style="color: #10b981; font-weight: 700; font-size: 1.1em;">Role-Based Access Control</span>
    </div>
    <div style="color: #6b7280; font-size: 0.9em;">Granular permissions with least privilege</div>
  </div>

  <div style="background: white; padding: 20px; border-radius: 10px; border-left: 4px solid #f59e0b;">
    <div style="display: flex; align-items: center; gap: 10px; margin-bottom: 10px;">
      <span style="font-size: 1.5em;">🚧</span>
      <span style="color: #f59e0b; font-weight: 700; font-size: 1.1em;">Multi-Factor Authentication</span>
    </div>
    <div style="color: #6b7280; font-size: 0.9em;">In progress: TOTP and SMS verification</div>
  </div>

  <div style="background: white; padding: 20px; border-radius: 10px; border-left: 4px solid #ef4444;">
    <div style="display: flex; align-items: center; gap: 10px; margin-bottom: 10px;">
      <span style="font-size: 1.5em;">📋</span>
      <span style="color: #ef4444; font-weight: 700; font-size: 1.1em;">API Key Rotation</span>
    </div>
    <div style="color: #6b7280; font-size: 0.9em;">Planned: Automated 90-day rotation</div>
  </div>

  <div style="background: white; padding: 20px; border-radius: 10px; border-left: 4px solid #10b981;">
    <div style="display: flex; align-items: center; gap: 10px; margin-bottom: 10px;">
      <span style="font-size: 1.5em;">✅</span>
      <span style="color: #10b981; font-weight: 700; font-size: 1.1em;">TLS 1.3 Encryption</span>
    </div>
    <div style="color: #6b7280; font-size: 0.9em;">End-to-end encryption for all traffic</div>
  </div>

  <div style="background: white; padding: 20px; border-radius: 10px; border-left: 4px solid #10b981;">
    <div style="display: flex; align-items: center; gap: 10px; margin-bottom: 10px;">
      <span style="font-size: 1.5em;">✅</span>
      <span style="color: #10b981; font-weight: 700; font-size: 1.1em;">Secrets Management</span>
    </div>
    <div style="color: #6b7280; font-size: 0.9em;">HashiCorp Vault for credential storage</div>
  </div>
</div>

### Security Data Flow

```mermaid
graph TD
    A[🌐 Client Request] --> B{🔐 TLS Termination}
    B -->|Encrypted| C[🛡️ WAF Layer]
    C -->|Validated| D{🔑 Auth Check}
    D -->|Valid Token| E[👮 RBAC Guards]
    D -->|Invalid| F[❌ 401 Unauthorized]
    E -->|Authorized| G[⚙️ Business Logic]
    E -->|Denied| H[❌ 403 Forbidden]
    G --> I{💾 Data Access}
    I -->|Encrypted| J[(🔒 Encrypted Data)]
    J -->|Decrypted| K[📊 Response Data]
    K --> L[🔐 Response Encryption]
    L --> M[✅ Secure Response]

    style B fill:#10b981,color:#fff
    style D fill:#3b82f6,color:#fff
    style E fill:#8b5cf6,color:#fff
    style F fill:#ef4444,color:#fff
    style H fill:#ef4444,color:#fff
    style J fill:#f59e0b,color:#fff
```

### 🛡️ Security Layers

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px; margin: 25px 0;">
  <div style="background: white; padding: 25px; border-radius: 12px; border-left: 4px solid #ef4444; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
    <div style="font-size: 1.8em; margin-bottom: 10px;">🛡️</div>
    <div style="color: #ef4444; font-weight: 700; font-size: 1.2em; margin-bottom: 10px;">Network Security</div>
    <div style="color: #6b7280; font-size: 0.95em; line-height: 1.6;">
      • WAF (ModSecurity)<br/>
      • DDoS Protection<br/>
      • IP Whitelisting<br/>
      • Rate Limiting
    </div>
  </div>

  <div style="background: white; padding: 25px; border-radius: 12px; border-left: 4px solid #f59e0b; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
    <div style="font-size: 1.8em; margin-bottom: 10px;">🔐</div>
    <div style="color: #f59e0b; font-weight: 700; font-size: 1.2em; margin-bottom: 10px;">Application Security</div>
    <div style="color: #6b7280; font-size: 0.95em; line-height: 1.6;">
      • Input Validation<br/>
      • SQL Injection Prevention<br/>
      • XSS Protection<br/>
      • CSRF Tokens
    </div>
  </div>

  <div style="background: white; padding: 25px; border-radius: 12px; border-left: 4px solid #8b5cf6; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
    <div style="font-size: 1.8em; margin-bottom: 10px;">🔑</div>
    <div style="color: #8b5cf6; font-weight: 700; font-size: 1.2em; margin-bottom: 10px;">Access Control</div>
    <div style="color: #6b7280; font-size: 0.95em; line-height: 1.6;">
      • OAuth 2.0<br/>
      • JWT Tokens<br/>
      • RBAC Policies<br/>
      • Session Management
    </div>
  </div>

  <div style="background: white; padding: 25px; border-radius: 12px; border-left: 4px solid #10b981; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
    <div style="font-size: 1.8em; margin-bottom: 10px;">💾</div>
    <div style="color: #10b981; font-weight: 700; font-size: 1.2em; margin-bottom: 10px;">Data Security</div>
    <div style="color: #6b7280; font-size: 0.95em; line-height: 1.6;">
      • Encryption at Rest<br/>
      • Encryption in Transit<br/>
      • Database Encryption<br/>
      • Backup Encryption
    </div>
  </div>
</div>

</div>

---

<a name="performance"></a>

## ⚡ Performance Dashboard

<div style="background: linear-gradient(135deg, rgba(139, 92, 246, 0.05) 0%, rgba(124, 58, 237, 0.05) 100%); padding: 30px; border-radius: 14px; border: 2px solid #8b5cf6; margin: 25px 0;">

### Current Performance Metrics

<table style="width: 100%; border-collapse: collapse; box-shadow: 0 4px 15px rgba(0,0,0,0.1); border-radius: 10px; overflow: hidden; margin: 25px 0;">
  <thead>
    <tr style="background: linear-gradient(135deg, #8b5cf6 0%, #7c3aed 100%); color: white;">
      <th style="padding: 15px; text-align: left; font-weight: 600;">Metric</th>
      <th style="padding: 15px; text-align: center; font-weight: 600;">Target</th>
      <th style="padding: 15px; text-align: center; font-weight: 600;">Current</th>
      <th style="padding: 15px; text-align: right; font-weight: 600;">Status</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background: #faf5ff;">
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff; font-weight: 600;">⚡ Response Time (P95)</td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #e9d5ff;">< 200ms</td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #e9d5ff; color: #10b981; font-weight: 700; font-size: 1.2em;">145ms</td>
      <td style="padding: 12px; text-align: right; border-bottom: 1px solid #e9d5ff;"><span style="color: #10b981; font-weight: 600;">✅ Excellent</span></td>
    </tr>
    <tr style="background: white;">
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff; font-weight: 600;">🔄 Throughput</td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #e9d5ff;">2,500 RPS</td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #e9d5ff; color: #10b981; font-weight: 700; font-size: 1.2em;">2,400 RPS</td>
      <td style="padding: 12px; text-align: right; border-bottom: 1px solid #e9d5ff;"><span style="color: #10b981; font-weight: 600;">✅ Good</span></td>
    </tr>
    <tr style="background: #faf5ff;">
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff; font-weight: 600;">📈 Uptime</td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #e9d5ff;">> 99.5%</td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #e9d5ff; color: #10b981; font-weight: 700; font-size: 1.2em;">99.9%</td>
      <td style="padding: 12px; text-align: right; border-bottom: 1px solid #e9d5ff;"><span style="color: #10b981; font-weight: 600;">✅ Excellent</span></td>
    </tr>
    <tr style="background: white;">
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff; font-weight: 600;">💾 Cache Hit Rate</td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #e9d5ff;">> 80%</td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #e9d5ff; color: #10b981; font-weight: 700; font-size: 1.2em;">85%</td>
      <td style="padding: 12px; text-align: right; border-bottom: 1px solid #e9d5ff;"><span style="color: #10b981; font-weight: 600;">✅ Excellent</span></td>
    </tr>
    <tr style="background: #faf5ff;">
      <td style="padding: 12px; font-weight: 600;">❌ Error Rate</td>
      <td style="padding: 12px; text-align: center;">< 0.1%</td>
      <td style="padding: 12px; text-align: center; color: #10b981; font-weight: 700; font-size: 1.2em;">0.05%</td>
      <td style="padding: 12px; text-align: right;"><span style="color: #10b981; font-weight: 600;">✅ Excellent</span></td>
    </tr>
  </tbody>
</table>

### 📊 Performance Breakdown

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 20px; margin: 25px 0;">
  <div style="background: white; padding: 20px; border-radius: 12px; box-shadow: 0 4px 15px rgba(0,0,0,0.1); text-align: center;">
    <div style="font-size: 2.5em; font-weight: 700; color: #10b981; margin-bottom: 5px;">145ms</div>
    <div style="color: #6b7280; font-weight: 600; margin-bottom: 10px;">P95 Response Time</div>
    <div style="background: #e5e7eb; height: 8px; border-radius: 10px; overflow: hidden;">
      <div style="background: linear-gradient(90deg, #10b981 0%, #059669 100%); height: 100%; width: 72%;"></div>
    </div>
    <div style="color: #10b981; font-size: 0.85em; margin-top: 5px;">Target: 200ms</div>
  </div>

  <div style="background: white; padding: 20px; border-radius: 12px; box-shadow: 0 4px 15px rgba(0,0,0,0.1); text-align: center;">
    <div style="font-size: 2.5em; font-weight: 700; color: #3b82f6; margin-bottom: 5px;">2,400</div>
    <div style="color: #6b7280; font-weight: 600; margin-bottom: 10px;">Requests/Second</div>
    <div style="background: #e5e7eb; height: 8px; border-radius: 10px; overflow: hidden;">
      <div style="background: linear-gradient(90deg, #3b82f6 0%, #2563eb 100%); height: 100%; width: 96%;"></div>
    </div>
    <div style="color: #3b82f6; font-size: 0.85em; margin-top: 5px;">Target: 2,500 RPS</div>
  </div>

  <div style="background: white; padding: 20px; border-radius: 12px; box-shadow: 0 4px 15px rgba(0,0,0,0.1); text-align: center;">
    <div style="font-size: 2.5em; font-weight: 700; color: #8b5cf6; margin-bottom: 5px;">99.9%</div>
    <div style="color: #6b7280; font-weight: 600; margin-bottom: 10px;">Uptime</div>
    <div style="background: #e5e7eb; height: 8px; border-radius: 10px; overflow: hidden;">
      <div style="background: linear-gradient(90deg, #8b5cf6 0%, #7c3aed 100%); height: 100%; width: 100%;"></div>
    </div>
    <div style="color: #8b5cf6; font-size: 0.85em; margin-top: 5px;">Target: 99.5%</div>
  </div>

  <div style="background: white; padding: 20px; border-radius: 12px; box-shadow: 0 4px 15px rgba(0,0,0,0.1); text-align: center;">
    <div style="font-size: 2.5em; font-weight: 700; color: #f59e0b; margin-bottom: 5px;">85%</div>
    <div style="color: #6b7280; font-weight: 600; margin-bottom: 10px;">Cache Hit Rate</div>
    <div style="background: #e5e7eb; height: 8px; border-radius: 10px; overflow: hidden;">
      <div style="background: linear-gradient(90deg, #f59e0b 0%, #d97706 100%); height: 100%; width: 85%;"></div>
    </div>
    <div style="color: #f59e0b; font-size: 0.85em; margin-top: 5px;">Target: 80%</div>
  </div>
</div>

</div>

---

<a name="monitoring"></a>

## 📈 Observability & Monitoring

<div style="background: linear-gradient(135deg, rgba(139, 92, 246, 0.05) 0%, rgba(124, 58, 237, 0.05) 100%); padding: 30px; border-radius: 14px; border: 2px solid #8b5cf6; margin: 25px 0;">

### Monitoring Stack

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px; margin: 25px 0;">
  <div style="background: white; padding: 25px; border-radius: 12px; border-left: 4px solid #3b82f6; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
    <div style="font-size: 1.8em; margin-bottom: 10px;">📊</div>
    <div style="color: #3b82f6; font-weight: 700; font-size: 1.2em; margin-bottom: 10px;">Logs</div>
    <div style="color: #6b7280; font-size: 0.95em; line-height: 1.6;">
      <strong>System:</strong> ELK Stack<br/>
      <strong>Location:</strong> [LOG_LOCATION]<br/>
      <strong>Retention:</strong> 30 days<br/>
      <strong>Volume:</strong> 500GB/day
    </div>
  </div>

  <div style="background: white; padding: 25px; border-radius: 12px; border-left: 4px solid #10b981; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
    <div style="font-size: 1.8em; margin-bottom: 10px;">📈</div>
    <div style="color: #10b981; font-weight: 700; font-size: 1.2em; margin-bottom: 10px;">Metrics</div>
    <div style="color: #6b7280; font-size: 0.95em; line-height: 1.6;">
      <strong>System:</strong> Prometheus<br/>
      <strong>Dashboard:</strong> [DASHBOARD_URL]<br/>
      <strong>Interval:</strong> 15 seconds<br/>
      <strong>Metrics:</strong> 10K+ series
    </div>
  </div>

  <div style="background: white; padding: 25px; border-radius: 12px; border-left: 4px solid #f59e0b; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
    <div style="font-size: 1.8em; margin-bottom: 10px;">🔍</div>
    <div style="color: #f59e0b; font-weight: 700; font-size: 1.2em; margin-bottom: 10px;">Traces</div>
    <div style="color: #6b7280; font-size: 0.95em; line-height: 1.6;">
      <strong>System:</strong> Jaeger<br/>
      <strong>Location:</strong> [TRACING_URL]<br/>
      <strong>Sampling:</strong> 10%<br/>
      <strong>Latency:</strong> <50ms
    </div>
  </div>

  <div style="background: white; padding: 25px; border-radius: 12px; border-left: 4px solid #ef4444; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
    <div style="font-size: 1.8em; margin-bottom: 10px;">🚨</div>
    <div style="color: #ef4444; font-weight: 700; font-size: 1.2em; margin-bottom: 10px;">Alerts</div>
    <div style="color: #6b7280; font-size: 0.95em; line-height: 1.6;">
      <strong>System:</strong> PagerDuty<br/>
      <strong>Channel:</strong> [ALERT_CHANNEL]<br/>
      <strong>Rules:</strong> 50+ alerts<br/>
      <strong>Response:</strong> <5min
    </div>
  </div>
</div>

### 🎯 Key Observability Metrics

<table style="width: 100%; border-collapse: collapse; box-shadow: 0 4px 15px rgba(0,0,0,0.1); border-radius: 10px; overflow: hidden; margin: 25px 0;">
  <thead>
    <tr style="background: linear-gradient(135deg, #8b5cf6 0%, #7c3aed 100%); color: white;">
      <th style="padding: 15px; text-align: left; font-weight: 600;">Category</th>
      <th style="padding: 15px; text-align: left; font-weight: 600;">Metric</th>
      <th style="padding: 15px; text-align: center; font-weight: 600;">Tool</th>
      <th style="padding: 15px; text-align: right; font-weight: 600;">Alert Threshold</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background: #faf5ff;">
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff; font-weight: 600;">⚡ Performance</td>
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff;">Response time P95</td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #e9d5ff;">Prometheus</td>
      <td style="padding: 12px; text-align: right; border-bottom: 1px solid #e9d5ff;">> 300ms</td>
    </tr>
    <tr style="background: white;">
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff; font-weight: 600;">📊 Availability</td>
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff;">Service uptime</td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #e9d5ff;">Pingdom</td>
      <td style="padding: 12px; text-align: right; border-bottom: 1px solid #e9d5ff;">< 99.5%</td>
    </tr>
    <tr style="background: #faf5ff;">
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff; font-weight: 600;">❌ Error Rate</td>
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff;">5xx responses</td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #e9d5ff;">ELK</td>
      <td style="padding: 12px; text-align: right; border-bottom: 1px solid #e9d5ff;">> 0.5%</td>
    </tr>
    <tr style="background: white;">
      <td style="padding: 12px; font-weight: 600;">💾 Database</td>
      <td style="padding: 12px;">Query duration P95</td>
      <td style="padding: 12px; text-align: center;">Datadog</td>
      <td style="padding: 12px; text-align: right;">> 100ms</td>
    </tr>
  </tbody>
</table>

</div>

---

## ❌ Error Handling & Recovery

<div style="background: linear-gradient(135deg, rgba(239, 68, 68, 0.05) 0%, rgba(220, 38, 38, 0.05) 100%); padding: 30px; border-radius: 14px; border: 2px solid #ef4444; margin: 25px 0;">

### Error Handling Flow

```mermaid
flowchart TD
    A[📥 Request] --> B{✅ Valid Input?}
    B -->|No| C[❌ 400 Bad Request]
    B -->|Yes| D[⚙️ Process Request]
    D --> E{🗄️ DB Available?}
    E -->|No| F[❌ 503 Service Unavailable]
    E -->|Yes| G{💾 Data Exists?}
    G -->|No| H[❌ 404 Not Found]
    G -->|Yes| I{🔐 Authorized?}
    I -->|No| J[❌ 403 Forbidden]
    I -->|Yes| K[✅ 200 Success]

    C --> L[📊 Log Error]
    F --> L
    H --> L
    J --> L
    L --> M[📈 Update Metrics]
    M --> N[🚨 Send Alert if Critical]

    style C fill:#ef4444,color:#fff
    style F fill:#ef4444,color:#fff
    style H fill:#ef4444,color:#fff
    style J fill:#ef4444,color:#fff
    style K fill:#10b981,color:#fff
```

### 🔧 Error Recovery Strategies

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 20px; margin: 25px 0;">
  <div style="background: white; padding: 25px; border-radius: 12px; border-left: 4px solid #3b82f6; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
    <div style="font-size: 1.8em; margin-bottom: 10px;">🔄</div>
    <div style="color: #3b82f6; font-weight: 700; font-size: 1.2em; margin-bottom: 10px;">Retry Logic</div>
    <div style="color: #6b7280; font-size: 0.95em; line-height: 1.6;">
      <strong>Strategy:</strong> Exponential backoff<br/>
      <strong>Max Retries:</strong> 3 attempts<br/>
      <strong>Initial Delay:</strong> 100ms<br/>
      <strong>Max Delay:</strong> 2 seconds
    </div>
  </div>

  <div style="background: white; padding: 25px; border-radius: 12px; border-left: 4px solid #10b981; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
    <div style="font-size: 1.8em; margin-bottom: 10px;">⚡</div>
    <div style="color: #10b981; font-weight: 700; font-size: 1.2em; margin-bottom: 10px;">Circuit Breaker</div>
    <div style="color: #6b7280; font-size: 0.95em; line-height: 1.6;">
      <strong>Threshold:</strong> 50% error rate<br/>
      <strong>Window:</strong> 10 seconds<br/>
      <strong>Timeout:</strong> 30 seconds<br/>
      <strong>Half-Open:</strong> 1 request
    </div>
  </div>

  <div style="background: white; padding: 25px; border-radius: 12px; border-left: 4px solid #f59e0b; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
    <div style="font-size: 1.8em; margin-bottom: 10px;">🛡️</div>
    <div style="color: #f59e0b; font-weight: 700; font-size: 1.2em; margin-bottom: 10px;">Fallback</div>
    <div style="color: #6b7280; font-size: 0.95em; line-height: 1.6;">
      <strong>Primary:</strong> Live database<br/>
      <strong>Fallback:</strong> Cache layer<br/>
      <strong>Emergency:</strong> Static data<br/>
      <strong>Timeout:</strong> 5 seconds
    </div>
  </div>

  <div style="background: white; padding: 25px; border-radius: 12px; border-left: 4px solid #8b5cf6; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
    <div style="font-size: 1.8em; margin-bottom: 10px;">📊</div>
    <div style="color: #8b5cf6; font-weight: 700; font-size: 1.2em; margin-bottom: 10px;">Rate Limiting</div>
    <div style="color: #6b7280; font-size: 0.95em; line-height: 1.6;">
      <strong>Global:</strong> 10,000 req/min<br/>
      <strong>Per User:</strong> 100 req/min<br/>
      <strong>Burst:</strong> 200 requests<br/>
      <strong>Response:</strong> 429 status
    </div>
  </div>
</div>

</div>

---

<a name="deployment"></a>

## 🚀 Deployment Pipeline

<div style="background: linear-gradient(135deg, rgba(139, 92, 246, 0.05) 0%, rgba(124, 58, 237, 0.05) 100%); padding: 30px; border-radius: 14px; border: 2px solid #8b5cf6; margin: 25px 0;">

### CI/CD Workflow

```mermaid
flowchart LR
    A[📝 Commit] --> B[🧪 Unit Tests]
    B --> C[🔒 Security Scan]
    C --> D[🏗️ Build]
    D --> E[📦 Package]
    E --> F[🚀 Deploy to Staging]
    F --> G{✅ Tests Pass?}
    G -->|Yes| H[🎯 Deploy to Production]
    G -->|No| I[❌ Rollback]
    I --> J[🐛 Fix Issues]
    J --> A
    H --> K[📊 Monitor]
    K --> L{🚨 Issues?}
    L -->|Yes| M[⚡ Auto-Rollback]
    L -->|No| N[✅ Success]

    style A fill:#8b5cf6,color:#fff
    style H fill:#10b981,color:#fff
    style I fill:#ef4444,color:#fff
    style M fill:#ef4444,color:#fff
    style N fill:#10b981,color:#fff
```

### 🎯 Deployment Stages

<table style="width: 100%; border-collapse: collapse; box-shadow: 0 4px 15px rgba(0,0,0,0.1); border-radius: 10px; overflow: hidden; margin: 25px 0;">
  <thead>
    <tr style="background: linear-gradient(135deg, #8b5cf6 0%, #7c3aed 100%); color: white;">
      <th style="padding: 15px; text-align: left; font-weight: 600;">Stage</th>
      <th style="padding: 15px; text-align: left; font-weight: 600;">Action</th>
      <th style="padding: 15px; text-align: center; font-weight: 600;">Duration</th>
      <th style="padding: 15px; text-align: right; font-weight: 600;">Gate</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background: #faf5ff;">
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff; font-weight: 600;">1. Build</td>
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff;">Compile, bundle, optimize assets</td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #e9d5ff;">~3 min</td>
      <td style="padding: 12px; text-align: right; border-bottom: 1px solid #e9d5ff;"><span style="color: #10b981;">✅ Auto</span></td>
    </tr>
    <tr style="background: white;">
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff; font-weight: 600;">2. Test</td>
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff;">Run unit, integration, E2E tests</td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #e9d5ff;">~5 min</td>
      <td style="padding: 12px; text-align: right; border-bottom: 1px solid #e9d5ff;"><span style="color: #10b981;">✅ Auto</span></td>
    </tr>
    <tr style="background: #faf5ff;">
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff; font-weight: 600;">3. Security</td>
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff;">Vulnerability scan, SAST, DAST</td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #e9d5ff;">~4 min</td>
      <td style="padding: 12px; text-align: right; border-bottom: 1px solid #e9d5ff;"><span style="color: #10b981;">✅ Auto</span></td>
    </tr>
    <tr style="background: white;">
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff; font-weight: 600;">4. Staging</td>
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff;">Deploy to staging environment</td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #e9d5ff;">~2 min</td>
      <td style="padding: 12px; text-align: right; border-bottom: 1px solid #e9d5ff;"><span style="color: #10b981;">✅ Auto</span></td>
    </tr>
    <tr style="background: #faf5ff;">
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff; font-weight: 600;">5. Validation</td>
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff;">Smoke tests, health checks</td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #e9d5ff;">~3 min</td>
      <td style="padding: 12px; text-align: right; border-bottom: 1px solid #e9d5ff;"><span style="color: #f59e0b;">👤 Manual</span></td>
    </tr>
    <tr style="background: white;">
      <td style="padding: 12px; font-weight: 600;">6. Production</td>
      <td style="padding: 12px;">Rolling deployment to production</td>
      <td style="padding: 12px; text-align: center;">~5 min</td>
      <td style="padding: 12px; text-align: right;"><span style="color: #f59e0b;">👤 Approval</span></td>
    </tr>
  </tbody>
</table>

### 🌍 Environments

<table style="width: 100%; border-collapse: collapse; box-shadow: 0 4px 15px rgba(0,0,0,0.1); border-radius: 10px; overflow: hidden; margin: 25px 0;">
  <thead>
    <tr style="background: linear-gradient(135deg, #8b5cf6 0%, #7c3aed 100%); color: white;">
      <th style="padding: 15px; text-align: left; font-weight: 600;">Environment</th>
      <th style="padding: 15px; text-align: left; font-weight: 600;">URL</th>
      <th style="padding: 15px; text-align: center; font-weight: 600;">Last Deploy</th>
      <th style="padding: 15px; text-align: right; font-weight: 600;">Owner</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background: #faf5ff;">
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff; font-weight: 600;">🛠️ Development</td>
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff;"><code>[DEV_URL]</code></td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #e9d5ff;">[DATE]</td>
      <td style="padding: 12px; text-align: right; border-bottom: 1px solid #e9d5ff;">[DEV_OWNER]</td>
    </tr>
    <tr style="background: white;">
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff; font-weight: 600;">🧪 Staging</td>
      <td style="padding: 12px; border-bottom: 1px solid #e9d5ff;"><code>[STAGING_URL]</code></td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #e9d5ff;">[DATE]</td>
      <td style="padding: 12px; text-align: right; border-bottom: 1px solid #e9d5ff;">[STAGING_OWNER]</td>
    </tr>
    <tr style="background: #faf5ff;">
      <td style="padding: 12px; font-weight: 600;">🚀 Production</td>
      <td style="padding: 12px;"><code>[PROD_URL]</code></td>
      <td style="padding: 12px; text-align: center;">[DATE]</td>
      <td style="padding: 12px; text-align: right;">[PROD_OWNER]</td>
    </tr>
  </tbody>
</table>

</div>

---

## 📋 Architecture Decision Records (ADRs)

<div style="background: linear-gradient(135deg, rgba(139, 92, 246, 0.05) 0%, rgba(124, 58, 237, 0.05) 100%); padding: 30px; border-radius: 14px; border: 2px solid #8b5cf6; margin: 25px 0;">

<div style="background: linear-gradient(135deg, rgba(139, 92, 246, 0.08) 0%, rgba(124, 58, 237, 0.08) 100%); padding: 20px; border-radius: 10px; margin-bottom: 25px; border-left: 4px solid #8b5cf6;">
  <div style="color: #8b5cf6; font-weight: 700; font-size: 1.1em; margin-bottom: 8px;">📌 About ADRs</div>
  <div style="color: #6b7280; font-size: 0.95em; line-height: 1.6;">Architecture Decision Records document significant architectural decisions made during system design and evolution. Each ADR captures the context, decision, and consequences to provide historical insight and rationale for future maintainers.</div>
</div>

### ADR Template Structure

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 15px; margin: 25px 0;">
  <div style="background: white; padding: 20px; border-radius: 10px; border-top: 4px solid #8b5cf6; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
    <div style="font-size: 1.5em; margin-bottom: 10px;">📝</div>
    <div style="color: #8b5cf6; font-weight: 700; margin-bottom: 5px;">Context</div>
    <div style="color: #6b7280; font-size: 0.9em;">Why was this decision needed?</div>
  </div>

  <div style="background: white; padding: 20px; border-radius: 10px; border-top: 4px solid #3b82f6; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
    <div style="font-size: 1.5em; margin-bottom: 10px;">🎯</div>
    <div style="color: #3b82f6; font-weight: 700; margin-bottom: 5px;">Decision</div>
    <div style="color: #6b7280; font-size: 0.9em;">What was decided and why?</div>
  </div>

  <div style="background: white; padding: 20px; border-radius: 10px; border-top: 4px solid #10b981; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
    <div style="font-size: 1.5em; margin-bottom: 10px;">⚖️</div>
    <div style="color: #10b981; font-weight: 700; margin-bottom: 5px;">Consequences</div>
    <div style="color: #6b7280; font-size: 0.9em;">What are the trade-offs?</div>
  </div>

  <div style="background: white; padding: 20px; border-radius: 10px; border-top: 4px solid #f59e0b; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
    <div style="font-size: 1.5em; margin-bottom: 10px;">📊</div>
    <div style="color: #f59e0b; font-weight: 700; margin-bottom: 5px;">Status</div>
    <div style="color: #6b7280; font-size: 0.9em;">Proposed, Accepted, Deprecated</div>
  </div>
</div>

### Example ADRs

<div style="margin: 25px 0;">

#### ADR-001: Database Selection (PostgreSQL)

<div style="background: white; padding: 25px; border-radius: 12px; border-left: 4px solid #10b981; box-shadow: 0 4px 15px rgba(0,0,0,0.1); margin: 20px 0;">
  <div style="display: flex; align-items: center; justify-content: space-between; margin-bottom: 15px;">
    <div style="color: #1f2937; font-weight: 700; font-size: 1.15em;">PostgreSQL as Primary Database</div>
    <span style="background: linear-gradient(135deg, #10b981 0%, #059669 100%); color: white; padding: 6px 14px; border-radius: 20px; font-size: 0.85em; font-weight: 600;">Accepted</span>
  </div>

  <div style="color: #6b7280; line-height: 1.8; margin-bottom: 15px;">
    <strong style="color: #8b5cf6;">📝 Context:</strong> Need reliable ACID-compliant database for transactional workloads with complex querying requirements.
  </div>

  <div style="color: #6b7280; line-height: 1.8; margin-bottom: 15px;">
    <strong style="color: #8b5cf6;">🎯 Decision:</strong> Selected PostgreSQL over MySQL, MongoDB for ACID compliance, JSON support, advanced indexing, and proven scalability.
  </div>

  <div style="color: #6b7280; line-height: 1.8;">
    <strong style="color: #8b5cf6;">⚖️ Consequences:</strong>
    <ul style="margin: 10px 0; padding-left: 25px;">
      <li><span style="color: #10b981;">✅ Pros:</span> ACID guarantees, rich feature set, strong community, excellent tooling</li>
      <li><span style="color: #ef4444;">❌ Cons:</span> Higher resource usage vs NoSQL, steeper learning curve, complex replication setup</li>
    </ul>
  </div>

  <div style="color: #9ca3af; font-size: 0.85em; margin-top: 15px; padding-top: 15px; border-top: 1px solid #e5e7eb;">
    <strong>Date:</strong> 2024-01-15 | <strong>Author:</strong> [ARCHITECT_NAME] | <strong>Reviewers:</strong> [TEAM_NAMES]
  </div>
</div>

#### ADR-002: Microservices Architecture

<div style="background: white; padding: 25px; border-radius: 12px; border-left: 4px solid #10b981; box-shadow: 0 4px 15px rgba(0,0,0,0.1); margin: 20px 0;">
  <div style="display: flex; align-items: center; justify-content: space-between; margin-bottom: 15px;">
    <div style="color: #1f2937; font-weight: 700; font-size: 1.15em;">Microservices Over Monolith</div>
    <span style="background: linear-gradient(135deg, #10b981 0%, #059669 100%); color: white; padding: 6px 14px; border-radius: 20px; font-size: 0.85em; font-weight: 600;">Accepted</span>
  </div>

  <div style="color: #6b7280; line-height: 1.8; margin-bottom: 15px;">
    <strong style="color: #8b5cf6;">📝 Context:</strong> Scaling challenges with monolithic architecture, need for independent deployment cycles, team autonomy requirements.
  </div>

  <div style="color: #6b7280; line-height: 1.8; margin-bottom: 15px;">
    <strong style="color: #8b5cf6;">🎯 Decision:</strong> Adopt microservices architecture with service mesh (Istio), API gateway (Kong), and event-driven communication (RabbitMQ).
  </div>

  <div style="color: #6b7280; line-height: 1.8;">
    <strong style="color: #8b5cf6;">⚖️ Consequences:</strong>
    <ul style="margin: 10px 0; padding-left: 25px;">
      <li><span style="color: #10b981;">✅ Pros:</span> Independent scaling, faster deployments, team autonomy, fault isolation</li>
      <li><span style="color: #ef4444;">❌ Cons:</span> Increased operational complexity, distributed debugging challenges, network overhead</li>
    </ul>
  </div>

  <div style="color: #9ca3af; font-size: 0.85em; margin-top: 15px; padding-top: 15px; border-top: 1px solid #e5e7eb;">
    <strong>Date:</strong> 2024-02-10 | <strong>Author:</strong> [ARCHITECT_NAME] | <strong>Reviewers:</strong> [TEAM_NAMES]
  </div>
</div>

#### ADR-003: Caching Strategy (Redis)

<div style="background: white; padding: 25px; border-radius: 12px; border-left: 4px solid #10b981; box-shadow: 0 4px 15px rgba(0,0,0,0.1); margin: 20px 0;">
  <div style="display: flex; align-items: center; justify-content: space-between; margin-bottom: 15px;">
    <div style="color: #1f2937; font-weight: 700; font-size: 1.15em;">Redis for Distributed Caching</div>
    <span style="background: linear-gradient(135deg, #10b981 0%, #059669 100%); color: white; padding: 6px 14px; border-radius: 20px; font-size: 0.85em; font-weight: 600;">Accepted</span>
  </div>

  <div style="color: #6b7280; line-height: 1.8; margin-bottom: 15px;">
    <strong style="color: #8b5cf6;">📝 Context:</strong> High database load from repeated queries, need sub-10ms response times for frequently accessed data, session management requirements.
  </div>

  <div style="color: #6b7280; line-height: 1.8; margin-bottom: 15px;">
    <strong style="color: #8b5cf6;">🎯 Decision:</strong> Implement Redis Cluster for distributed caching with 80%+ hit rate target, TTL-based invalidation, and write-through pattern.
  </div>

  <div style="color: #6b7280; line-height: 1.8;">
    <strong style="color: #8b5cf6;">⚖️ Consequences:</strong>
    <ul style="margin: 10px 0; padding-left: 25px;">
      <li><span style="color: #10b981;">✅ Pros:</span> Sub-ms latency, reduced DB load, persistence support, rich data structures</li>
      <li><span style="color: #ef4444;">❌ Cons:</span> Cache invalidation complexity, memory costs, potential stale data issues</li>
    </ul>
  </div>

  <div style="color: #9ca3af; font-size: 0.85em; margin-top: 15px; padding-top: 15px; border-top: 1px solid #e5e7eb;">
    <strong>Date:</strong> 2024-03-05 | <strong>Author:</strong> [ARCHITECT_NAME] | <strong>Reviewers:</strong> [TEAM_NAMES]
  </div>
</div>

</div>

### ADR Decision Timeline

```mermaid
timeline
    title Architecture Decision Timeline
    2024-Q1 : ADR-001 Database Selection
           : ADR-002 Microservices Architecture
    2024-Q2 : ADR-003 Caching Strategy
           : ADR-004 Auth Service Design
    2024-Q3 : ADR-005 Monitoring Stack
           : ADR-006 CI/CD Pipeline
    2024-Q4 : ADR-007 Security Framework
```

</div>

---

## 🛡️ Disaster Recovery & Business Continuity

<div style="background: linear-gradient(135deg, rgba(239, 68, 68, 0.05) 0%, rgba(220, 38, 38, 0.05) 100%); padding: 30px; border-radius: 14px; border: 2px solid #ef4444; margin: 25px 0;">

<div style="background: linear-gradient(135deg, rgba(239, 68, 68, 0.08) 0%, rgba(220, 38, 38, 0.08) 100%); padding: 20px; border-radius: 10px; margin-bottom: 25px; border-left: 4px solid #ef4444;">
  <div style="color: #ef4444; font-weight: 700; font-size: 1.1em; margin-bottom: 8px;">⚠️ Critical Business Protection</div>
  <div style="color: #6b7280; font-size: 0.95em; line-height: 1.6;">Disaster Recovery Plan ensures business continuity during catastrophic failures. This section defines Recovery Time Objectives (RTO), Recovery Point Objectives (RPO), backup strategies, and incident response procedures.</div>
</div>

### 🎯 RTO/RPO Targets

<table style="width: 100%; border-collapse: collapse; box-shadow: 0 4px 15px rgba(0,0,0,0.1); border-radius: 10px; overflow: hidden; margin: 25px 0;">
  <thead>
    <tr style="background: linear-gradient(135deg, #ef4444 0%, #dc2626 100%); color: white;">
      <th style="padding: 15px; text-align: left; font-weight: 600;">Service Tier</th>
      <th style="padding: 15px; text-align: center; font-weight: 600;">RTO (Recovery Time)</th>
      <th style="padding: 15px; text-align: center; font-weight: 600;">RPO (Data Loss)</th>
      <th style="padding: 15px; text-align: left; font-weight: 600;">Impact</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background: #fef2f2;">
      <td style="padding: 12px; border-bottom: 1px solid #fecaca; font-weight: 600;">🔴 Critical (Tier 1)</td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #fecaca;"><span style="background: #ef4444; color: white; padding: 4px 10px; border-radius: 6px; font-size: 0.85em; font-weight: 600;">< 1 hour</span></td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #fecaca;"><span style="background: #ef4444; color: white; padding: 4px 10px; border-radius: 6px; font-size: 0.85em; font-weight: 600;">< 5 min</span></td>
      <td style="padding: 12px; border-bottom: 1px solid #fecaca;">Payment processing, user authentication, core transactions</td>
    </tr>
    <tr style="background: white;">
      <td style="padding: 12px; border-bottom: 1px solid #fecaca; font-weight: 600;">🟠 High (Tier 2)</td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #fecaca;"><span style="background: #f59e0b; color: white; padding: 4px 10px; border-radius: 6px; font-size: 0.85em; font-weight: 600;">< 4 hours</span></td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #fecaca;"><span style="background: #f59e0b; color: white; padding: 4px 10px; border-radius: 6px; font-size: 0.85em; font-weight: 600;">< 30 min</span></td>
      <td style="padding: 12px; border-bottom: 1px solid #fecaca;">Order management, inventory, notifications</td>
    </tr>
    <tr style="background: #fef2f2;">
      <td style="padding: 12px; font-weight: 600;">🟢 Medium (Tier 3)</td>
      <td style="padding: 12px; text-align: center;"><span style="background: #10b981; color: white; padding: 4px 10px; border-radius: 6px; font-size: 0.85em; font-weight: 600;">< 24 hours</span></td>
      <td style="padding: 12px; text-align: center;"><span style="background: #10b981; color: white; padding: 4px 10px; border-radius: 6px; font-size: 0.85em; font-weight: 600;">< 4 hours</span></td>
      <td style="padding: 12px;">Analytics, reporting, admin tools</td>
    </tr>
  </tbody>
</table>

### 💾 Backup Strategy

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 20px; margin: 25px 0;">
  <div style="background: white; padding: 25px; border-radius: 12px; border-left: 4px solid #3b82f6; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
    <div style="font-size: 1.8em; margin-bottom: 10px;">🗄️</div>
    <div style="color: #3b82f6; font-weight: 700; font-size: 1.2em; margin-bottom: 10px;">Database Backups</div>
    <div style="color: #6b7280; font-size: 0.95em; line-height: 1.6;">
      <strong>Frequency:</strong> Every 6 hours<br/>
      <strong>Retention:</strong> 30 days<br/>
      <strong>Location:</strong> Multi-region S3<br/>
      <strong>Encryption:</strong> AES-256
    </div>
  </div>

  <div style="background: white; padding: 25px; border-radius: 12px; border-left: 4px solid #10b981; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
    <div style="font-size: 1.8em; margin-bottom: 10px;">📸</div>
    <div style="color: #10b981; font-weight: 700; font-size: 1.2em; margin-bottom: 10px;">System Snapshots</div>
    <div style="color: #6b7280; font-size: 0.95em; line-height: 1.6;">
      <strong>Frequency:</strong> Daily<br/>
      <strong>Retention:</strong> 7 days<br/>
      <strong>Location:</strong> Cloud snapshots<br/>
      <strong>Type:</strong> Incremental
    </div>
  </div>

  <div style="background: white; padding: 25px; border-radius: 12px; border-left: 4px solid #f59e0b; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
    <div style="font-size: 1.8em; margin-bottom: 10px;">📋</div>
    <div style="color: #f59e0b; font-weight: 700; font-size: 1.2em; margin-bottom: 10px;">Config Backups</div>
    <div style="color: #6b7280; font-size: 0.95em; line-height: 1.6;">
      <strong>Frequency:</strong> On change<br/>
      <strong>Retention:</strong> Indefinite<br/>
      <strong>Location:</strong> Git repository<br/>
      <strong>Type:</strong> Version controlled
    </div>
  </div>
</div>

### ⚡ Failover Procedures

```mermaid
flowchart TD
    A[🚨 Disaster Detected] --> B{Severity?}
    B -->|Critical| C[📢 Page On-Call Team]
    B -->|High| D[📧 Alert Team]
    B -->|Medium| E[📊 Log & Monitor]

    C --> F[🔄 Initiate Failover]
    D --> F

    F --> G{Service Tier?}
    G -->|Tier 1| H[⚡ Immediate Failover<br/>Target: 15 min]
    G -->|Tier 2| I[🔧 Planned Failover<br/>Target: 2 hours]
    G -->|Tier 3| J[📅 Scheduled Recovery<br/>Target: 24 hours]

    H --> K[🔍 Verify Primary Failure]
    I --> K
    J --> K

    K --> L[🔀 Promote Replica]
    L --> M[✅ Health Checks]
    M --> N{Healthy?}

    N -->|Yes| O[📊 Monitor Performance]
    N -->|No| P[🔧 Troubleshoot Issues]
    P --> M

    O --> Q[📝 Update DNS/Load Balancer]
    Q --> R[✅ Service Restored]
    R --> S[📋 Post-Incident Review]

    style A fill:#ef4444,color:#fff
    style C fill:#ef4444,color:#fff
    style R fill:#10b981,color:#fff
    style H fill:#8b5cf6,color:#fff
```

### 🎯 Incident Response Playbook

<div style="background: white; padding: 25px; border-radius: 12px; border-left: 4px solid #ef4444; box-shadow: 0 4px 15px rgba(0,0,0,0.1); margin: 25px 0;">
  <div style="color: #ef4444; font-weight: 700; font-size: 1.2em; margin-bottom: 15px;">🔥 Critical Incident Response (< 1 hour RTO)</div>

  <div style="color: #6b7280; line-height: 1.8;">
    <strong style="color: #1f2937;">Phase 1: Detection & Alert (0-5 min)</strong>
    <ol style="margin: 10px 0; padding-left: 25px;">
      <li>Automated monitoring detects failure</li>
      <li>PagerDuty alerts on-call engineer</li>
      <li>Incident commander acknowledges alert</li>
      <li>War room channel created (Slack #incident-YYYYMMDD)</li>
    </ol>

    <strong style="color: #1f2937;">Phase 2: Assessment (5-15 min)</strong>
    <ol style="margin: 10px 0; padding-left: 25px;">
      <li>Check service health dashboards</li>
      <li>Review error logs and traces</li>
      <li>Assess scope: single service vs multi-service</li>
      <li>Determine if failover is required</li>
    </ol>

    <strong style="color: #1f2937;">Phase 3: Mitigation (15-45 min)</strong>
    <ol style="margin: 10px 0; padding-left: 25px;">
      <li>Execute automated failover runbook</li>
      <li>Verify replica health before promotion</li>
      <li>Update DNS/load balancer configuration</li>
      <li>Monitor for cascading failures</li>
    </ol>

    <strong style="color: #1f2937;">Phase 4: Verification (45-60 min)</strong>
    <ol style="margin: 10px 0; padding-left: 25px;">
      <li>Run smoke tests on recovered service</li>
      <li>Verify customer-facing functionality</li>
      <li>Check SLA compliance metrics</li>
      <li>All-clear declaration to stakeholders</li>
    </ol>
  </div>
</div>

### 📊 Recovery Validation Checklist

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 15px; margin: 20px 0;">
  <div style="background: white; padding: 20px; border-radius: 10px; border-left: 4px solid #10b981;">
    <div style="display: flex; align-items: center; gap: 10px; margin-bottom: 10px;">
      <span style="font-size: 1.5em;">✅</span>
      <span style="color: #10b981; font-weight: 700; font-size: 1.1em;">Service Availability</span>
    </div>
    <div style="color: #6b7280; font-size: 0.9em;">All critical services responding to health checks</div>
  </div>

  <div style="background: white; padding: 20px; border-radius: 10px; border-left: 4px solid #10b981;">
    <div style="display: flex; align-items: center; gap: 10px; margin-bottom: 10px;">
      <span style="font-size: 1.5em;">✅</span>
      <span style="color: #10b981; font-weight: 700; font-size: 1.1em;">Data Integrity</span>
    </div>
    <div style="color: #6b7280; font-size: 0.9em;">Database checksums verified, no corruption detected</div>
  </div>

  <div style="background: white; padding: 20px; border-radius: 10px; border-left: 4px solid #10b981;">
    <div style="display: flex; align-items: center; gap: 10px; margin-bottom: 10px;">
      <span style="font-size: 1.5em;">✅</span>
      <span style="color: #10b981; font-weight: 700; font-size: 1.1em;">Performance Metrics</span>
    </div>
    <div style="color: #6b7280; font-size: 0.9em;">Response times within SLA targets</div>
  </div>

  <div style="background: white; padding: 20px; border-radius: 10px; border-left: 4px solid #10b981;">
    <div style="display: flex; align-items: center; gap: 10px; margin-bottom: 10px;">
      <span style="font-size: 1.5em;">✅</span>
      <span style="color: #10b981; font-weight: 700; font-size: 1.1em;">User Impact</span>
    </div>
    <div style="color: #6b7280; font-size: 0.9em;">Customer-facing functionality fully restored</div>
  </div>
</div>

</div>

---

## ⚠️ Risk Register

<div style="background: linear-gradient(135deg, rgba(239, 68, 68, 0.05) 0%, rgba(220, 38, 38, 0.05) 100%); padding: 30px; border-radius: 14px; border: 2px solid #ef4444; margin: 25px 0;">

<table style="width: 100%; border-collapse: collapse; box-shadow: 0 4px 15px rgba(0,0,0,0.1); border-radius: 10px; overflow: hidden;">
  <thead>
    <tr style="background: linear-gradient(135deg, #ef4444 0%, #dc2626 100%); color: white;">
      <th style="padding: 15px; text-align: left; font-weight: 600;">Risk</th>
      <th style="padding: 15px; text-align: center; font-weight: 600;">Probability</th>
      <th style="padding: 15px; text-align: center; font-weight: 600;">Impact</th>
      <th style="padding: 15px; text-align: left; font-weight: 600;">Mitigation Strategy</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background: #fef2f2;">
      <td style="padding: 12px; border-bottom: 1px solid #fecaca; font-weight: 600;">Database Outage</td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #fecaca;"><span style="background: #f59e0b; color: white; padding: 4px 10px; border-radius: 6px; font-size: 0.85em;">MEDIUM</span></td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #fecaca;"><span style="background: #ef4444; color: white; padding: 4px 10px; border-radius: 6px; font-size: 0.85em;">HIGH</span></td>
      <td style="padding: 12px; border-bottom: 1px solid #fecaca;">Multi-region replicas, automated failover, backup every 6 hours</td>
    </tr>
    <tr style="background: white;">
      <td style="padding: 12px; border-bottom: 1px solid #fecaca; font-weight: 600;">DDoS Attack</td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #fecaca;"><span style="background: #f59e0b; color: white; padding: 4px 10px; border-radius: 6px; font-size: 0.85em;">MEDIUM</span></td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #fecaca;"><span style="background: #f59e0b; color: white; padding: 4px 10px; border-radius: 6px; font-size: 0.85em;">MEDIUM</span></td>
      <td style="padding: 12px; border-bottom: 1px solid #fecaca;">CloudFlare protection, rate limiting, auto-scaling, CDN caching</td>
    </tr>
    <tr style="background: #fef2f2;">
      <td style="padding: 12px; border-bottom: 1px solid #fecaca; font-weight: 600;">Security Breach</td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #fecaca;"><span style="background: #10b981; color: white; padding: 4px 10px; border-radius: 6px; font-size: 0.85em;">LOW</span></td>
      <td style="padding: 12px; text-align: center; border-bottom: 1px solid #fecaca;"><span style="background: #ef4444; color: white; padding: 4px 10px; border-radius: 6px; font-size: 0.85em;">HIGH</span></td>
      <td style="padding: 12px; border-bottom: 1px solid #fecaca;">WAF, penetration testing, SOC monitoring, incident response plan</td>
    </tr>
    <tr style="background: white;">
      <td style="padding: 12px; font-weight: 600;">Third-Party API Failure</td>
      <td style="padding: 12px; text-align: center;"><span style="background: #ef4444; color: white; padding: 4px 10px; border-radius: 6px; font-size: 0.85em;">HIGH</span></td>
      <td style="padding: 12px; text-align: center;"><span style="background: #f59e0b; color: white; padding: 4px 10px; border-radius: 6px; font-size: 0.85em;">MEDIUM</span></td>
      <td style="padding: 12px;">Circuit breakers, fallback mechanisms, multiple providers, caching</td>
    </tr>
  </tbody>
</table>

</div>

---

## 🔧 Troubleshooting Guide

<div style="background: linear-gradient(135deg, rgba(139, 92, 246, 0.05) 0%, rgba(124, 58, 237, 0.05) 100%); padding: 30px; border-radius: 14px; border: 2px solid #8b5cf6; margin: 25px 0;">

### Common Issues & Solutions

<div style="display: grid; grid-template-columns: 1fr; gap: 20px; margin: 25px 0;">
  <div style="background: white; padding: 25px; border-radius: 12px; border-left: 4px solid #ef4444; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
    <div style="color: #ef4444; font-weight: 700; font-size: 1.2em; margin-bottom: 15px;">❌ High Response Time</div>
    <div style="color: #6b7280; line-height: 1.8;">
      <strong style="color: #1f2937;">Symptom:</strong> API response time > 500ms<br/>
      <strong style="color: #1f2937;">Cause:</strong> Database query inefficiency, cache miss, network latency<br/>
      <strong style="color: #1f2937;">Fix:</strong>
      <ol style="margin: 10px 0; padding-left: 25px;">
        <li>Check slow query logs in database</li>
        <li>Verify cache hit rate (target: >80%)</li>
        <li>Review connection pool settings</li>
        <li>Enable query result caching</li>
      </ol>
    </div>
  </div>

  <div style="background: white; padding: 25px; border-radius: 12px; border-left: 4px solid #f59e0b; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
    <div style="color: #f59e0b; font-weight: 700; font-size: 1.2em; margin-bottom: 15px;">⚠️ Service Unavailable</div>
    <div style="color: #6b7280; line-height: 1.8;">
      <strong style="color: #1f2937;">Symptom:</strong> 503 errors, service health check failing<br/>
      <strong style="color: #1f2937;">Cause:</strong> Service crash, resource exhaustion, deployment issue<br/>
      <strong style="color: #1f2937;">Fix:</strong>
      <ol style="margin: 10px 0; padding-left: 25px;">
        <li>Check service logs for error messages</li>
        <li>Verify CPU/memory usage (alerts if >80%)</li>
        <li>Restart service pods/containers</li>
        <li>Rollback to previous stable version if needed</li>
      </ol>
    </div>
  </div>

  <div style="background: white; padding: 25px; border-radius: 12px; border-left: 4px solid #3b82f6; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
    <div style="color: #3b82f6; font-weight: 700; font-size: 1.2em; margin-bottom: 15px;">🔐 Authentication Failures</div>
    <div style="color: #6b7280; line-height: 1.8;">
      <strong style="color: #1f2937;">Symptom:</strong> 401 Unauthorized errors, token validation failing<br/>
      <strong style="color: #1f2937;">Cause:</strong> Expired tokens, secret rotation, clock skew<br/>
      <strong style="color: #1f2937;">Fix:</strong>
      <ol style="margin: 10px 0; padding-left: 25px;">
        <li>Verify JWT secret matches across services</li>
        <li>Check token expiration time (default: 15 min)</li>
        <li>Sync server time with NTP</li>
        <li>Review auth service logs for details</li>
      </ol>
    </div>
  </div>
</div>

</div>

---

## ✅ Validation Criteria

<div style="background: linear-gradient(135deg, rgba(16, 185, 129, 0.05) 0%, rgba(5, 150, 105, 0.05) 100%); padding: 30px; border-radius: 14px; border: 2px solid #10b981; margin: 25px 0;">

### Documentation Validation Checklist

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 15px; margin: 20px 0;">
  <div style="background: white; padding: 20px; border-radius: 10px; border-left: 4px solid #10b981;">
    <div style="display: flex; align-items: center; gap: 10px; margin-bottom: 10px;">
      <span style="font-size: 1.5em;">✅</span>
      <span style="color: #10b981; font-weight: 700; font-size: 1.1em;">Executable Procedures</span>
    </div>
    <div style="color: #6b7280; font-size: 0.9em;">All deployment and troubleshooting steps are actionable and complete</div>
  </div>

  <div style="background: white; padding: 20px; border-radius: 10px; border-left: 4px solid #10b981;">
    <div style="display: flex; align-items: center; gap: 10px; margin-bottom: 10px;">
      <span style="font-size: 1.5em;">✅</span>
      <span style="color: #10b981; font-weight: 700; font-size: 1.1em;">Runnable Code Samples</span>
    </div>
    <div style="color: #6b7280; font-size: 0.9em;">All code examples are correct, tested, and production-ready</div>
  </div>

  <div style="background: white; padding: 20px; border-radius: 10px; border-left: 4px solid #10b981;">
    <div style="display: flex; align-items: center; gap: 10px; margin-bottom: 10px;">
      <span style="font-size: 1.5em;">✅</span>
      <span style="color: #10b981; font-weight: 700; font-size: 1.1em;">Clear Recovery Steps</span>
    </div>
    <div style="color: #6b7280; font-size: 0.9em;">Troubleshooting guides provide step-by-step recovery procedures</div>
  </div>

  <div style="background: white; padding: 20px; border-radius: 10px; border-left: 4px solid #10b981;">
    <div style="display: flex; align-items: center; gap: 10px; margin-bottom: 10px;">
      <span style="font-size: 1.5em;">✅</span>
      <span style="color: #10b981; font-weight: 700; font-size: 1.1em;">Measurable Criteria</span>
    </div>
    <div style="color: #6b7280; font-size: 0.9em;">Success metrics are quantifiable and verifiable</div>
  </div>

  <div style="background: white; padding: 20px; border-radius: 10px; border-left: 4px solid #10b981;">
    <div style="display: flex; align-items: center; gap: 10px; margin-bottom: 10px;">
      <span style="font-size: 1.5em;">✅</span>
      <span style="color: #10b981; font-weight: 700; font-size: 1.1em;">Up-to-Date Diagrams</span>
    </div>
    <div style="color: #6b7280; font-size: 0.9em;">All Mermaid diagrams accurately reflect current architecture</div>
  </div>

  <div style="background: white; padding: 20px; border-radius: 10px; border-left: 4px solid #10b981;">
    <div style="display: flex; align-items: center; gap: 10px; margin-bottom: 10px;">
      <span style="font-size: 1.5em;">✅</span>
      <span style="color: #10b981; font-weight: 700; font-size: 1.1em;">Security Validated</span>
    </div>
    <div style="color: #6b7280; font-size: 0.9em;">All security measures documented and implemented</div>
  </div>
</div>

</div>

---

<div style="background: linear-gradient(135deg, #8b5cf6 0%, #7c3aed 100%); padding: 40px; border-radius: 20px; color: white; text-align: center; margin: 40px 0;">
  <div style="font-size: 2.5em; margin-bottom: 15px;">🎉 Architecture Documentation Complete! 🎉</div>
  <div style="font-size: 1.2em; opacity: 0.95; margin-bottom: 25px;">Professional system architecture with comprehensive technical documentation</div>
  <div style="display: inline-flex; gap: 15px; flex-wrap: wrap; justify-content: center;">
    <span style="background: rgba(255,255,255,0.2); padding: 8px 18px; border-radius: 20px; font-size: 0.9em;">🏗️ Enterprise Architecture</span>
    <span style="background: rgba(255,255,255,0.2); padding: 8px 18px; border-radius: 20px; font-size: 0.9em;">⚡ High Performance</span>
    <span style="background: rgba(255,255,255,0.2); padding: 8px 18px; border-radius: 20px; font-size: 0.9em;">🔒 Security First</span>
    <span style="background: rgba(255,255,255,0.2); padding: 8px 18px; border-radius: 20px; font-size: 0.9em;">📊 Observable</span>
  </div>
</div>

---

<div style="text-align: center; padding: 30px; background: #f9fafb; border-radius: 12px; margin: 30px 0;">
  <div style="color: #6b7280; font-size: 0.95em; line-height: 1.8;">
    <strong style="color: #8b5cf6;">Enhanced System Architecture Template</strong><br/>
    Created: 2025-12-28 | Enhanced with Indigo/Violet Theme<br/>
    <em>Professional technical documentation for enterprise systems</em>
  </div>
</div>
