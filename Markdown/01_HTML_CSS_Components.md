# HTML/CSS Components Template

**Purpose**: Beautiful HTML/CSS styling components for markdown
**Source**: Compiled from 6 Obsidian vault templates
**Usage**: Copy and customize these components for your markdown files

---

## Table of Contents
1. [Gradient Cards](#gradient-cards)
2. [Profile Avatar Cards](#profile-avatar-cards)
3. [Flexbox Layouts](#flexbox-layouts)
4. [Animated SVG Elements](#animated-svg-elements)
5. [Grid Layouts](#grid-layouts)
6. [Status Indicators](#status-indicators)

---

## Gradient Cards

### Linear Gradient Card (Red to Orange)
```html
<div style="border: 1px solid #ddd; border-radius: 12px; padding: 20px; background: linear-gradient(135deg, #ff416c 0%, #ff4b2b 100%); color: white; margin: 15px 0; box-shadow: 0 4px 6px rgba(0,0,0,0.1);">
    <h3 style="margin: 0 0 10px 0;">Card Title</h3>
    <p style="margin: 0; opacity: 0.9;">Card content goes here with beautiful gradient background</p>
</div>
```

**Live Example**:
<div style="border: 1px solid #ddd; border-radius: 12px; padding: 20px; background: linear-gradient(135deg, #ff416c 0%, #ff4b2b 100%); color: white; margin: 15px 0; box-shadow: 0 4px 6px rgba(0,0,0,0.1);">
    <h3 style="margin: 0 0 10px 0;">Beautiful Gradient Card</h3>
    <p style="margin: 0; opacity: 0.9;">This card uses a 135-degree linear gradient from pink to orange-red</p>
</div>

### Blue to Purple Gradient Card
```html
<div style="border: 1px solid #ddd; border-radius: 12px; padding: 20px; background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); color: white; margin: 15px 0; box-shadow: 0 4px 6px rgba(0,0,0,0.1);">
    <h3 style="margin: 0 0 10px 0;">Blue to Purple</h3>
    <p style="margin: 0; opacity: 0.9;">Professional gradient for dashboards and metrics</p>
</div>
```

**Live Example**:
<div style="border: 1px solid #ddd; border-radius: 12px; padding: 20px; background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); color: white; margin: 15px 0; box-shadow: 0 4px 6px rgba(0,0,0,0.1);">
    <h3 style="margin: 0 0 10px 0;">Blue to Purple</h3>
    <p style="margin: 0; opacity: 0.9;">Professional gradient for dashboards and metrics</p>
</div>

### Green to Teal Gradient Card
```html
<div style="border: 1px solid #ddd; border-radius: 12px; padding: 20px; background: linear-gradient(135deg, #11998e 0%, #38ef7d 100%); color: white; margin: 15px 0; box-shadow: 0 4px 6px rgba(0,0,0,0.1);">
    <h3 style="margin: 0 0 10px 0;">Success State</h3>
    <p style="margin: 0; opacity: 0.9;">Perfect for positive metrics and achievements</p>
</div>
```

---

## Profile Avatar Cards

### Circular Avatar with Initials
```html
<div style="display: flex; align-items: center; gap: 15px; padding: 15px; border: 1px solid #eee; border-radius: 8px;">
    <div style="width: 60px; height: 60px; border-radius: 50%; background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); display: flex; align-items: center; justify-content: center; color: white; font-size: 24px; font-weight: bold;">
        JD
    </div>
    <div>
        <h4 style="margin: 0 0 5px 0;">John Doe</h4>
        <p style="margin: 0; color: #666; font-size: 14px;">Software Engineer</p>
    </div>
</div>
```

**Live Example**:
<div style="display: flex; align-items: center; gap: 15px; padding: 15px; border: 1px solid #eee; border-radius: 8px;">
    <div style="width: 60px; height: 60px; border-radius: 50%; background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); display: flex; align-items: center; justify-content: center; color: white; font-size: 24px; font-weight: bold;">
        JD
    </div>
    <div>
        <h4 style="margin: 0 0 5px 0;">John Doe</h4>
        <p style="margin: 0; color: #666; font-size: 14px;">Software Engineer</p>
    </div>
</div>

### Contact Card with Avatar
```html
<div style="border: 1px solid #ddd; border-radius: 12px; padding: 20px; background: linear-gradient(135deg, #ff416c 0%, #ff4b2b 100%); color: white; margin: 15px 0; box-shadow: 0 4px 6px rgba(0,0,0,0.1);">
    <div style="display: flex; justify-content: space-between; align-items: flex-start; margin-bottom: 15px;">
        <div style="width: 60px; height: 60px; border-radius: 50%; background: white; display: flex; align-items: center; justify-content: center; color: #ff416c; font-size: 24px; font-weight: bold;">
            F
        </div>
        <div style="text-align: right;">
            <p style="margin: 0; font-size: 12px; opacity: 0.8;">ID: #12345</p>
            <p style="margin: 0; font-size: 12px; opacity: 0.8;">Status: Active</p>
        </div>
    </div>
    <h3 style="margin: 0 0 10px 0;">Full Name</h3>
    <p style="margin: 0 0 5px 0; opacity: 0.9;">📧 email@example.com</p>
    <p style="margin: 0; opacity: 0.9;">📱 +1 (555) 123-4567</p>
</div>
```

---

## Flexbox Layouts

### Two-Column Flex Layout
```html
<div style="display: flex; gap: 20px; margin: 20px 0;">
    <div style="flex: 1; padding: 20px; border: 1px solid #ddd; border-radius: 8px; background: #f9f9f9;">
        <h4 style="margin-top: 0;">Left Column</h4>
        <p>Content for the left side</p>
    </div>
    <div style="flex: 1; padding: 20px; border: 1px solid #ddd; border-radius: 8px; background: #f9f9f9;">
        <h4 style="margin-top: 0;">Right Column</h4>
        <p>Content for the right side</p>
    </div>
</div>
```

### Three-Column Flex Layout
```html
<div style="display: flex; gap: 15px; margin: 20px 0;">
    <div style="flex: 1; padding: 15px; border: 1px solid #ddd; border-radius: 8px; background: #f9f9f9;">
        <h5 style="margin-top: 0;">Column 1</h5>
        <p style="margin: 0; font-size: 14px;">Content here</p>
    </div>
    <div style="flex: 1; padding: 15px; border: 1px solid #ddd; border-radius: 8px; background: #f9f9f9;">
        <h5 style="margin-top: 0;">Column 2</h5>
        <p style="margin: 0; font-size: 14px;">Content here</p>
    </div>
    <div style="flex: 1; padding: 15px; border: 1px solid #ddd; border-radius: 8px; background: #f9f9f9;">
        <h5 style="margin-top: 0;">Column 3</h5>
        <p style="margin: 0; font-size: 14px;">Content here</p>
    </div>
</div>
```

### Centered Content with Flexbox
```html
<div style="display: flex; justify-content: center; align-items: center; min-height: 200px; border: 2px dashed #ddd; border-radius: 8px;">
    <div style="text-align: center;">
        <h3 style="margin: 0 0 10px 0;">Perfectly Centered</h3>
        <p style="margin: 0; color: #666;">Both horizontally and vertically</p>
    </div>
</div>
```

---

## Animated SVG Elements

### Pulsing Circle Indicator
```html
<div style="position: relative; display: inline-block;">
    <svg width="22" height="22">
        <circle cx="11" cy="11" r="9" fill="none" stroke="#4cd964" stroke-width="3"
                stroke-dasharray="56.5" stroke-dashoffset="0"
                style="animation: archPulse 1.8s infinite alternate;"/>
        <style>
            @keyframes archPulse {
                0% { stroke-dashoffset: 0; }
                100% { stroke-dashoffset: 28; }
            }
        </style>
    </svg>
</div>
```

**Live Example**:
<div style="position: relative; display: inline-block;">
    <svg width="22" height="22">
        <circle cx="11" cy="11" r="9" fill="none" stroke="#4cd964" stroke-width="3"
                stroke-dasharray="56.5" stroke-dashoffset="0"
                style="animation: archPulse 1.8s infinite alternate;"/>
        <style>
            @keyframes archPulse {
                0% { stroke-dashoffset: 0; }
                100% { stroke-dashoffset: 28; }
            }
        </style>
    </svg>
</div>

### Status Indicator with Animation
```html
<div style="display: inline-flex; align-items: center; gap: 8px; padding: 8px 16px; border-radius: 20px; background: #e8f5e9;">
    <svg width="12" height="12">
        <circle cx="6" cy="6" r="5" fill="#4cd964" style="animation: statusPulse 2s infinite;"/>
        <style>
            @keyframes statusPulse {
                0%, 100% { opacity: 1; }
                50% { opacity: 0.5; }
            }
        </style>
    </svg>
    <span style="color: #2e7d32; font-weight: 500; font-size: 14px;">Active</span>
</div>
```

---

## Grid Layouts

### Two-Column Grid
```html
<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 20px; margin: 20px 0;">
    <div style="padding: 20px; border: 1px solid #ddd; border-radius: 8px; background: #f9f9f9;">
        <h4 style="margin-top: 0;">Grid Item 1</h4>
        <p>Content for first grid item</p>
    </div>
    <div style="padding: 20px; border: 1px solid #ddd; border-radius: 8px; background: #f9f9f9;">
        <h4 style="margin-top: 0;">Grid Item 2</h4>
        <p>Content for second grid item</p>
    </div>
</div>
```

### Three-Column Grid
```html
<div style="display: grid; grid-template-columns: repeat(3, 1fr); gap: 15px; margin: 20px 0;">
    <div style="padding: 15px; border: 1px solid #ddd; border-radius: 8px; background: #f9f9f9;">
        <h5 style="margin-top: 0;">Item 1</h5>
    </div>
    <div style="padding: 15px; border: 1px solid #ddd; border-radius: 8px; background: #f9f9f9;">
        <h5 style="margin-top: 0;">Item 2</h5>
    </div>
    <div style="padding: 15px; border: 1px solid #ddd; border-radius: 8px; background: #f9f9f9;">
        <h5 style="margin-top: 0;">Item 3</h5>
    </div>
</div>
```

### Four-Column Metric Grid
```html
<div style="display: grid; grid-template-columns: repeat(4, 1fr); gap: 15px; margin: 20px 0;">
    <div style="padding: 20px; border-radius: 8px; background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); color: white; text-align: center;">
        <div style="font-size: 32px; font-weight: bold; margin-bottom: 5px;">150</div>
        <div style="font-size: 14px; opacity: 0.9;">Total Users</div>
    </div>
    <div style="padding: 20px; border-radius: 8px; background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%); color: white; text-align: center;">
        <div style="font-size: 32px; font-weight: bold; margin-bottom: 5px;">45</div>
        <div style="font-size: 14px; opacity: 0.9;">Active Now</div>
    </div>
    <div style="padding: 20px; border-radius: 8px; background: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%); color: white; text-align: center;">
        <div style="font-size: 32px; font-weight: bold; margin-bottom: 5px;">89%</div>
        <div style="font-size: 14px; opacity: 0.9;">Satisfaction</div>
    </div>
    <div style="padding: 20px; border-radius: 8px; background: linear-gradient(135deg, #43e97b 0%, #38f9d7 100%); color: white; text-align: center;">
        <div style="font-size: 32px; font-weight: bold; margin-bottom: 5px;">$12.5k</div>
        <div style="font-size: 14px; opacity: 0.9;">Revenue</div>
    </div>
</div>
```

---

## Status Indicators

### Progress Bar
```html
<div style="margin: 20px 0;">
    <div style="display: flex; justify-content: space-between; margin-bottom: 5px;">
        <span style="font-size: 14px; font-weight: 500;">Project Progress</span>
        <span style="font-size: 14px; color: #666;">75%</span>
    </div>
    <div style="width: 100%; height: 8px; background: #e0e0e0; border-radius: 4px; overflow: hidden;">
        <div style="width: 75%; height: 100%; background: linear-gradient(90deg, #667eea 0%, #764ba2 100%); border-radius: 4px;"></div>
    </div>
</div>
```

**Live Example**:
<div style="margin: 20px 0;">
    <div style="display: flex; justify-content: space-between; margin-bottom: 5px;">
        <span style="font-size: 14px; font-weight: 500;">Project Progress</span>
        <span style="font-size: 14px; color: #666;">75%</span>
    </div>
    <div style="width: 100%; height: 8px; background: #e0e0e0; border-radius: 4px; overflow: hidden;">
        <div style="width: 75%; height: 100%; background: linear-gradient(90deg, #667eea 0%, #764ba2 100%); border-radius: 4px;"></div>
    </div>
</div>

### Status Badges
```html
<div style="display: flex; gap: 10px; margin: 20px 0;">
    <span style="padding: 4px 12px; border-radius: 12px; background: #e8f5e9; color: #2e7d32; font-size: 12px; font-weight: 500;">✓ Active</span>
    <span style="padding: 4px 12px; border-radius: 12px; background: #fff3e0; color: #e65100; font-size: 12px; font-weight: 500;">⏸ Pending</span>
    <span style="padding: 4px 12px; border-radius: 12px; background: #ffebee; color: #c62828; font-size: 12px; font-weight: 500;">✕ Inactive</span>
</div>
```

**Live Example**:
<div style="display: flex; gap: 10px; margin: 20px 0;">
    <span style="padding: 4px 12px; border-radius: 12px; background: #e8f5e9; color: #2e7d32; font-size: 12px; font-weight: 500;">✓ Active</span>
    <span style="padding: 4px 12px; border-radius: 12px; background: #fff3e0; color: #e65100; font-size: 12px; font-weight: 500;">⏸ Pending</span>
    <span style="padding: 4px 12px; border-radius: 12px; background: #ffebee; color: #c62828; font-size: 12px; font-weight: 500;">✕ Inactive</span>
</div>

---

## Best Practices

1. **Use Box Shadow for Depth**: Add `box-shadow: 0 4px 6px rgba(0,0,0,0.1);` for subtle depth
2. **Border Radius for Smooth Edges**: Use `border-radius: 8px` to `12px` for modern look
3. **Gradient Angles**: 135deg creates diagonal gradients (most visually appealing)
4. **White Space**: Add generous padding (15px-20px) for breathing room
5. **Color Contrast**: Ensure text is readable on gradient backgrounds (use white text)
6. **Flexbox vs Grid**: Use flexbox for one-dimensional layouts, grid for two-dimensional
7. **Animation Duration**: Keep animations between 1-2 seconds for smooth effects
8. **Responsive Design**: Use `flex: 1` or `grid-template-columns: repeat(auto-fit, minmax(200px, 1fr))`

---

**Template Version**: 1.0
**Last Updated**: 2025-12-28
**Source Files**: 6 Obsidian markdown templates
