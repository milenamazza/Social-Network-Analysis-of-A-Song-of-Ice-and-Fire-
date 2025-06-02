# **Social Network Analysis of "A Song of Ice and Fire"**  
*A Network Science Exploration of George R.R. Martin's Epic Fantasy Saga*  

---

## **📖 Project Overview**  
This study applies **Social Network Analysis (SNA)** to George R.R. Martin's *A Song of Ice and Fire* series, uncovering the hidden structures of power, influence, and narrative cohesion in Westeros. By modeling character interactions as a network, we identify:  
✔ **Key leaders** (Tyrion, Jon Snow, Daenerys)  
✔ **Hidden influencers** (Olenna Tyrell, Mandon Moore)  
✔ **Critical mediators** bridging factions  
✔ **Community structures** (Houses Stark, Lannister, Targaryen)  
✔ **Epidemic spread dynamics** (simulating plagues & pandemics)  

**Dataset**: 796 characters (nodes) and 2,823 interactions (edges) from the first five books.  

---

## **🔍 Key Findings**  

### **1. Global Network Structure**  
- **Scale-free network** (few highly connected hubs, many peripheral characters)  
- **Small-world properties**: Short average path length (3.42) despite sparse density (0.0089)  
- **Core-periphery structure**: Dense central cluster (Tyrion, Jon, Cersei) drives the narrative  
- **109 articulation points** (e.g., Jon Snow's removal would split the network into 5+ fragments)  

### **2. Character Centrality & Influence**  
| **Metric**               | **Top Characters**               | **Key Insight** |
|--------------------------|----------------------------------|----------------|
| **Degree Centrality**    | Tyrion (122), Jon Snow (114)     | Most visible leaders |
| **PageRank**            | Jon Snow (0.019), Tyrion (0.018) | Narrative influence beyond direct ties |
| **Betweenness**         | Jon Snow (0.192), Tyrion (0.162) | Critical mediators between factions |
| **Hidden Leaders**      | Olenna Tyrell, Mandon Moore      | Low visibility but high strategic connections |

### **3. Houses & Communities**  
- **House Stark** = Most cohesive (intra-density 0.50)  
- **House Lannister** = Most politically connected (31 edges to House Stark)  
- **19 Louvain communities** detected, with Tyrion bridging 10+ groups  

### **4. Epidemic Simulations**  
Modeled two disease scenarios:  
- **COVID-19-like**: High spread, low mortality (infected 50%+ nodes)  
- **Black Plague-like**: Lower spread, high mortality (killed 55% of infected)  
🔹 **Robert Baratheon** = Worst superspreader (411 infections avg.)  
🔹 **Jon Snow** = Highest recovery rate (605 cured)  

---

## **📊 Visualizations (See Appendix)**  
- **Network graphs** colored by House/community (Figs. 14–19)  
- **Centrality distributions** (Fig. 20)  
- **Epidemic simulations** (Figs. 21–26)  

---

## **⚖️ Limitations**  
1. **Data constraints**: Interactions based on name co-occurrence (15-word window)  
2. **Undirected edges**: Misses power asymmetries (e.g., commands vs. alliances)  
3. **Static analysis**: Ignores temporal dynamics (e.g., character deaths)  

---

## **📂 Repository Contents**  
- **`SNA.pdf`**: Full analysis (metrics, methodology, results)  
- **`/plots`**: Network visualizations & epidemic simulations  
- **Datasets**: Character interactions (CSV/JSON)  

---

## **👥 Authors**  
Arianna Arruzzoli, Benedetta Bottari, Claudia Brunetti, Milena Mazza  
*University of Bologna, Computer Science*  

🔗 **License**: CC BY-NC-SA 4.0  
📜 **Full Report**: `SNA.pdf`
