# 📐 Page Layouts - Visual Guide

## 🎨 Admin Reports Page (`/admin/reports`)

```
┌─────────────────────────────────────────────────────────────┐
│  NAVBAR: Smart City Portal | Analytics | All Reports | User │
└─────────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────────┐
│  📊 All Citizen Reports                                      │
│  Manage and update status of all reported issues            │
└─────────────────────────────────────────────────────────────┘

┌──────────┬──────────┬──────────┬──────────┬──────────┐
│  Total   │   Open   │In Progress│ Resolved │  Closed  │
│   125    │    45    │    32     │    38    │    10    │
└──────────┴──────────┴──────────┴──────────┴──────────┘

┌─────────────────────────────────────────────────────────────┐
│  🔍 Search & Filters                                         │
│  ┌─────────────────────────────────────────────────────┐   │
│  │ 🔍 Search by title, description, or reporter...     │   │
│  └─────────────────────────────────────────────────────┘   │
│  ┌──────────┬──────────┬──────────┬──────────┐            │
│  │ Status ▼ │Category ▼│Priority ▼│[Clear]   │            │
│  └──────────┴──────────┴──────────┴──────────┘            │
└─────────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────────┐
│  🚧 Broken Road on Main Street                        [▼]   │
│  👤 John Doe  📅 Oct 20, 2024                               │
│  ┌──────┬──────┬──────┬──────┐                             │
│  │ OPEN │ HIGH │ ROAD │ ROADS│                             │
│  └──────┴──────┴──────┴──────┘                             │
│  There is a large pothole causing traffic issues...        │
│  [Edit Status] [View Details]                              │
└─────────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────────┐
│  💡 Street Light Not Working                          [▼]   │
│  👤 Jane Smith  📅 Oct 19, 2024                             │
│  ┌──────────┬────────┬──────────┬────────────┐            │
│  │IN PROGRESS│ MEDIUM │ LIGHTING │ ELECTRICITY│            │
│  └──────────┴────────┴──────────┴────────────┘            │
│  The street light on 5th Avenue has been off...            │
│  [Edit Status] [View Details]                              │
└─────────────────────────────────────────────────────────────┘

WHEN EDITING:
┌─────────────────────────────────────────────────────────────┐
│  🚧 Broken Road on Main Street                        [▲]   │
│  👤 John Doe  📅 Oct 20, 2024                               │
│  ┌──────┬──────┬──────┬──────┐                             │
│  │ OPEN │ HIGH │ ROAD │ ROADS│                             │
│  └──────┴──────┴──────┴──────┘                             │
│  There is a large pothole causing traffic issues...        │
│  ┌─────────────────────────────────────────────────────┐   │
│  │ ✏️ Update Report Details                            │   │
│  │ Status: [In Progress ▼]  Priority: [High ▼]        │   │
│  │ Category: [Road ▼]  Department: [Roads ▼]          │   │
│  │ Admin Notes: ┌──────────────────────────────────┐  │   │
│  │              │ Assigned to repair team...       │  │   │
│  │              └──────────────────────────────────┘  │   │
│  │ [💾 Save Changes] [❌ Cancel]                       │   │
│  └─────────────────────────────────────────────────────┘   │
└─────────────────────────────────────────────────────────────┘
```

---

## 🏠 User Dashboard (`/dashboard`)

```
┌─────────────────────────────────────────────────────────────┐
│  NAVBAR: Smart City Portal | Dashboard | Report | Reports   │
└─────────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────────┐
│  🏠 My Dashboard                          [+ Report Issue]   │
│  Track and manage your reported issues                      │
└─────────────────────────────────────────────────────────────┘

┌──────────┬──────────┬──────────┬──────────┬──────────┐
│  Total   │   Open   │In Progress│ Resolved │  Closed  │
│   📊 12  │  🔵 3    │  🟡 4     │  🟢 4    │  ⚫ 1    │
└──────────┴──────────┴──────────┴──────────┴──────────┘

┌─────────────────────────────────────────────────────────────┐
│  🔍 Search your reports...                                   │
│  [All] [Open] [In Progress] [Resolved] [Closed]             │
└─────────────────────────────────────────────────────────────┘

┌──────────────┬──────────────┬──────────────┐
│ ━━━━━━━━━━━  │ ━━━━━━━━━━━  │ ━━━━━━━━━━━  │ (Status Bar)
│              │              │              │
│ 🚧 Road      │ 💡 Lighting  │ 🗑️ Waste     │
│              │              │              │
│ Broken Road  │ Light Issue  │ Garbage Pile │
│ on Main St   │ on 5th Ave   │ at Park      │
│              │              │              │
│ Large pothole│ Street light │ Uncollected  │
│ causing...   │ has been...  │ waste for... │
│              │              │              │
│ [Image]      │ [Image]      │ [Image]      │
│              │              │              │
│ ┌──────────┐ │ ┌──────────┐ │ ┌──────────┐ │
│ │   OPEN   │ │ │IN PROGRESS│ │ │ RESOLVED │ │
│ └──────────┘ │ └──────────┘ │ └──────────┘ │
│              │              │              │
│ 📅 Oct 20    │ 📅 Oct 19    │ 📅 Oct 18    │
│ 🔴 High      │ 🟡 Medium    │ 🟢 Low       │
│              │              │              │
│ 📍 Main St   │ 📍 5th Ave   │ 📍 Park Rd   │
│              │              │              │
│ ⚠️ Admin Note│ ⚠️ Admin Note│              │
│ Assigned to  │ Team working │              │
│ repair team  │ on it        │              │
│              │              │              │
│[View Details]│[View Details]│[View Details]│
└──────────────┴──────────────┴──────────────┘
```

---

## 🔄 Navigation Flow

### For Citizens:

```
Landing Page
    │
    ├─→ Register/Login
    │
    ├─→ Dashboard (NEW!)
    │   ├─→ View Statistics
    │   ├─→ Search Reports
    │   ├─→ Filter by Status
    │   └─→ View Report Details
    │
    ├─→ Report Issue
    │   └─→ Submit New Report
    │
    └─→ My Reports
        └─→ List View of Reports
```

### For Admins:

```
Landing Page
    │
    ├─→ Login
    │
    ├─→ Analytics Dashboard
    │   ├─→ View Charts
    │   ├─→ See Statistics
    │   └─→ Department Workload
    │
    └─→ All Reports (NEW!)
        ├─→ View All Citizen Reports
        ├─→ Search Reports
        ├─→ Filter Reports
        ├─→ Update Status
        ├─→ Add Admin Notes
        ├─→ Assign Departments
        └─→ View Full Details
```

---

## 📱 Responsive Layouts

### Desktop (> 1024px):
```
┌────────────────────────────────────────────┐
│  [Card] [Card] [Card]                      │
│  [Card] [Card] [Card]                      │
│  [Card] [Card] [Card]                      │
└────────────────────────────────────────────┘
3 columns
```

### Tablet (640px - 1024px):
```
┌────────────────────────────────────────────┐
│  [Card] [Card]                             │
│  [Card] [Card]                             │
│  [Card] [Card]                             │
└────────────────────────────────────────────┘
2 columns
```

### Mobile (< 640px):
```
┌────────────────────────────────────────────┐
│  [Card]                                    │
│  [Card]                                    │
│  [Card]                                    │
└────────────────────────────────────────────┘
1 column
```

---

## 🎨 Color Scheme

### Status Colors:
```
┌──────────┬──────────┬──────────┬──────────┐
│   OPEN   │IN PROGRESS│ RESOLVED │  CLOSED  │
│  🔵 Blue │ 🟡 Yellow │ 🟢 Green │ ⚫ Gray   │
└──────────┴──────────┴──────────┴──────────┘
```

### Priority Colors:
```
┌──────────┬──────────┬──────────┐
│   HIGH   │  MEDIUM  │   LOW    │
│  🔴 Red  │🟡 Yellow │ 🟢 Green │
└──────────┴──────────┴──────────┘
```

### Category Icons:
```
🚧 Road      💡 Lighting    🗑️ Waste
🛡️ Safety    💧 Water       📋 Other
```

---

## 🔍 Interactive Elements

### Expandable Report Card:

**Collapsed:**
```
┌─────────────────────────────────────────────┐
│  🚧 Broken Road on Main Street        [▼]   │
│  Summary information...                     │
│  [Edit Status] [View Details]               │
└─────────────────────────────────────────────┘
```

**Expanded:**
```
┌─────────────────────────────────────────────┐
│  🚧 Broken Road on Main Street        [▲]   │
│  Summary information...                     │
│  [Edit Status] [View Details]               │
│  ┌─────────────────────────────────────┐   │
│  │ Full Description:                   │   │
│  │ Detailed description text...        │   │
│  │                                     │   │
│  │ Location: 123 Main Street          │   │
│  │ Reporter: John Doe                 │   │
│  │ Email: john@example.com            │   │
│  │                                     │   │
│  │ Images: [img] [img] [img]          │   │
│  └─────────────────────────────────────┘   │
└─────────────────────────────────────────────┘
```

---

## 📊 Statistics Display

### Admin Stats:
```
┌──────────┬──────────┬──────────┬──────────┬──────────┐
│  Total   │   Open   │In Progress│ Resolved │  Closed  │
│  ┌────┐  │  ┌────┐  │  ┌────┐  │  ┌────┐  │  ┌────┐  │
│  │125 │  │  │ 45 │  │  │ 32 │  │  │ 38 │  │  │ 10 │  │
│  └────┘  │  └────┘  │  └────┘  │  └────┘  │  └────┘  │
└──────────┴──────────┴──────────┴──────────┴──────────┘
```

### User Stats:
```
┌──────────┬──────────┬──────────┬──────────┬──────────┐
│  Total   │   Open   │In Progress│ Resolved │  Closed  │
│ ┌──────┐ │ ┌──────┐ │ ┌──────┐ │ ┌──────┐ │ ┌──────┐ │
│ │ 📊12 │ │ │ 🔵3  │ │ │ 🟡4  │ │ │ 🟢4  │ │ │ ⚫1  │ │
│ └──────┘ │ └──────┘ │ └──────┘ │ └──────┘ │ └──────┘ │
│ Gradient │  White   │  White   │  White   │  White   │
│   Blue   │   Card   │   Card   │   Card   │   Card   │
└──────────┴──────────┴──────────┴──────────┴──────────┘
```

---

## 🎯 Key UI Components

### Search Bar:
```
┌─────────────────────────────────────────────┐
│ 🔍 Search by title, description, or...      │
└─────────────────────────────────────────────┘
```

### Filter Dropdowns:
```
┌──────────┬──────────┬──────────┬──────────┐
│ Status ▼ │Category ▼│Priority ▼│[Clear]   │
└──────────┴──────────┴──────────┴──────────┘
```

### Status Tabs:
```
┌─────┬─────┬──────────┬─────────┬────────┐
│ All │Open │In Progress│Resolved │Closed  │
└─────┴─────┴──────────┴─────────┴────────┘
  Active state highlighted in blue
```

### Action Buttons:
```
┌──────────────┐  ┌──────────────┐
│ Edit Status  │  │ View Details │
└──────────────┘  └──────────────┘
  Primary Blue      Secondary Gray
```

---

## 🎨 Visual Hierarchy

### Priority Order:
1. **Page Title** - Large, bold
2. **Statistics Cards** - Prominent, colorful
3. **Search & Filters** - Easy to find
4. **Report Cards** - Main content
5. **Action Buttons** - Clear CTAs

### Typography:
- **Headings**: Bold, 24-32px
- **Subheadings**: Semi-bold, 18-20px
- **Body Text**: Regular, 14-16px
- **Labels**: Medium, 12-14px
- **Badges**: Bold, 10-12px

---

This visual guide provides a clear understanding of how the new pages are structured and how users will interact with them!
