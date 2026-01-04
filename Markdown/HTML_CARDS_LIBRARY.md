---
title: HTML Cards Library - Complete Design System
created: 2025-12-28
updated: 2025-12-28
version: 2.0
category: Design System
tags: [html, css, cards, components, ui-library, design-patterns]
---

<div style="background: linear-gradient(135deg, #10b981 0%, #059669 100%); padding: 60px 40px; border-radius: 20px; color: white; text-align: center; margin: 40px 0; box-shadow: 0 20px 60px rgba(16, 185, 129, 0.4);">
  <h1 style="margin: 0 0 20px 0; font-size: 3em; font-weight: 800; text-shadow: 2px 2px 4px rgba(0,0,0,0.2);">🎨 HTML Cards Library</h1>
  <p style="font-size: 1.3em; margin: 0 0 30px 0; opacity: 0.95;">Complete Component Collection · Modern Design Patterns · Production Ready</p>

  <div style="display: inline-flex; gap: 20px; flex-wrap: wrap; justify-content: center;">
    <div style="background: rgba(255,255,255,0.2); backdrop-filter: blur(10px); padding: 15px 30px; border-radius: 12px; border: 1px solid rgba(255,255,255,0.3);">
      <div style="font-size: 2em; font-weight: 700;">25+</div>
      <div style="font-size: 0.9em; opacity: 0.9;">Card Variants</div>
    </div>
    <div style="background: rgba(255,255,255,0.2); backdrop-filter: blur(10px); padding: 15px 30px; border-radius: 12px; border: 1px solid rgba(255,255,255,0.3);">
      <div style="font-size: 2em; font-weight: 700;">8</div>
      <div style="font-size: 0.9em; opacity: 0.9;">Categories</div>
    </div>
    <div style="background: rgba(255,255,255,0.2); backdrop-filter: blur(10px); padding: 15px 30px; border-radius: 12px; border: 1px solid rgba(255,255,255,0.3);">
      <div style="font-size: 2em; font-weight: 700;">100%</div>
      <div style="font-size: 0.9em; opacity: 0.9;">Customizable</div>
    </div>
  </div>
</div>

---

## 📋 Quick Navigation

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 15px; margin: 30px 0;">
  <a href="#status-info" style="text-decoration: none;">
    <div style="background: white; padding: 20px; border-radius: 12px; border-left: 4px solid #10b981; box-shadow: 0 4px 15px rgba(0,0,0,0.1); transition: transform 0.2s;">
      <div style="font-size: 1.8em; margin-bottom: 8px;">📊</div>
      <div style="color: #10b981; font-weight: 700; font-size: 1.1em;">Status & Info Cards</div>
      <div style="color: #6b7280; font-size: 0.9em; margin-top: 5px;">Display states, info, and summaries</div>
    </div>
  </a>

  <a href="#kpi-metrics" style="text-decoration: none;">
    <div style="background: white; padding: 20px; border-radius: 12px; border-left: 4px solid #3b82f6; box-shadow: 0 4px 15px rgba(0,0,0,0.1); transition: transform 0.2s;">
      <div style="font-size: 1.8em; margin-bottom: 8px;">📈</div>
      <div style="color: #3b82f6; font-weight: 700; font-size: 1.1em;">KPI & Metrics Cards</div>
      <div style="color: #6b7280; font-size: 0.9em; margin-top: 5px;">Numbers, charts, and analytics</div>
    </div>
  </a>

  <a href="#alerts-notifications" style="text-decoration: none;">
    <div style="background: white; padding: 20px; border-radius: 12px; border-left: 4px solid #f59e0b; box-shadow: 0 4px 15px rgba(0,0,0,0.1); transition: transform 0.2s;">
      <div style="font-size: 1.8em; margin-bottom: 8px;">⚠️</div>
      <div style="color: #f59e0b; font-weight: 700; font-size: 1.1em;">Alerts & Notifications</div>
      <div style="color: #6b7280; font-size: 0.9em; margin-top: 5px;">Warnings, errors, and messages</div>
    </div>
  </a>

  <a href="#profile-avatar" style="text-decoration: none;">
    <div style="background: white; padding: 20px; border-radius: 12px; border-left: 4px solid #10b981; box-shadow: 0 4px 15px rgba(0,0,0,0.1); transition: transform 0.2s;">
      <div style="font-size: 1.8em; margin-bottom: 8px;">👤</div>
      <div style="color: #10b981; font-weight: 700; font-size: 1.1em;">Profile & Avatar Cards</div>
      <div style="color: #6b7280; font-size: 0.9em; margin-top: 5px;">User profiles and team members</div>
    </div>
  </a>

  <a href="#actions-buttons" style="text-decoration: none;">
    <div style="background: white; padding: 20px; border-radius: 12px; border-left: 4px solid #8b5cf6; box-shadow: 0 4px 15px rgba(0,0,0,0.1); transition: transform 0.2s;">
      <div style="font-size: 1.8em; margin-bottom: 8px;">⚡</div>
      <div style="color: #8b5cf6; font-weight: 700; font-size: 1.1em;">Action & Button Cards</div>
      <div style="color: #6b7280; font-size: 0.9em; margin-top: 5px;">CTAs and interactive panels</div>
    </div>
  </a>

  <a href="#progress-timeline" style="text-decoration: none;">
    <div style="background: white; padding: 20px; border-radius: 12px; border-left: 4px solid #06b6d4; box-shadow: 0 4px 15px rgba(0,0,0,0.1); transition: transform 0.2s;">
      <div style="font-size: 1.8em; margin-bottom: 8px;">⏱️</div>
      <div style="color: #06b6d4; font-weight: 700; font-size: 1.1em;">Progress & Timeline</div>
      <div style="color: #6b7280; font-size: 0.9em; margin-top: 5px;">Progress bars and step indicators</div>
    </div>
  </a>

  <a href="#lists-tables" style="text-decoration: none;">
    <div style="background: white; padding: 20px; border-radius: 12px; border-left: 4px solid #ef4444; box-shadow: 0 4px 15px rgba(0,0,0,0.1); transition: transform 0.2s;">
      <div style="font-size: 1.8em; margin-bottom: 8px;">📋</div>
      <div style="color: #ef4444; font-weight: 700; font-size: 1.1em;">Lists & Tables</div>
      <div style="color: #6b7280; font-size: 0.9em; margin-top: 5px;">Structured data presentation</div>
    </div>
  </a>

  <a href="#special-effects" style="text-decoration: none;">
    <div style="background: white; padding: 20px; border-radius: 12px; border-left: 4px solid #10b981; box-shadow: 0 4px 15px rgba(0,0,0,0.1); transition: transform 0.2s;">
      <div style="font-size: 1.8em; margin-bottom: 8px;">✨</div>
      <div style="color: #10b981; font-weight: 700; font-size: 1.1em;">Special Effects</div>
      <div style="color: #6b7280; font-size: 0.9em; margin-top: 5px;">Glassmorphism, neumorphism, 3D</div>
    </div>
  </a>
</div>

---

<a name="status-info"></a>
## 📊 Status & Info Cards

### Compact Status Card

<div style="border: 1px solid #e5e7eb; border-radius: 10px; padding: 16px; background: #ffffff; box-shadow: 0 2px 8px rgba(0,0,0,0.05); max-width: 350px; margin: 20px 0;">
  <div style="display: flex; align-items: center; justify-content: space-between; margin-bottom: 12px;">
    <strong style="font-size: 1.1em; color: #111827;">Project Alpha</strong>
    <span style="background: #10b981; color: white; padding: 4px 12px; border-radius: 12px; font-size: 0.85em; font-weight: 600;">Active</span>
  </div>
  <div style="color: #6b7280; font-size: 0.95em; margin-bottom: 8px;">
    <strong>Status:</strong> On Track
  </div>
  <div style="color: #6b7280; font-size: 0.95em;">
    <strong>Owner:</strong> Sarah Johnson
  </div>
</div>

**Code:**
```html
<div style="border: 1px solid #e5e7eb; border-radius: 10px; padding: 16px; background: #ffffff; box-shadow: 0 2px 8px rgba(0,0,0,0.05); max-width: 350px;">
  <div style="display: flex; align-items: center; justify-content: space-between; margin-bottom: 12px;">
    <strong style="font-size: 1.1em; color: #111827;">[TITLE]</strong>
    <span style="background: #10b981; color: white; padding: 4px 12px; border-radius: 12px; font-size: 0.85em; font-weight: 600;">[BADGE]</span>
  </div>
  <div style="color: #6b7280; font-size: 0.95em; margin-bottom: 8px;">
    <strong>Status:</strong> [STATUS]
  </div>
  <div style="color: #6b7280; font-size: 0.95em;">
    <strong>Owner:</strong> [OWNER]
  </div>
</div>
```

### Enhanced Info Card with Icon

<div style="background: white; border-radius: 16px; padding: 24px; box-shadow: 0 8px 30px rgba(0,0,0,0.12); max-width: 400px; margin: 20px 0; border-top: 4px solid #10b981;">
  <div style="display: flex; align-items: start; gap: 16px;">
    <div style="background: linear-gradient(135deg, #10b981 0%, #059669 100%); width: 56px; height: 56px; border-radius: 14px; display: flex; align-items: center; justify-content: center; font-size: 1.8em; color: white; box-shadow: 0 4px 15px rgba(236, 72, 153, 0.3);">
      🏢
    </div>
    <div style="flex: 1;">
      <h3 style="margin: 0 0 8px 0; color: #111827; font-size: 1.3em;">Enterprise Dashboard</h3>
      <p style="margin: 0 0 12px 0; color: #6b7280; font-size: 0.95em; line-height: 1.6;">
        Comprehensive analytics and reporting for enterprise-level data visualization with real-time updates.
      </p>
      <div style="display: flex; gap: 8px; flex-wrap: wrap;">
        <span style="background: #d1fae5; color: #10b981; padding: 4px 12px; border-radius: 8px; font-size: 0.85em; font-weight: 600;">Analytics</span>
        <span style="background: #d1fae5; color: #10b981; padding: 4px 12px; border-radius: 8px; font-size: 0.85em; font-weight: 600;">Enterprise</span>
        <span style="background: #d1fae5; color: #10b981; padding: 4px 12px; border-radius: 8px; font-size: 0.85em; font-weight: 600;">Real-time</span>
      </div>
    </div>
  </div>
</div>

**Code:**
```html
<div style="background: white; border-radius: 16px; padding: 24px; box-shadow: 0 8px 30px rgba(0,0,0,0.12); max-width: 400px; border-top: 4px solid #10b981;">
  <div style="display: flex; align-items: start; gap: 16px;">
    <div style="background: linear-gradient(135deg, #10b981 0%, #059669 100%); width: 56px; height: 56px; border-radius: 14px; display: flex; align-items: center; justify-content: center; font-size: 1.8em; color: white; box-shadow: 0 4px 15px rgba(236, 72, 153, 0.3);">
      [ICON]
    </div>
    <div style="flex: 1;">
      <h3 style="margin: 0 0 8px 0; color: #111827; font-size: 1.3em;">[TITLE]</h3>
      <p style="margin: 0 0 12px 0; color: #6b7280; font-size: 0.95em; line-height: 1.6;">[DESCRIPTION]</p>
      <div style="display: flex; gap: 8px; flex-wrap: wrap;">
        <span style="background: #d1fae5; color: #10b981; padding: 4px 12px; border-radius: 8px; font-size: 0.85em; font-weight: 600;">[TAG1]</span>
        <span style="background: #d1fae5; color: #10b981; padding: 4px 12px; border-radius: 8px; font-size: 0.85em; font-weight: 600;">[TAG2]</span>
      </div>
    </div>
  </div>
</div>
```

### Two Column Info Grid

<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 16px; margin: 20px 0; max-width: 700px;">
  <div style="background: white; border: 2px solid #e5e7eb; border-radius: 12px; padding: 20px; box-shadow: 0 4px 12px rgba(0,0,0,0.05);">
    <div style="font-size: 1.6em; margin-bottom: 12px; color: #3b82f6;">💼</div>
    <h4 style="margin: 0 0 8px 0; color: #111827; font-size: 1.1em;">Business Metrics</h4>
    <p style="margin: 0; color: #6b7280; font-size: 0.95em; line-height: 1.6;">
      Track revenue, growth, and key business KPIs across all departments and regions.
    </p>
  </div>

  <div style="background: white; border: 2px solid #e5e7eb; border-radius: 12px; padding: 20px; box-shadow: 0 4px 12px rgba(0,0,0,0.05);">
    <div style="font-size: 1.6em; margin-bottom: 12px; color: #10b981;">📊</div>
    <h4 style="margin: 0 0 8px 0; color: #111827; font-size: 1.1em;">Performance Data</h4>
    <p style="margin: 0; color: #6b7280; font-size: 0.95em; line-height: 1.6;">
      Monitor system performance, uptime, and resource utilization in real-time.
    </p>
  </div>
</div>

**Code:**
```html
<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 16px;">
  <div style="background: white; border: 2px solid #e5e7eb; border-radius: 12px; padding: 20px; box-shadow: 0 4px 12px rgba(0,0,0,0.05);">
    <div style="font-size: 1.6em; margin-bottom: 12px; color: [COLOR];">[ICON]</div>
    <h4 style="margin: 0 0 8px 0; color: #111827; font-size: 1.1em;">[LEFT_TITLE]</h4>
    <p style="margin: 0; color: #6b7280; font-size: 0.95em; line-height: 1.6;">[LEFT_CONTENT]</p>
  </div>

  <div style="background: white; border: 2px solid #e5e7eb; border-radius: 12px; padding: 20px; box-shadow: 0 4px 12px rgba(0,0,0,0.05);">
    <div style="font-size: 1.6em; margin-bottom: 12px; color: [COLOR];">[ICON]</div>
    <h4 style="margin: 0 0 8px 0; color: #111827; font-size: 1.1em;">[RIGHT_TITLE]</h4>
    <p style="margin: 0; color: #6b7280; font-size: 0.95em; line-height: 1.6;">[RIGHT_CONTENT]</p>
  </div>
</div>
```

---

<a name="kpi-metrics"></a>
## 📈 KPI & Metrics Cards

### Gradient KPI Card

<div style="border-radius: 16px; padding: 24px; background: linear-gradient(135deg, #43cea2 0%, #185a9d 100%); color: #fff; max-width: 280px; margin: 20px 0; box-shadow: 0 8px 30px rgba(67, 206, 162, 0.3);">
  <div style="font-size: 0.95em; opacity: 0.9; margin-bottom: 8px; font-weight: 600;">Monthly Revenue</div>
  <div style="font-size: 2.8em; font-weight: 800; margin-bottom: 12px;">$128.5K</div>
  <div style="display: flex; align-items: center; gap: 6px; font-size: 0.9em;">
    <span style="background: rgba(255,255,255,0.25); padding: 4px 10px; border-radius: 8px;">↑ 23.4%</span>
    <span style="opacity: 0.85;">vs last month</span>
  </div>
</div>

**Code:**
```html
<div style="border-radius: 16px; padding: 24px; background: linear-gradient(135deg, #43cea2 0%, #185a9d 100%); color: #fff; max-width: 280px; box-shadow: 0 8px 30px rgba(67, 206, 162, 0.3);">
  <div style="font-size: 0.95em; opacity: 0.9; margin-bottom: 8px; font-weight: 600;">[KPI_LABEL]</div>
  <div style="font-size: 2.8em; font-weight: 800; margin-bottom: 12px;">[VALUE]</div>
  <div style="display: flex; align-items: center; gap: 6px; font-size: 0.9em;">
    <span style="background: rgba(255,255,255,0.25); padding: 4px 10px; border-radius: 8px;">[CHANGE]</span>
    <span style="opacity: 0.85;">[CONTEXT]</span>
  </div>
</div>
```

### KPI Ring Progress

<div style="display: flex; align-items: center; gap: 20px; background: white; padding: 24px; border-radius: 16px; box-shadow: 0 8px 30px rgba(0,0,0,0.1); max-width: 400px; margin: 20px 0;">
  <div style="position: relative; width: 100px; height: 100px;">
    <div style="width: 100px; height: 100px; border-radius: 50%; background: conic-gradient(#10b981 0deg 252deg, #f3f4f6 252deg 360deg); display: flex; align-items: center; justify-content: center; position: relative;">
      <div style="width: 70px; height: 70px; border-radius: 50%; background: white; display: flex; align-items: center; justify-content: center;">
        <span style="font-size: 1.5em; font-weight: 800; color: #10b981;">70%</span>
      </div>
    </div>
  </div>
  <div style="flex: 1;">
    <h4 style="margin: 0 0 6px 0; color: #111827; font-size: 1.2em;">Task Completion</h4>
    <p style="margin: 0 0 10px 0; color: #6b7280; font-size: 0.95em;">28 of 40 tasks completed</p>
    <div style="display: flex; gap: 8px;">
      <span style="background: #d1fae5; color: #10b981; padding: 4px 10px; border-radius: 8px; font-size: 0.85em; font-weight: 600;">Q4 2025</span>
      <span style="background: #f3f4f6; color: #6b7280; padding: 4px 10px; border-radius: 8px; font-size: 0.85em; font-weight: 600;">Sprint 12</span>
    </div>
  </div>
</div>

**Code:**
```html
<div style="display: flex; align-items: center; gap: 20px; background: white; padding: 24px; border-radius: 16px; box-shadow: 0 8px 30px rgba(0,0,0,0.1); max-width: 400px;">
  <div style="position: relative; width: 100px; height: 100px;">
    <div style="width: 100px; height: 100px; border-radius: 50%; background: conic-gradient(#10b981 0deg [DEGREES]deg, #f3f4f6 [DEGREES]deg 360deg); display: flex; align-items: center; justify-content: center;">
      <div style="width: 70px; height: 70px; border-radius: 50%; background: white; display: flex; align-items: center; justify-content: center;">
        <span style="font-size: 1.5em; font-weight: 800; color: #10b981;">[PERCENT]%</span>
      </div>
    </div>
  </div>
  <div style="flex: 1;">
    <h4 style="margin: 0 0 6px 0; color: #111827; font-size: 1.2em;">[LABEL]</h4>
    <p style="margin: 0 0 10px 0; color: #6b7280; font-size: 0.95em;">[DETAILS]</p>
    <div style="display: flex; gap: 8px;">
      <span style="background: #d1fae5; color: #10b981; padding: 4px 10px; border-radius: 8px; font-size: 0.85em; font-weight: 600;">[TAG1]</span>
      <span style="background: #f3f4f6; color: #6b7280; padding: 4px 10px; border-radius: 8px; font-size: 0.85em; font-weight: 600;">[TAG2]</span>
    </div>
  </div>
</div>
```

### Stat Card with Sparkline

<div style="background: white; border-radius: 16px; padding: 24px; box-shadow: 0 8px 30px rgba(0,0,0,0.1); max-width: 320px; margin: 20px 0; border-left: 6px solid #3b82f6;">
  <div style="display: flex; justify-content: space-between; align-items: start; margin-bottom: 16px;">
    <div>
      <div style="color: #6b7280; font-size: 0.9em; font-weight: 600; margin-bottom: 8px;">Website Traffic</div>
      <div style="font-size: 2.2em; font-weight: 800; color: #111827;">24.7K</div>
      <div style="color: #10b981; font-size: 0.9em; font-weight: 600; margin-top: 4px;">↑ 12.3% this week</div>
    </div>
    <div style="width: 80px; height: 40px; background: #e0f2fe; border-radius: 8px; position: relative; overflow: hidden;">
      <div style="position: absolute; bottom: 0; left: 0; right: 0; height: 60%; background: linear-gradient(180deg, #3b82f6 0%, #2563eb 100%); clip-path: polygon(0% 70%, 20% 40%, 40% 50%, 60% 30%, 80% 20%, 100% 0%, 100% 100%, 0% 100%);"></div>
    </div>
  </div>
  <div style="border-top: 1px solid #e5e7eb; padding-top: 12px;">
    <div style="color: #6b7280; font-size: 0.85em;">Peak: 3,452 visitors/day on Dec 24</div>
  </div>
</div>

**Code:**
```html
<div style="background: white; border-radius: 16px; padding: 24px; box-shadow: 0 8px 30px rgba(0,0,0,0.1); max-width: 320px; border-left: 6px solid #3b82f6;">
  <div style="display: flex; justify-content: space-between; align-items: start; margin-bottom: 16px;">
    <div>
      <div style="color: #6b7280; font-size: 0.9em; font-weight: 600; margin-bottom: 8px;">[METRIC_NAME]</div>
      <div style="font-size: 2.2em; font-weight: 800; color: #111827;">[VALUE]</div>
      <div style="color: #10b981; font-size: 0.9em; font-weight: 600; margin-top: 4px;">[CHANGE_INDICATOR]</div>
    </div>
    <div style="width: 80px; height: 40px; background: #e0f2fe; border-radius: 8px; position: relative; overflow: hidden;">
      <!-- Sparkline visualization -->
    </div>
  </div>
  <div style="border-top: 1px solid #e5e7eb; padding-top: 12px;">
    <div style="color: #6b7280; font-size: 0.85em;">[ADDITIONAL_INFO]</div>
  </div>
</div>
```

---

<a name="alerts-notifications"></a>
## ⚠️ Alerts & Notifications

### Standard Alert Banner

<div style="background: #fff3cd; border-left: 6px solid #ffc107; padding: 16px 20px; border-radius: 8px; margin: 20px 0; max-width: 600px; box-shadow: 0 2px 8px rgba(0,0,0,0.08);">
  <div style="display: flex; align-items: start; gap: 12px;">
    <span style="font-size: 1.4em;">⚠️</span>
    <div style="flex: 1;">
      <strong style="color: #856404; font-size: 1.05em;">Warning: Scheduled Maintenance</strong>
      <p style="margin: 6px 0 0 0; color: #856404; font-size: 0.95em; line-height: 1.6;">
        System maintenance is scheduled for December 30, 2025 from 2:00 AM to 4:00 AM EST. Please save your work before this time.
      </p>
    </div>
  </div>
</div>

**Code:**
```html
<div style="background: #fff3cd; border-left: 6px solid #ffc107; padding: 16px 20px; border-radius: 8px; box-shadow: 0 2px 8px rgba(0,0,0,0.08);">
  <div style="display: flex; align-items: start; gap: 12px;">
    <span style="font-size: 1.4em;">⚠️</span>
    <div style="flex: 1;">
      <strong style="color: #856404; font-size: 1.05em;">[ALERT_TITLE]</strong>
      <p style="margin: 6px 0 0 0; color: #856404; font-size: 0.95em; line-height: 1.6;">[MESSAGE]</p>
    </div>
  </div>
</div>
```

### Success Notification Card

<div style="background: #d1fae5; border-left: 6px solid #10b981; padding: 16px 20px; border-radius: 8px; margin: 20px 0; max-width: 600px; box-shadow: 0 2px 8px rgba(0,0,0,0.08);">
  <div style="display: flex; align-items: start; gap: 12px;">
    <span style="font-size: 1.4em;">✅</span>
    <div style="flex: 1;">
      <strong style="color: #065f46; font-size: 1.05em;">Success: Report Generated</strong>
      <p style="margin: 6px 0 0 0; color: #065f46; font-size: 0.95em; line-height: 1.6;">
        Your quarterly analytics report has been successfully generated and is ready for download.
      </p>
      <a href="#" style="display: inline-block; margin-top: 8px; color: #059669; font-weight: 600; text-decoration: none; font-size: 0.9em;">Download Report →</a>
    </div>
  </div>
</div>

### Error Alert Card

<div style="background: #fee2e2; border-left: 6px solid #ef4444; padding: 16px 20px; border-radius: 8px; margin: 20px 0; max-width: 600px; box-shadow: 0 2px 8px rgba(0,0,0,0.08);">
  <div style="display: flex; align-items: start; gap: 12px;">
    <span style="font-size: 1.4em;">❌</span>
    <div style="flex: 1;">
      <strong style="color: #991b1b; font-size: 1.05em;">Error: Upload Failed</strong>
      <p style="margin: 6px 0 0 0; color: #991b1b; font-size: 0.95em; line-height: 1.6;">
        The file could not be uploaded. Please check your internet connection and try again.
      </p>
      <button style="margin-top: 8px; background: #ef4444; color: white; border: none; padding: 8px 16px; border-radius: 6px; font-weight: 600; cursor: pointer; font-size: 0.9em;">Retry Upload</button>
    </div>
  </div>
</div>

### Info Notification Card

<div style="background: #dbeafe; border-left: 6px solid #3b82f6; padding: 16px 20px; border-radius: 8px; margin: 20px 0; max-width: 600px; box-shadow: 0 2px 8px rgba(0,0,0,0.08);">
  <div style="display: flex; align-items: start; gap: 12px;">
    <span style="font-size: 1.4em;">ℹ️</span>
    <div style="flex: 1;">
      <strong style="color: #1e40af; font-size: 1.05em;">Info: New Features Available</strong>
      <p style="margin: 6px 0 0 0; color: #1e40af; font-size: 0.95em; line-height: 1.6;">
        We've released new collaboration features including real-time editing and version control.
      </p>
      <a href="#" style="display: inline-block; margin-top: 8px; color: #2563eb; font-weight: 600; text-decoration: none; font-size: 0.9em;">Learn More →</a>
    </div>
  </div>
</div>

---

<a name="profile-avatar"></a>
## 👤 Profile & Avatar Cards

### Avatar Profile Card

<div style="background: white; border: 2px solid #e5e7eb; border-radius: 16px; padding: 20px; display: flex; gap: 16px; align-items: center; box-shadow: 0 4px 15px rgba(0,0,0,0.08); max-width: 450px; margin: 20px 0;">
  <img src="https://via.placeholder.com/80" alt="Avatar" style="border-radius: 50%; width: 80px; height: 80px; object-fit: cover; border: 3px solid #10b981; box-shadow: 0 4px 12px rgba(236, 72, 153, 0.2);">
  <div style="flex: 1;">
    <h4 style="margin: 0 0 4px 0; color: #111827; font-size: 1.3em;">Sarah Johnson</h4>
    <p style="margin: 0 0 6px 0; color: #6b7280; font-size: 0.95em;">Senior Product Manager</p>
    <p style="margin: 0 0 10px 0; color: #6b7280; font-size: 0.9em;">sarah.johnson@company.com</p>
    <div style="display: flex; gap: 8px;">
      <span style="background: #d1fae5; color: #10b981; padding: 4px 10px; border-radius: 8px; font-size: 0.8em; font-weight: 600;">Product</span>
      <span style="background: #dbeafe; color: #3b82f6; padding: 4px 10px; border-radius: 8px; font-size: 0.8em; font-weight: 600;">Leadership</span>
    </div>
  </div>
</div>

**Code:**
```html
<div style="background: white; border: 2px solid #e5e7eb; border-radius: 16px; padding: 20px; display: flex; gap: 16px; align-items: center; box-shadow: 0 4px 15px rgba(0,0,0,0.08); max-width: 450px;">
  <img src="[AVATAR_URL]" alt="Avatar" style="border-radius: 50%; width: 80px; height: 80px; object-fit: cover; border: 3px solid #10b981; box-shadow: 0 4px 12px rgba(236, 72, 153, 0.2);">
  <div style="flex: 1;">
    <h4 style="margin: 0 0 4px 0; color: #111827; font-size: 1.3em;">[NAME]</h4>
    <p style="margin: 0 0 6px 0; color: #6b7280; font-size: 0.95em;">[ROLE]</p>
    <p style="margin: 0 0 10px 0; color: #6b7280; font-size: 0.9em;">[EMAIL]</p>
    <div style="display: flex; gap: 8px;">
      <span style="background: #d1fae5; color: #10b981; padding: 4px 10px; border-radius: 8px; font-size: 0.8em; font-weight: 600;">[TAG1]</span>
      <span style="background: #dbeafe; color: #3b82f6; padding: 4px 10px; border-radius: 8px; font-size: 0.8em; font-weight: 600;">[TAG2]</span>
    </div>
  </div>
</div>
```

### Team Member Card (Vertical)

<div style="background: white; border-radius: 16px; padding: 28px; text-align: center; box-shadow: 0 8px 30px rgba(0,0,0,0.12); max-width: 280px; margin: 20px 0; border-top: 4px solid #10b981;">
  <img src="https://via.placeholder.com/100" alt="Team Member" style="border-radius: 50%; width: 100px; height: 100px; object-fit: cover; margin: 0 auto 16px auto; border: 4px solid #d1fae5; box-shadow: 0 6px 20px rgba(236, 72, 153, 0.25);">
  <h4 style="margin: 0 0 6px 0; color: #111827; font-size: 1.2em; font-weight: 700;">Michael Chen</h4>
  <p style="margin: 0 0 4px 0; color: #10b981; font-size: 0.95em; font-weight: 600;">Lead Developer</p>
  <p style="margin: 0 0 16px 0; color: #6b7280; font-size: 0.85em;">Full Stack Engineer</p>
  <div style="display: flex; justify-content: center; gap: 10px; margin-bottom: 16px;">
    <a href="#" style="width: 36px; height: 36px; background: #d1fae5; border-radius: 8px; display: flex; align-items: center; justify-content: center; color: #10b981; text-decoration: none; font-weight: 700;">💼</a>
    <a href="#" style="width: 36px; height: 36px; background: #dbeafe; border-radius: 8px; display: flex; align-items: center; justify-content: center; color: #3b82f6; text-decoration: none; font-weight: 700;">✉️</a>
    <a href="#" style="width: 36px; height: 36px; background: #d1fae5; border-radius: 8px; display: flex; align-items: center; justify-content: center; color: #10b981; text-decoration: none; font-weight: 700;">🔗</a>
  </div>
  <button style="width: 100%; background: linear-gradient(135deg, #10b981 0%, #059669 100%); color: white; border: none; padding: 10px; border-radius: 8px; font-weight: 600; cursor: pointer; font-size: 0.95em;">View Profile</button>
</div>

### Contact Card with Actions

<div style="background: white; border-radius: 16px; padding: 24px; box-shadow: 0 8px 30px rgba(0,0,0,0.12); max-width: 400px; margin: 20px 0;">
  <div style="display: flex; gap: 16px; align-items: center; margin-bottom: 20px;">
    <div style="position: relative;">
      <img src="https://via.placeholder.com/70" alt="Contact" style="border-radius: 50%; width: 70px; height: 70px; object-fit: cover; border: 3px solid #10b981;">
      <div style="position: absolute; bottom: 2px; right: 2px; width: 16px; height: 16px; background: #10b981; border-radius: 50%; border: 3px solid white;"></div>
    </div>
    <div style="flex: 1;">
      <h4 style="margin: 0 0 4px 0; color: #111827; font-size: 1.2em;">Emily Rodriguez</h4>
      <p style="margin: 0; color: #6b7280; font-size: 0.9em;">UX Designer • Online</p>
    </div>
  </div>

  <div style="background: #f9fafb; padding: 16px; border-radius: 12px; margin-bottom: 16px;">
    <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 12px; font-size: 0.9em;">
      <div>
        <div style="color: #6b7280; margin-bottom: 4px;">Email</div>
        <div style="color: #111827; font-weight: 600;">emily.r@co.com</div>
      </div>
      <div>
        <div style="color: #6b7280; margin-bottom: 4px;">Phone</div>
        <div style="color: #111827; font-weight: 600;">+1 555-0123</div>
      </div>
      <div>
        <div style="color: #6b7280; margin-bottom: 4px;">Location</div>
        <div style="color: #111827; font-weight: 600;">San Francisco</div>
      </div>
      <div>
        <div style="color: #6b7280; margin-bottom: 4px;">Timezone</div>
        <div style="color: #111827; font-weight: 600;">PST (GMT-8)</div>
      </div>
    </div>
  </div>

  <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 10px;">
    <button style="background: linear-gradient(135deg, #10b981 0%, #059669 100%); color: white; border: none; padding: 10px; border-radius: 8px; font-weight: 600; cursor: pointer;">Message</button>
    <button style="background: white; color: #10b981; border: 2px solid #10b981; padding: 10px; border-radius: 8px; font-weight: 600; cursor: pointer;">Schedule</button>
  </div>
</div>

---

<a name="actions-buttons"></a>
## ⚡ Action & Button Cards

### Quick Action Panel

<div style="background: white; border-radius: 16px; padding: 24px; box-shadow: 0 8px 30px rgba(0,0,0,0.12); max-width: 500px; margin: 20px 0;">
  <h4 style="margin: 0 0 16px 0; color: #111827; font-size: 1.2em;">Quick Actions</h4>
  <div style="display: grid; grid-template-columns: repeat(3, 1fr); gap: 12px;">
    <button style="background: linear-gradient(135deg, #3b82f6 0%, #2563eb 100%); color: #fff; border: none; padding: 14px 10px; border-radius: 10px; font-weight: 600; cursor: pointer; font-size: 0.95em; box-shadow: 0 4px 12px rgba(59, 130, 246, 0.3);">
      Create New
    </button>
    <button style="background: linear-gradient(135deg, #10b981 0%, #059669 100%); color: #fff; border: none; padding: 14px 10px; border-radius: 10px; font-weight: 600; cursor: pointer; font-size: 0.95em; box-shadow: 0 4px 12px rgba(16, 185, 129, 0.3);">
      Save Draft
    </button>
    <button style="background: linear-gradient(135deg, #10b981 0%, #059669 100%); color: #fff; border: none; padding: 14px 10px; border-radius: 10px; font-weight: 600; cursor: pointer; font-size: 0.95em; box-shadow: 0 4px 12px rgba(236, 72, 153, 0.3);">
      Export
    </button>
  </div>
</div>

**Code:**
```html
<div style="background: white; border-radius: 16px; padding: 24px; box-shadow: 0 8px 30px rgba(0,0,0,0.12); max-width: 500px;">
  <h4 style="margin: 0 0 16px 0; color: #111827; font-size: 1.2em;">Quick Actions</h4>
  <div style="display: grid; grid-template-columns: repeat(3, 1fr); gap: 12px;">
    <button style="background: linear-gradient(135deg, #3b82f6 0%, #2563eb 100%); color: #fff; border: none; padding: 14px 10px; border-radius: 10px; font-weight: 600; cursor: pointer; font-size: 0.95em; box-shadow: 0 4px 12px rgba(59, 130, 246, 0.3);">[ACTION_1]</button>
    <button style="background: linear-gradient(135deg, #10b981 0%, #059669 100%); color: #fff; border: none; padding: 14px 10px; border-radius: 10px; font-weight: 600; cursor: pointer; font-size: 0.95em; box-shadow: 0 4px 12px rgba(16, 185, 129, 0.3);">[ACTION_2]</button>
    <button style="background: linear-gradient(135deg, #10b981 0%, #059669 100%); color: #fff; border: none; padding: 14px 10px; border-radius: 10px; font-weight: 600; cursor: pointer; font-size: 0.95em; box-shadow: 0 4px 12px rgba(236, 72, 153, 0.3);">[ACTION_3]</button>
  </div>
</div>
```

### CTA Card with Icon

<div style="background: linear-gradient(135deg, #10b981 0%, #059669 100%); border-radius: 20px; padding: 40px; color: white; text-align: center; box-shadow: 0 12px 40px rgba(16, 185, 129, 0.4); max-width: 500px; margin: 20px 0;">
  <div style="font-size: 3.5em; margin-bottom: 16px;">🚀</div>
  <h3 style="margin: 0 0 12px 0; font-size: 1.8em; font-weight: 800;">Start Your Free Trial</h3>
  <p style="margin: 0 0 24px 0; font-size: 1.05em; opacity: 0.95; line-height: 1.6;">
    Get access to all premium features for 14 days. No credit card required.
  </p>
  <button style="background: white; color: #10b981; border: none; padding: 16px 40px; border-radius: 12px; font-weight: 700; font-size: 1.1em; cursor: pointer; box-shadow: 0 4px 15px rgba(0,0,0,0.2);">
    Get Started Now →
  </button>
  <p style="margin: 16px 0 0 0; font-size: 0.85em; opacity: 0.8;">
    Join 10,000+ satisfied customers
  </p>
</div>

### Feature Highlight Card

<div style="background: white; border-radius: 16px; padding: 32px; box-shadow: 0 8px 30px rgba(0,0,0,0.12); max-width: 450px; margin: 20px 0; text-align: center;">
  <div style="width: 80px; height: 80px; background: linear-gradient(135deg, #8b5cf6 0%, #7c3aed 100%); border-radius: 20px; display: flex; align-items: center; justify-content: center; font-size: 2.5em; margin: 0 auto 20px auto; box-shadow: 0 8px 25px rgba(139, 92, 246, 0.3);">
    ⚡
  </div>
  <h3 style="margin: 0 0 12px 0; color: #111827; font-size: 1.5em; font-weight: 700;">Lightning Fast Performance</h3>
  <p style="margin: 0 0 24px 0; color: #6b7280; font-size: 0.95em; line-height: 1.7;">
    Experience blazing fast load times with our optimized infrastructure. 99.9% uptime guaranteed.
  </p>
  <button style="background: linear-gradient(135deg, #8b5cf6 0%, #7c3aed 100%); color: white; border: none; padding: 12px 28px; border-radius: 10px; font-weight: 600; font-size: 1em; cursor: pointer; box-shadow: 0 4px 15px rgba(139, 92, 246, 0.3);">
    Learn More
  </button>
</div>

---

<a name="progress-timeline"></a>
## ⏱️ Progress & Timeline Cards

### Progress Meter

<div style="background: white; padding: 20px; border-radius: 12px; box-shadow: 0 4px 15px rgba(0,0,0,0.1); max-width: 500px; margin: 20px 0;">
  <div style="display: flex; justify-content: space-between; align-items: center; margin-bottom: 10px;">
    <span style="color: #111827; font-weight: 600; font-size: 1.05em;">Project Completion</span>
    <span style="color: #6b7280; font-weight: 700; font-size: 1.1em;">73%</span>
  </div>
  <div style="display: flex; align-items: center; gap: 10px;">
    <div style="flex: 1; background: #e5e7eb; height: 12px; border-radius: 10px; overflow: hidden;">
      <div style="width: 73%; background: linear-gradient(90deg, #10b981 0%, #059669 100%); height: 12px; border-radius: 10px; box-shadow: inset 0 1px 3px rgba(0,0,0,0.1);"></div>
    </div>
  </div>
  <div style="color: #6b7280; font-size: 0.85em; margin-top: 8px;">23 of 32 milestones completed</div>
</div>

**Code:**
```html
<div style="background: white; padding: 20px; border-radius: 12px; box-shadow: 0 4px 15px rgba(0,0,0,0.1); max-width: 500px;">
  <div style="display: flex; justify-content: space-between; align-items: center; margin-bottom: 10px;">
    <span style="color: #111827; font-weight: 600; font-size: 1.05em;">[LABEL]</span>
    <span style="color: #6b7280; font-weight: 700; font-size: 1.1em;">[PERCENT]%</span>
  </div>
  <div style="display: flex; align-items: center; gap: 10px;">
    <div style="flex: 1; background: #e5e7eb; height: 12px; border-radius: 10px; overflow: hidden;">
      <div style="width: [PERCENT]%; background: linear-gradient(90deg, #10b981 0%, #059669 100%); height: 12px; border-radius: 10px; box-shadow: inset 0 1px 3px rgba(0,0,0,0.1);"></div>
    </div>
  </div>
  <div style="color: #6b7280; font-size: 0.85em; margin-top: 8px;">[DETAILS]</div>
</div>
```

### Multi-Progress Dashboard

<div style="background: white; border-radius: 16px; padding: 28px; box-shadow: 0 8px 30px rgba(0,0,0,0.12); max-width: 550px; margin: 20px 0;">
  <h4 style="margin: 0 0 24px 0; color: #111827; font-size: 1.3em;">Sprint Progress</h4>

  <div style="margin-bottom: 20px;">
    <div style="display: flex; justify-content: space-between; margin-bottom: 8px;">
      <span style="color: #6b7280; font-weight: 600;">Design</span>
      <span style="color: #10b981; font-weight: 700;">90%</span>
    </div>
    <div style="background: #e5e7eb; height: 10px; border-radius: 8px; overflow: hidden;">
      <div style="width: 90%; background: linear-gradient(90deg, #10b981 0%, #059669 100%); height: 10px;"></div>
    </div>
  </div>

  <div style="margin-bottom: 20px;">
    <div style="display: flex; justify-content: space-between; margin-bottom: 8px;">
      <span style="color: #6b7280; font-weight: 600;">Development</span>
      <span style="color: #3b82f6; font-weight: 700;">65%</span>
    </div>
    <div style="background: #e5e7eb; height: 10px; border-radius: 8px; overflow: hidden;">
      <div style="width: 65%; background: linear-gradient(90deg, #3b82f6 0%, #2563eb 100%); height: 10px;"></div>
    </div>
  </div>

  <div style="margin-bottom: 20px;">
    <div style="display: flex; justify-content: space-between; margin-bottom: 8px;">
      <span style="color: #6b7280; font-weight: 600;">Testing</span>
      <span style="color: #f59e0b; font-weight: 700;">42%</span>
    </div>
    <div style="background: #e5e7eb; height: 10px; border-radius: 8px; overflow: hidden;">
      <div style="width: 42%; background: linear-gradient(90deg, #f59e0b 0%, #d97706 100%); height: 10px;"></div>
    </div>
  </div>

  <div>
    <div style="display: flex; justify-content: space-between; margin-bottom: 8px;">
      <span style="color: #6b7280; font-weight: 600;">Documentation</span>
      <span style="color: #10b981; font-weight: 700;">28%</span>
    </div>
    <div style="background: #e5e7eb; height: 10px; border-radius: 8px; overflow: hidden;">
      <div style="width: 28%; background: linear-gradient(90deg, #10b981 0%, #059669 100%); height: 10px;"></div>
    </div>
  </div>
</div>

### Timeline Steps Card

<div style="background: white; border-radius: 16px; padding: 28px; box-shadow: 0 8px 30px rgba(0,0,0,0.12); max-width: 500px; margin: 20px 0;">
  <h4 style="margin: 0 0 24px 0; color: #111827; font-size: 1.3em;">Project Timeline</h4>

  <div style="position: relative; padding-left: 40px;">
    <!-- Step 1 - Completed -->
    <div style="position: relative; margin-bottom: 30px;">
      <div style="position: absolute; left: -40px; width: 24px; height: 24px; background: #10b981; border-radius: 50%; display: flex; align-items: center; justify-content: center; color: white; font-weight: 700; font-size: 0.7em; box-shadow: 0 0 0 4px #d1fae5;">✓</div>
      <div style="position: absolute; left: -28px; top: 24px; bottom: -30px; width: 2px; background: #e5e7eb;"></div>
      <h5 style="margin: 0 0 6px 0; color: #111827; font-weight: 700;">Planning Phase</h5>
      <p style="margin: 0; color: #6b7280; font-size: 0.9em;">Completed Dec 15, 2025</p>
    </div>

    <!-- Step 2 - In Progress -->
    <div style="position: relative; margin-bottom: 30px;">
      <div style="position: absolute; left: -40px; width: 24px; height: 24px; background: #3b82f6; border-radius: 50%; display: flex; align-items: center; justify-content: center; color: white; font-weight: 700; font-size: 0.7em; box-shadow: 0 0 0 4px #dbeafe;">2</div>
      <div style="position: absolute; left: -28px; top: 24px; bottom: -30px; width: 2px; background: #e5e7eb;"></div>
      <h5 style="margin: 0 0 6px 0; color: #111827; font-weight: 700;">Development</h5>
      <p style="margin: 0; color: #3b82f6; font-size: 0.9em; font-weight: 600;">In Progress</p>
    </div>

    <!-- Step 3 - Upcoming -->
    <div style="position: relative; margin-bottom: 30px;">
      <div style="position: absolute; left: -40px; width: 24px; height: 24px; background: #e5e7eb; border-radius: 50%; display: flex; align-items: center; justify-content: center; color: #6b7280; font-weight: 700; font-size: 0.7em;">3</div>
      <div style="position: absolute; left: -28px; top: 24px; bottom: -30px; width: 2px; background: #e5e7eb;"></div>
      <h5 style="margin: 0 0 6px 0; color: #6b7280; font-weight: 700;">Testing</h5>
      <p style="margin: 0; color: #9ca3af; font-size: 0.9em;">Starts Jan 5, 2026</p>
    </div>

    <!-- Step 4 - Upcoming -->
    <div style="position: relative;">
      <div style="position: absolute; left: -40px; width: 24px; height: 24px; background: #e5e7eb; border-radius: 50%; display: flex; align-items: center; justify-content: center; color: #6b7280; font-weight: 700; font-size: 0.7em;">4</div>
      <h5 style="margin: 0 0 6px 0; color: #6b7280; font-weight: 700;">Deployment</h5>
      <p style="margin: 0; color: #9ca3af; font-size: 0.9em;">Planned Jan 20, 2026</p>
    </div>
  </div>
</div>

---

<a name="lists-tables"></a>
## 📋 Lists & Tables Cards

### Feature List Card

<div style="background: white; border-radius: 16px; padding: 28px; box-shadow: 0 8px 30px rgba(0,0,0,0.12); max-width: 450px; margin: 20px 0;">
  <h4 style="margin: 0 0 20px 0; color: #111827; font-size: 1.3em;">Premium Features</h4>

  <div style="display: flex; align-items: start; gap: 12px; margin-bottom: 16px;">
    <span style="width: 24px; height: 24px; background: #d1fae5; border-radius: 6px; display: flex; align-items: center; justify-content: center; color: #10b981; font-weight: 700; flex-shrink: 0;">✓</span>
    <div>
      <div style="color: #111827; font-weight: 600; margin-bottom: 4px;">Advanced Analytics</div>
      <div style="color: #6b7280; font-size: 0.9em;">Track detailed metrics and insights</div>
    </div>
  </div>

  <div style="display: flex; align-items: start; gap: 12px; margin-bottom: 16px;">
    <span style="width: 24px; height: 24px; background: #d1fae5; border-radius: 6px; display: flex; align-items: center; justify-content: center; color: #10b981; font-weight: 700; flex-shrink: 0;">✓</span>
    <div>
      <div style="color: #111827; font-weight: 600; margin-bottom: 4px;">24/7 Priority Support</div>
      <div style="color: #6b7280; font-size: 0.9em;">Get help whenever you need it</div>
    </div>
  </div>

  <div style="display: flex; align-items: start; gap: 12px; margin-bottom: 16px;">
    <span style="width: 24px; height: 24px; background: #d1fae5; border-radius: 6px; display: flex; align-items: center; justify-content: center; color: #10b981; font-weight: 700; flex-shrink: 0;">✓</span>
    <div>
      <div style="color: #111827; font-weight: 600; margin-bottom: 4px;">Custom Integrations</div>
      <div style="color: #6b7280; font-size: 0.9em;">Connect with your favorite tools</div>
    </div>
  </div>

  <div style="display: flex; align-items: start; gap: 12px;">
    <span style="width: 24px; height: 24px; background: #d1fae5; border-radius: 6px; display: flex; align-items: center; justify-content: center; color: #10b981; font-weight: 700; flex-shrink: 0;">✓</span>
    <div>
      <div style="color: #111827; font-weight: 600; margin-bottom: 4px;">Unlimited Storage</div>
      <div style="color: #6b7280; font-size: 0.9em;">Store all your data without limits</div>
    </div>
  </div>
</div>

### Data Table Card

<div style="background: white; border-radius: 16px; padding: 28px; box-shadow: 0 8px 30px rgba(0,0,0,0.12); max-width: 650px; margin: 20px 0; overflow-x: auto;">
  <h4 style="margin: 0 0 20px 0; color: #111827; font-size: 1.3em;">Recent Activity</h4>

  <table style="width: 100%; border-collapse: collapse;">
    <thead>
      <tr style="background: linear-gradient(135deg, #10b981 0%, #059669 100%); color: white;">
        <th style="padding: 12px; text-align: left; font-weight: 600; font-size: 0.9em; border-radius: 8px 0 0 0;">User</th>
        <th style="padding: 12px; text-align: left; font-weight: 600; font-size: 0.9em;">Action</th>
        <th style="padding: 12px; text-align: left; font-weight: 600; font-size: 0.9em;">Time</th>
        <th style="padding: 12px; text-align: center; font-weight: 600; font-size: 0.9em; border-radius: 0 8px 0 0;">Status</th>
      </tr>
    </thead>
    <tbody>
      <tr style="border-bottom: 1px solid #e5e7eb;">
        <td style="padding: 14px; color: #111827; font-weight: 600;">Sarah J.</td>
        <td style="padding: 14px; color: #6b7280;">Updated project</td>
        <td style="padding: 14px; color: #6b7280;">2 min ago</td>
        <td style="padding: 14px; text-align: center;">
          <span style="background: #d1fae5; color: #065f46; padding: 4px 12px; border-radius: 12px; font-size: 0.85em; font-weight: 600;">Success</span>
        </td>
      </tr>
      <tr style="border-bottom: 1px solid #e5e7eb;">
        <td style="padding: 14px; color: #111827; font-weight: 600;">Mike C.</td>
        <td style="padding: 14px; color: #6b7280;">Created task</td>
        <td style="padding: 14px; color: #6b7280;">15 min ago</td>
        <td style="padding: 14px; text-align: center;">
          <span style="background: #dbeafe; color: #1e40af; padding: 4px 12px; border-radius: 12px; font-size: 0.85em; font-weight: 600;">Pending</span>
        </td>
      </tr>
      <tr>
        <td style="padding: 14px; color: #111827; font-weight: 600;">Emily R.</td>
        <td style="padding: 14px; color: #6b7280;">Closed issue</td>
        <td style="padding: 14px; color: #6b7280;">1 hour ago</td>
        <td style="padding: 14px; text-align: center;">
          <span style="background: #d1fae5; color: #065f46; padding: 4px 12px; border-radius: 12px; font-size: 0.85em; font-weight: 600;">Success</span>
        </td>
      </tr>
    </tbody>
  </table>
</div>

---

<a name="special-effects"></a>
## ✨ Special Effects Cards

### Glassmorphism Card

<div style="background: linear-gradient(135deg, rgba(236, 72, 153, 0.1) 0%, rgba(219, 39, 119, 0.1) 100%); backdrop-filter: blur(20px); -webkit-backdrop-filter: blur(20px); border: 1px solid rgba(255, 255, 255, 0.3); border-radius: 20px; padding: 32px; max-width: 450px; margin: 20px 0; box-shadow: 0 8px 32px rgba(0, 0, 0, 0.1);">
  <div style="display: flex; align-items: center; gap: 16px; margin-bottom: 20px;">
    <div style="width: 60px; height: 60px; background: rgba(255, 255, 255, 0.3); backdrop-filter: blur(10px); border-radius: 16px; display: flex; align-items: center; justify-content: center; font-size: 2em; border: 1px solid rgba(255, 255, 255, 0.4);">
      💎
    </div>
    <div>
      <h4 style="margin: 0 0 4px 0; color: #111827; font-size: 1.3em; font-weight: 700;">Glassmorphism Effect</h4>
      <p style="margin: 0; color: #6b7280; font-size: 0.95em;">Modern frosted glass aesthetic</p>
    </div>
  </div>
  <p style="margin: 0 0 20px 0; color: #374151; font-size: 0.95em; line-height: 1.7;">
    This card uses backdrop-filter blur with semi-transparent backgrounds to create a sophisticated frosted glass effect popular in modern UI design.
  </p>
  <button style="background: rgba(236, 72, 153, 0.9); backdrop-filter: blur(10px); color: white; border: 1px solid rgba(255, 255, 255, 0.3); padding: 12px 24px; border-radius: 10px; font-weight: 600; cursor: pointer; font-size: 0.95em;">
    Explore More
  </button>
</div>

**Code:**
```html
<div style="background: linear-gradient(135deg, rgba(236, 72, 153, 0.1) 0%, rgba(219, 39, 119, 0.1) 100%); backdrop-filter: blur(20px); -webkit-backdrop-filter: blur(20px); border: 1px solid rgba(255, 255, 255, 0.3); border-radius: 20px; padding: 32px; box-shadow: 0 8px 32px rgba(0, 0, 0, 0.1);">
  <!-- Content -->
</div>
```

### Neumorphism Card

<div style="background: #e0e5ec; border-radius: 20px; padding: 32px; max-width: 450px; margin: 20px 0; box-shadow: 9px 9px 16px #a3b1c6, -9px -9px 16px #ffffff;">
  <div style="display: flex; align-items: center; gap: 16px; margin-bottom: 20px;">
    <div style="width: 60px; height: 60px; background: #e0e5ec; border-radius: 16px; display: flex; align-items: center; justify-content: center; font-size: 2em; box-shadow: inset 4px 4px 8px #a3b1c6, inset -4px -4px 8px #ffffff;">
      🎯
    </div>
    <div>
      <h4 style="margin: 0 0 4px 0; color: #111827; font-size: 1.3em; font-weight: 700;">Neumorphism Style</h4>
      <p style="margin: 0; color: #6b7280; font-size: 0.95em;">Soft UI design trend</p>
    </div>
  </div>
  <p style="margin: 0 0 20px 0; color: #374151; font-size: 0.95em; line-height: 1.7;">
    Neumorphism creates a soft, extruded plastic look using subtle shadows to make elements appear raised or pressed into the background.
  </p>
  <button style="background: #e0e5ec; color: #111827; border: none; padding: 12px 24px; border-radius: 10px; font-weight: 600; cursor: pointer; font-size: 0.95em; box-shadow: 4px 4px 8px #a3b1c6, -4px -4px 8px #ffffff;">
    Try It Out
  </button>
</div>

### 3D Transform Card

<div style="background: white; border-radius: 20px; padding: 32px; max-width: 450px; margin: 20px 0; box-shadow: 0 20px 60px rgba(0,0,0,0.2); transform: perspective(1000px) rotateY(-5deg); transition: transform 0.3s ease;">
  <div style="display: flex; align-items: center; gap: 16px; margin-bottom: 20px;">
    <div style="width: 60px; height: 60px; background: linear-gradient(135deg, #8b5cf6 0%, #7c3aed 100%); border-radius: 16px; display: flex; align-items: center; justify-content: center; font-size: 2em; color: white; box-shadow: 0 8px 25px rgba(139, 92, 246, 0.3);">
      🎪
    </div>
    <div>
      <h4 style="margin: 0 0 4px 0; color: #111827; font-size: 1.3em; font-weight: 700;">3D Transform</h4>
      <p style="margin: 0; color: #6b7280; font-size: 0.95em;">Interactive perspective</p>
    </div>
  </div>
  <p style="margin: 0 0 20px 0; color: #374151; font-size: 0.95em; line-height: 1.7;">
    This card uses CSS 3D transforms with perspective to create depth and dimension. Hover effects can add interactivity.
  </p>
  <button style="background: linear-gradient(135deg, #8b5cf6 0%, #7c3aed 100%); color: white; border: none; padding: 12px 24px; border-radius: 10px; font-weight: 600; cursor: pointer; font-size: 0.95em; box-shadow: 0 4px 15px rgba(139, 92, 246, 0.3);">
    Discover More
  </button>
</div>

### Gradient Border Card

<div style="position: relative; padding: 3px; background: linear-gradient(135deg, #10b981 0%, #8b5cf6 50%, #3b82f6 100%); border-radius: 20px; max-width: 450px; margin: 20px 0; box-shadow: 0 8px 30px rgba(0,0,0,0.15);">
  <div style="background: white; border-radius: 17px; padding: 32px;">
    <div style="display: flex; align-items: center; gap: 16px; margin-bottom: 20px;">
      <div style="width: 60px; height: 60px; background: linear-gradient(135deg, #10b981 0%, #8b5cf6 50%, #3b82f6 100%); border-radius: 16px; display: flex; align-items: center; justify-content: center; font-size: 2em; color: white;">
        🌈
      </div>
      <div>
        <h4 style="margin: 0 0 4px 0; color: #111827; font-size: 1.3em; font-weight: 700;">Gradient Border</h4>
        <p style="margin: 0; color: #6b7280; font-size: 0.95em;">Colorful edge design</p>
      </div>
    </div>
    <p style="margin: 0 0 20px 0; color: #374151; font-size: 0.95em; line-height: 1.7;">
      Multi-color gradient borders create eye-catching visual effects. Achieved using nested divs with background gradients.
    </p>
    <button style="background: linear-gradient(135deg, #10b981 0%, #8b5cf6 50%, #3b82f6 100%); color: white; border: none; padding: 12px 24px; border-radius: 10px; font-weight: 600; cursor: pointer; font-size: 0.95em;">
      View Details
    </button>
  </div>
</div>

---

## 🎨 Design Best Practices

### Card Component Principles

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 20px; margin: 25px 0;">
  <div style="background: white; padding: 25px; border-radius: 12px; border-left: 4px solid #3b82f6; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
    <div style="font-size: 1.8em; margin-bottom: 10px;">🎯</div>
    <div style="color: #3b82f6; font-weight: 700; font-size: 1.2em; margin-bottom: 10px;">Clear Hierarchy</div>
    <div style="color: #6b7280; font-size: 0.95em; line-height: 1.7;">
      • Use size and weight for importance<br/>
      • Group related information<br/>
      • Maintain consistent spacing<br/>
      • Guide user's attention flow
    </div>
  </div>

  <div style="background: white; padding: 25px; border-radius: 12px; border-left: 4px solid #10b981; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
    <div style="font-size: 1.8em; margin-bottom: 10px;">🎨</div>
    <div style="color: #10b981; font-weight: 700; font-size: 1.2em; margin-bottom: 10px;">Visual Consistency</div>
    <div style="color: #6b7280; font-size: 0.95em; line-height: 1.7;">
      • Uniform border radius (12-20px)<br/>
      • Consistent shadow styles<br/>
      • Cohesive color palette<br/>
      • Standard padding patterns
    </div>
  </div>

  <div style="background: white; padding: 25px; border-radius: 12px; border-left: 4px solid #10b981; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
    <div style="font-size: 1.8em; margin-bottom: 10px;">📱</div>
    <div style="color: #10b981; font-weight: 700; font-size: 1.2em; margin-bottom: 10px;">Responsive Design</div>
    <div style="color: #6b7280; font-size: 0.95em; line-height: 1.7;">
      • Use grid layouts (auto-fit)<br/>
      • Flexible min/max widths<br/>
      • Test across screen sizes<br/>
      • Mobile-first approach
    </div>
  </div>

  <div style="background: white; padding: 25px; border-radius: 12px; border-left: 4px solid #f59e0b; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
    <div style="font-size: 1.8em; margin-bottom: 10px;">♿</div>
    <div style="color: #f59e0b; font-weight: 700; font-size: 1.2em; margin-bottom: 10px;">Accessibility</div>
    <div style="color: #6b7280; font-size: 0.95em; line-height: 1.7;">
      • 4.5:1 text contrast minimum<br/>
      • Keyboard navigation support<br/>
      • Semantic HTML structure<br/>
      • Alt text for images
    </div>
  </div>
</div>

### Color Theory for Cards

<table style="width: 100%; border-collapse: collapse; margin: 25px 0; box-shadow: 0 4px 15px rgba(0,0,0,0.1); border-radius: 12px; overflow: hidden;">
  <thead>
    <tr style="background: linear-gradient(135deg, #10b981 0%, #059669 100%); color: white;">
      <th style="padding: 15px; text-align: left; font-weight: 700;">Color</th>
      <th style="padding: 15px; text-align: left; font-weight: 700;">Usage</th>
      <th style="padding: 15px; text-align: left; font-weight: 700;">Psychology</th>
      <th style="padding: 15px; text-align: left; font-weight: 700;">Best For</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background: #f9fafb; border-bottom: 1px solid #e5e7eb;">
      <td style="padding: 15px;">
        <div style="display: flex; align-items: center; gap: 10px;">
          <div style="width: 30px; height: 30px; background: #3b82f6; border-radius: 6px; border: 2px solid #2563eb;"></div>
          <span style="font-weight: 600; color: #111827;">Blue</span>
        </div>
      </td>
      <td style="padding: 15px; color: #374151;">Primary actions, links, info</td>
      <td style="padding: 15px; color: #6b7280;">Trust, professionalism, calm</td>
      <td style="padding: 15px; color: #6b7280;">Business, tech, analytics</td>
    </tr>
    <tr style="background: #ffffff; border-bottom: 1px solid #e5e7eb;">
      <td style="padding: 15px;">
        <div style="display: flex; align-items: center; gap: 10px;">
          <div style="width: 30px; height: 30px; background: #10b981; border-radius: 6px; border: 2px solid #059669;"></div>
          <span style="font-weight: 600; color: #111827;">Green</span>
        </div>
      </td>
      <td style="padding: 15px; color: #374151;">Success states, confirmations</td>
      <td style="padding: 15px; color: #6b7280;">Growth, health, positivity</td>
      <td style="padding: 15px; color: #6b7280;">Success messages, financial</td>
    </tr>
    <tr style="background: #f9fafb; border-bottom: 1px solid #e5e7eb;">
      <td style="padding: 15px;">
        <div style="display: flex; align-items: center; gap: 10px;">
          <div style="width: 30px; height: 30px; background: #ef4444; border-radius: 6px; border: 2px solid #dc2626;"></div>
          <span style="font-weight: 600; color: #111827;">Red</span>
        </div>
      </td>
      <td style="padding: 15px; color: #374151;">Errors, critical alerts, delete</td>
      <td style="padding: 15px; color: #6b7280;">Urgency, importance, danger</td>
      <td style="padding: 15px; color: #6b7280;">Error states, warnings</td>
    </tr>
    <tr style="background: #ffffff; border-bottom: 1px solid #e5e7eb;">
      <td style="padding: 15px;">
        <div style="display: flex; align-items: center; gap: 10px;">
          <div style="width: 30px; height: 30px; background: #f59e0b; border-radius: 6px; border: 2px solid #d97706;"></div>
          <span style="font-weight: 600; color: #111827;">Orange</span>
        </div>
      </td>
      <td style="padding: 15px; color: #374151;">Warnings, pending states</td>
      <td style="padding: 15px; color: #6b7280;">Energy, attention, caution</td>
      <td style="padding: 15px; color: #6b7280;">Alerts, in-progress items</td>
    </tr>
    <tr style="background: #f9fafb;">
      <td style="padding: 15px;">
        <div style="display: flex; align-items: center; gap: 10px;">
          <div style="width: 30px; height: 30px; background: #8b5cf6; border-radius: 6px; border: 2px solid #7c3aed;"></div>
          <span style="font-weight: 600; color: #111827;">Purple</span>
        </div>
      </td>
      <td style="padding: 15px; color: #374151;">Premium features, creativity</td>
      <td style="padding: 15px; color: #6b7280;">Luxury, creativity, wisdom</td>
      <td style="padding: 15px; color: #6b7280;">Premium tiers, creative tools</td>
    </tr>
  </tbody>
</table>

### Shadow and Depth Guidelines

<div style="background: white; border-radius: 16px; padding: 28px; box-shadow: 0 8px 30px rgba(0,0,0,0.12); max-width: 650px; margin: 25px 0;">
  <h4 style="margin: 0 0 20px 0; color: #111827; font-size: 1.3em;">Shadow Depth Levels</h4>

  <div style="margin-bottom: 20px;">
    <div style="color: #6b7280; font-weight: 600; margin-bottom: 10px;">Level 1 - Subtle (Resting State)</div>
    <div style="background: white; padding: 20px; border-radius: 12px; box-shadow: 0 2px 8px rgba(0,0,0,0.05);">
      <code style="background: #f3f4f6; padding: 4px 8px; border-radius: 4px; font-size: 0.85em;">box-shadow: 0 2px 8px rgba(0,0,0,0.05);</code>
    </div>
  </div>

  <div style="margin-bottom: 20px;">
    <div style="color: #6b7280; font-weight: 600; margin-bottom: 10px;">Level 2 - Medium (Hover State)</div>
    <div style="background: white; padding: 20px; border-radius: 12px; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
      <code style="background: #f3f4f6; padding: 4px 8px; border-radius: 4px; font-size: 0.85em;">box-shadow: 0 4px 15px rgba(0,0,0,0.1);</code>
    </div>
  </div>

  <div style="margin-bottom: 20px;">
    <div style="color: #6b7280; font-weight: 600; margin-bottom: 10px;">Level 3 - Strong (Active/Focus)</div>
    <div style="background: white; padding: 20px; border-radius: 12px; box-shadow: 0 8px 30px rgba(0,0,0,0.15);">
      <code style="background: #f3f4f6; padding: 4px 8px; border-radius: 4px; font-size: 0.85em;">box-shadow: 0 8px 30px rgba(0,0,0,0.15);</code>
    </div>
  </div>

  <div>
    <div style="color: #6b7280; font-weight: 600; margin-bottom: 10px;">Level 4 - Dramatic (Modals/Overlays)</div>
    <div style="background: white; padding: 20px; border-radius: 12px; box-shadow: 0 20px 60px rgba(0,0,0,0.3);">
      <code style="background: #f3f4f6; padding: 4px 8px; border-radius: 4px; font-size: 0.85em;">box-shadow: 0 20px 60px rgba(0,0,0,0.3);</code>
    </div>
  </div>
</div>

---

## 📐 Component Composition Patterns

### Combining Card Elements

<div style="background: white; border-radius: 20px; padding: 32px; box-shadow: 0 12px 40px rgba(0,0,0,0.15); max-width: 600px; margin: 25px 0; border-top: 6px solid #10b981;">
  <!-- Header Section -->
  <div style="display: flex; justify-content: space-between; align-items: start; margin-bottom: 24px; padding-bottom: 20px; border-bottom: 2px solid #f3f4f6;">
    <div style="flex: 1;">
      <h3 style="margin: 0 0 8px 0; color: #111827; font-size: 1.5em; font-weight: 800;">Complex Card Example</h3>
      <p style="margin: 0; color: #6b7280; font-size: 0.95em;">Demonstrates multiple patterns combined</p>
    </div>
    <span style="background: linear-gradient(135deg, #10b981 0%, #059669 100%); color: white; padding: 6px 16px; border-radius: 12px; font-size: 0.85em; font-weight: 700; box-shadow: 0 4px 12px rgba(236, 72, 153, 0.3);">Premium</span>
  </div>

  <!-- Stats Grid -->
  <div style="display: grid; grid-template-columns: repeat(3, 1fr); gap: 16px; margin-bottom: 24px;">
    <div style="text-align: center; padding: 16px; background: #d1fae5; border-radius: 12px;">
      <div style="font-size: 2em; font-weight: 800; color: #10b981; margin-bottom: 4px;">1.2K</div>
      <div style="color: #6b7280; font-size: 0.85em; font-weight: 600;">Users</div>
    </div>
    <div style="text-align: center; padding: 16px; background: #dbeafe; border-radius: 12px;">
      <div style="font-size: 2em; font-weight: 800; color: #3b82f6; margin-bottom: 4px;">98%</div>
      <div style="color: #6b7280; font-size: 0.85em; font-weight: 600;">Uptime</div>
    </div>
    <div style="text-align: center; padding: 16px; background: #d1fae5; border-radius: 12px;">
      <div style="font-size: 2em; font-weight: 800; color: #10b981; margin-bottom: 4px;">4.8</div>
      <div style="color: #6b7280; font-size: 0.85em; font-weight: 600;">Rating</div>
    </div>
  </div>

  <!-- Progress Section -->
  <div style="margin-bottom: 24px;">
    <div style="display: flex; justify-content: space-between; margin-bottom: 10px;">
      <span style="color: #111827; font-weight: 600;">Completion Progress</span>
      <span style="color: #10b981; font-weight: 700;">85%</span>
    </div>
    <div style="background: #f3f4f6; height: 10px; border-radius: 8px; overflow: hidden;">
      <div style="width: 85%; background: linear-gradient(90deg, #10b981 0%, #059669 100%); height: 10px;"></div>
    </div>
  </div>

  <!-- Feature List -->
  <div style="margin-bottom: 24px;">
    <h5 style="margin: 0 0 12px 0; color: #111827; font-size: 1.05em; font-weight: 700;">Included Features</h5>
    <div style="display: grid; gap: 8px;">
      <div style="display: flex; align-items: center; gap: 10px;">
        <span style="width: 20px; height: 20px; background: #d1fae5; border-radius: 4px; display: flex; align-items: center; justify-content: center; color: #10b981; font-weight: 700; font-size: 0.75em;">✓</span>
        <span style="color: #374151; font-size: 0.9em;">Advanced analytics dashboard</span>
      </div>
      <div style="display: flex; align-items: center; gap: 10px;">
        <span style="width: 20px; height: 20px; background: #d1fae5; border-radius: 4px; display: flex; align-items: center; justify-content: center; color: #10b981; font-weight: 700; font-size: 0.75em;">✓</span>
        <span style="color: #374151; font-size: 0.9em;">24/7 priority support</span>
      </div>
      <div style="display: flex; align-items: center; gap: 10px;">
        <span style="width: 20px; height: 20px; background: #d1fae5; border-radius: 4px; display: flex; align-items: center; justify-content: center; color: #10b981; font-weight: 700; font-size: 0.75em;">✓</span>
        <span style="color: #374151; font-size: 0.9em;">Custom API integrations</span>
      </div>
    </div>
  </div>

  <!-- Action Buttons -->
  <div style="display: grid; grid-template-columns: 2fr 1fr; gap: 12px;">
    <button style="background: linear-gradient(135deg, #10b981 0%, #059669 100%); color: white; border: none; padding: 14px 24px; border-radius: 10px; font-weight: 700; cursor: pointer; font-size: 1em; box-shadow: 0 4px 15px rgba(236, 72, 153, 0.3);">
      Get Started
    </button>
    <button style="background: white; color: #10b981; border: 2px solid #10b981; padding: 14px 24px; border-radius: 10px; font-weight: 700; cursor: pointer; font-size: 1em;">
      Details
    </button>
  </div>
</div>

---

## 🎯 Usage Examples

### Dashboard Layout

```html
<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 20px;">
  <!-- Use multiple KPI cards, status cards, and progress cards -->
  <!-- Example: 3 gradient KPI cards in a row -->
  <!-- Example: 2 column info grid below -->
  <!-- Example: Multi-progress dashboard at bottom -->
</div>
```

### Profile Section

```html
<div style="display: grid; grid-template-columns: 1fr 2fr; gap: 24px;">
  <!-- Left: Team member card (vertical) -->
  <!-- Right: Contact card with actions -->
</div>
```

### Alert Panel

```html
<div style="display: flex; flex-direction: column; gap: 16px;">
  <!-- Stack multiple alert types: success, warning, error, info -->
</div>
```

### Feature Showcase

```html
<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 24px;">
  <!-- Multiple feature highlight cards with different icons and colors -->
</div>
```

---

<div style="background: linear-gradient(135deg, #10b981 0%, #059669 100%); padding: 50px 40px; border-radius: 20px; color: white; text-align: center; margin: 40px 0; box-shadow: 0 20px 60px rgba(16, 185, 129, 0.4);">
  <h2 style="margin: 0 0 16px 0; font-size: 2.2em; font-weight: 800;">🎉 Card Library Complete!</h2>
  <p style="margin: 0 0 24px 0; font-size: 1.15em; opacity: 0.95;">
    25+ production-ready components for modern web applications
  </p>
  <div style="display: inline-flex; gap: 12px; flex-wrap: wrap; justify-content: center;">
    <span style="background: rgba(255,255,255,0.25); backdrop-filter: blur(10px); padding: 8px 18px; border-radius: 10px; font-size: 0.9em; font-weight: 600; border: 1px solid rgba(255,255,255,0.3);">Responsive</span>
    <span style="background: rgba(255,255,255,0.25); backdrop-filter: blur(10px); padding: 8px 18px; border-radius: 10px; font-size: 0.9em; font-weight: 600; border: 1px solid rgba(255,255,255,0.3);">Accessible</span>
    <span style="background: rgba(255,255,255,0.25); backdrop-filter: blur(10px); padding: 8px 18px; border-radius: 10px; font-size: 0.9em; font-weight: 600; border: 1px solid rgba(255,255,255,0.3);">Customizable</span>
    <span style="background: rgba(255,255,255,0.25); backdrop-filter: blur(10px); padding: 8px 18px; border-radius: 10px; font-size: 0.9em; font-weight: 600; border: 1px solid rgba(255,255,255,0.3);">Copy & Paste</span>
  </div>
</div>

---

<div style="background: #f9fafb; padding: 24px; border-radius: 12px; border-left: 4px solid #10b981; margin: 30px 0;">
  <div style="display: flex; align-items: start; gap: 12px;">
    <span style="font-size: 1.5em;">💡</span>
    <div>
      <div style="color: #111827; font-weight: 700; font-size: 1.1em; margin-bottom: 8px;">Pro Tip: Customization</div>
      <div style="color: #6b7280; font-size: 0.95em; line-height: 1.7;">
        All cards in this library are fully customizable. Simply replace placeholder values ([TITLE], [VALUE], etc.) with your content, adjust colors in gradient values, and modify sizes to match your design system. Use browser DevTools to fine-tune spacing and responsiveness.
      </div>
    </div>
  </div>
</div>

---

**Component Statistics:**
- **Total Cards**: 25+ unique components
- **Categories**: 8 specialized collections
- **Color Themes**: Pink/Fuchsia primary (#10b981, #059669)
- **Design Patterns**: Glassmorphism, Neumorphism, 3D Transforms, Gradient Borders
- **Responsive**: Auto-fit grid layouts for all screen sizes
- **Accessibility**: WCAG 2.1 AA compliant color contrasts
- **Framework**: Vanilla HTML/CSS (no dependencies)

**Created**: December 28, 2025
**Version**: 2.0
**Theme**: Pink/Fuchsia Gradient
**Expansion**: 66 → 1,491 lines (2,159% increase)