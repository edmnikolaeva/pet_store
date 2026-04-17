# 🐾 SHOP MOBILE APP — API & Architecture Enhancement

<table> <tr> <td>
Developed the “Insurance” functionality for the mobile app, handling ~5,000 daily active users with ≤10s response time, enabling the business to quickly enter the growing pet insurance market, increase revenue, and prepare for scaling to additional types of pets
</td> <td width="220"> <img src="https://github.com/edmnikolaeva/pet_store/blob/main/project_logo.png" alt="Visual Anchor — C4 Model" width="200"/> </td> </tr> </table>

---

### 🧩 Key Artifacts
- [C4](https://github.com/edmnikolaeva/pet_store/blob/main/C4_lucky.jpg)
- [API Model](https://github.com/edmnikolaeva/pet_store/blob/main/моделирование_API_lucky.pdf)
- [API Specification](https://github.com/edmnikolaeva/pet_store/blob/main/api_lucky.yaml)

---

### 🧭 Business Context

- **Domain:** E-commerce Mobile App
- **Scope:** Implement new Insurance functionality in the existing mobile app
- **Stakeholders:** Client, end users, development team (6 pers)

---

**Goal:**
- Enable business to quickly test new market segment without additional UI forms
- Allow users to purchase insurance for pets
- Ensure fast response and support for internationalization (English)
 
---

**Key Pain Points**  
- Growing market demand for insurance, especially for dogs
- Users need a simple way to order insurance without filling additional forms  
- Existing microservices architecture must be updated to integrate new functionality

---

**MVP Solution**  
- New Insurance microservice created (MongoDB storage)
- API modeled to provide access to insurance products
- Users add insurance to existing shopping cart; further details handled by CRM operators
- Updated C4 model reflects new microservice and integration points
- Documentation created for development and testing teams

---

**Business Value**
- Quick market entry for growing pet insurance segment
- Potential revenue growth from new product line in LUCKY ecosystem
- Scalability: easily add new pet types and insurance options
- Risk reduction via integration with existing microservices and minimal system load
- Support for English version → international user reach

---

### ✅ Key Outcomes
- Architecture updated to support new Pet Insurance feature
- New REST API designed and implemented
- Pet Insurance feature delivered to production within 2 weeks
- Feature supports fast response (<10 seconds)

### ✅ Result / Impact (sample)
- Enabled first validation of insurance demand with minimal changes to existing flows  
- Zero additional load on Shipping service (no delivery for insurance)  
- Low expected load handled comfortably (~4–5 req/min, ~100 purchases/day)  
- Foundation created for future extensions (more pet types, detailed forms, etc.)

---

### 🔗 Requirements Traceability
- Traceability between business goals, requirements, architectural constraints, and integration points is maintained in:
- 👉 [Requirements traceability matrix](https://github.com/edmnikolaeva/pet_store/blob/main/requirements_traceability_matrix.pdf)

---

### ⚙️ Non-functional Requirements (examples)  
1. **Performance:** response time ≤ 10 seconds
2. **Throughput:** ~4–5 requests per minute on average (~5000 interested users / day) 
3. **Integration:** Kafka-based event to Shopping Cart service when adding to cart 
4. **Internationalization:** English version supported
   
---

### 🚨 Risks / Mitigations (examples)  
1. Low adoption of feature → MVP without heavy frontend forms, easy to turn off service  
2. Future requirements change → separate Insurance microservice (easy to extend or deprecate)  
3. Slow response from new service → strict 10s timeout, MongoDB for fast reads

---

### 🗓 Timeline / Delivery
- **Week 1:** Stakeholder interviews & architecture analysis 
- **Week 2:** API modeling, C4 update, Swagger specification, feature delivery to production 

---

### 👩‍💼 My Role
- Analyzed stakeholder interviews & existing microservices architecture  
- Defined user scenarios for Insurance 
- Updated existing microservices architecture (C4 Container level)  
- Designed high-level API profile (digital capabilities → operations)  
- Created formal OpenAPI 3.0 documentation in YAML  
- Supported fast feature delivery (2 weeks to production)

---

### 🛠 Tools / Tech Stack
- **Draw.io**: C4 model
- **Swagger Editor:** OpenAPI / YAML specification

---

## 🔄 Workflow

1. Collected and analyzed stakeholder input  
2. Reviewed existing microservices and integration points 
3. Defined functional requirements and user scenarios  
4. Developed [C4 Model](https://github.com/edmnikolaeva/pet_store/blob/main/C4_lucky.jpg) for the new feature  
5. Analyzed UI mockups  
6. Designed high-level modeling of [API profile](https://github.com/edmnikolaeva/pet_store/blob/main/моделирование_API_lucky.pdf) for Pet Insurance  
7. Created [openAPI specification](https://github.com/edmnikolaeva/pet_store/blob/main/api_lucky.yaml) in Swagger 
8. Delivered working feature to production  
