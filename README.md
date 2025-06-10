# OPTIMIZATION MODEL

**Company**: CODTECH IT SOLUTIONS  
**Name**: Jonna Nikhil  
**Intern ID**: CT04DF1123  
**Domain**: Data Science  
**Duration**: 4 Weeks  
**Mentor**: Neela Santhosh  

---

## 📌 Objective

To solve a logistics optimization problem using **Linear Programming (LP)** with Python’s `PuLP` library. The goal is to **minimize total transportation cost** from multiple warehouses to customer locations while satisfying customer demand and not exceeding warehouse capacity.

---

Project Description: In this project, we solve a logistics optimization problem for a delivery company aiming to minimize transportation costs while ensuring all customer demands are met. The business has multiple warehouses and delivery locations, each with specific supply and demand values. 

---

## 📦 Dataset Description
We modeled the supply chain of a logistics company with:

- **2 Warehouses**: `W1`, `W2`
- **3 Customer Locations**: `C1`, `C2`, `C3`
- Each warehouse has a **fixed supply**
- Each customer has a **fixed demand**
- A **cost matrix** defines the cost per unit for each route (Warehouse → Customer)

---

## 🧮 Optimization Formulation

- **Decision Variables**: `x[i][j]` = number of units shipped from warehouse `i` to customer `j`
- **Objective Function**:  
  Minimize total cost = ∑ (cost[i][j] × x[i][j])
- **Constraints**:
  - Shipments from a warehouse cannot exceed its supply
  - Each customer’s demand must be fully met

---

The model includes constraints to ensure:

Supplies are not exceeded at warehouses

Demands are fulfilled at customer locations

Route costs are respected

Once solved, the notebook presents:

Optimal delivery routes 

Total minimum cost

Resource allocation

Business insights for strategic planning

Key Concepts Covered: Objective function formulation

Constraint modeling

Solving LP using PuLP

Business interpretation of the result

## 🛠 Libraries Used

- `pulp`
- `pandas`

---

## 💻 Output

```
Status: Optimal

Optimal Routes and Quantities:
W1 -> C1: 0.0 units
W1 -> C2: 0.0 units
W1 -> C3: 100.0 units
W2 -> C1: 80.0 units
W2 -> C2: 70.0 units
W2 -> C3: 0.0 units

Total Minimum Transportation Cost: ₹810.0
```

---

A simple diagram showing warehouse-to-customer flow based on our optimization output.

visual plot of optimized delivery routes is ready:


---
## 📊 Business Insights

- 🧠 Warehouse **W2** should handle all deliveries to **C1** and **C2**, utilizing its full capacity.
- 📦 Warehouse **W1** is best used for fulfilling all demand to **C3**.
- ✅ This route configuration **minimizes total delivery cost** to ₹810.
- 🚛 Optimized logistics planning can reduce operational costs and improve supply chain efficiency.

---

## ✅ Conclusion

This project fulfills the internship requirement for **Task 4 – Optimization Model** by:
- Formulating a real-world logistics problem
- Modeling constraints and objective function using Linear Programming
- Solving with Python’s `PuLP` and interpreting the optimal strategy

The solution offers a practical decision-making tool for logistics cost savings.

---
