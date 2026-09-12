

```markdown
# Agri Farma Express — Technical & Operational Overview

## Problem Statement
Traditional agricultural procurement mandis face severe logistical bottlenecks during peak harvest seasons. Farmers endure queues lasting between 12 and 48 hours, exposing crops to post-harvest degradation, open weather damage, and high operational inefficiencies.

## Solution Architecture
Agri Farma Express replaces open-ended queues with a **Dynamic Token & Geofenced Scheduling System**. 

### 1. Inclusive Access Architecture
To ensure complete coverage across all farmer demographics, token allocation is accessible through:
- **Smartphone PWA App:** Native web portal for digital-first users.
- **IVR / Voice Bot / SMS:** Interactive voice menu accessible via feature phones without internet requirements.
- **Vernacular WhatsApp Assistant:** Direct message-based token booking.
- **Assisted KVK / CSC Desks:** Physical support hubs for non-tech-literate farmers.

### 2. Geofence Perimeter Logic
- **Standby State (> 2 km):** Farmers receive a broad delivery window.
- **Active State (< 2 km):** As the delivery truck crosses the 2 km perimeter, the system dynamically promotes the token into the gate queue line to ensure optimal weighbridge utilization.

### 3. Operational Impact Matrix
| Metric | Traditional Mandi Model | Agri Farma Express Model |
| :--- | :--- | :--- |
| **Average Queue Wait Time** | 12 – 48 Hours | 1 – 2 Hours |
| **Gate Verification** | Manual Paper Receipts | Instant QR Optical Scan |
| **Spoilage Risk** | High (Open Air Waiting) | Low (Just-in-Time Scheduling) |
| **Payment Pipeline** | Delayed Manual Ledger | Integrated Direct Benefit Transfer (DBT) |

---

## Implementation Footprint
- **Minimal Field Hardware:** Mandi gate operators require only a basic mobile tablet or handheld scanner.
- **Scalable Hosting:** Fully static client-side single-page layout ready for immediate deployment on web edge nodes.
