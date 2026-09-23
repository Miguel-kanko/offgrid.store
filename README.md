<p align="center">
  <img src="illustration.png" width="500"/>
</p>

 ### How it Works (Concept Diagram)
> *Illustration of the SMS code flow - Conceptual architecture*

# offgrid.store - Commerce Without Internet
> Buy in Paris, collect in Awaé. An offline-first protocol for rural Cameroon.

**Author:** KANKO DJOUA MIGUEL - L1 Software Engineering, IAI Yaoundé
**Location:** Awaé, Centre Region, Cameroon
**Contact:** kankodjouamiguel@gmail.com
**Goal:** Build the first offline marketplace dataset from rural Cameroon for PhD Research (UT Dallas 2029) on Offline-First Systems.

### The Problem
In Awaé, near Yaoundé:
- 60% of sellers have no stable internet. When MTN cuts, business stops.
- Farmers lose 40% of harvest because they can't find buyers offline.
- Apps like Jumia need 100% internet. They don't work here.
- 6 Million Cameroonians in the diaspora (France/USA) want to buy for their family in the village, but can't send Mobile Money to someone who is offline.

### The Vision: How it Will Work
Not an app that needs internet, but a protocol that works without it.

**1. 100% Offline Vendor App:** A mama in Awaé can add "1 bag of cassava - 15.000 FCFA" on her phone with ZERO internet. It's saved locally on her phone (SQLite).

**2. The SMS Code System (No Internet Needed):** The app generates a code offline: `OFFGRID-7A3B: 1 bag of cassava from Mary - Awaé Market`. The buyer just shows this code. No smartphone needed to collect.

**3. Diaspora Mode:** My cousin in Paris pays on offgrid.store website (online). The system sends an SMS to the family in Awaé with the collection code. The village seller validates the code OFFLINE from her app.

**4. Auto-Sync:** When MTN network comes back, all the offline sales sync automatically to the cloud.

### Why This Matters for Research
This will be the first dataset of real offline commerce from rural Cameroon.
- **Research Topics:** Offline-First Distributed Systems (CRDTs), SMS-based consensus, FinTech for Diaspora, Offline AI for local languages (Ewondo, Bassa).
- **Impact:** A solution for the 60% of Cameroonians excluded from e-commerce.

### Current Status: BUILD PHASE - Sept 2026
I have completed field research in Awaé:

- **Sept 3, 2026:** Documented 50 real products with real prices (cassava, plantain, palm oil, etc.) in FCFA from Awaé Market - file: `data/product.json`
- **Fieldwork:** Interviewed 12 sellers (2h each) - Main finding: MTN cuts 3-4h/day, they lose clients
- **Test:** Tested SMS collection logic with my uncle - validated that code system can work without internet
- **Learning:** Currently learning Flutter + SQLite
- **Next:** Build offline vendor app that shows the 50 products 100% offline + generates OFFGRID code

### Real Market Data
- **Live dataset:** [50 products from Awaé Market - Sept 2026](./data/products.json)
- **Fieldwork log:** [Fieldwork - Sept 3, 2026](./research/fieldwork-03-sept-2026.md)

### Tech Stack (Planned)
Flutter, SQLite, Firebase (for sync only), MTN MoMo API, SMS Gateway / USSD

### Inspired by
@sanix-darker and the OSS Cameroon community - building simple tools for complex African problems.

---
**I am looking for mentors in Offline-First Systems and Mobile Money. If you work on this, please reach out.**