🏙️ SmartCity-Islamabad: Data Structures in Urban Planning

SmartCity-Islamabad is a comprehensive urban simulation that models the rapid expansion of Pakistan's capital. By leveraging advanced data structures, the system optimizes transportation, manages administrative hierarchies, and streamlines healthcare and population services.

Note: This project is built using pure C++. No external libraries (like SFML) or STL were used for the core data structures, demonstrating deep, manual implementation of algorithmic concepts.

🚀 Key Features
🚌 Transport Sector (Graph-Based)
  Dynamic Routing: Models city stops as graph nodes and roads as weighted edges.
  Path Optimization: Implements a manual Dijkstra’s Algorithm to find the shortest path between    any two locations.
  Bus Tracking: Real-time lookup of buses by number using a polynomial rolling hash.
  
🏥 Medical & Emergency Sector (Priority-Driven)
  Emergency Bed Management: Uses a Binary Max-Heap to instantly rank hospitals based on bed        availability.
  Pharmacy Indexing: Rapid O(1) medicine search using a custom hash table with separate chaining.

🎓 Education & Administration (Hierarchical)
  City Hierarchy: Islamabad's sectors, streets, and houses are modeled using an N-ary Tree.
  School Organograms: A 3-level tree structure (School → Department → Class) manages academic      data.

👥 Population & Housing
  Citizen Registry: Secure and fast data retrieval for citizens via CNIC-based Hashing.
  Demographic Reports: Generates summaries of age distribution, gender ratios, and occupation      density.
  
🏗️ Data Structures Architecture

| Structure          | Logic Applied           | Real-world Use Case                |
| ------------------ | ----------------------- | ---------------------------------- |
|   Graph            | Adjacency List          | Road network & connectivity        |
|   N-ary Tree       | Arbitrary Child Nodes   | Islamabad administrative divisions |
|   Hash Table       | Separate Chaining       | `O(1)` lookup for CNIC & Medicines |
|   Min-Heap         | Array-based Binary Heap | Ranking nearest public facilities  |
|   Circular Queue   | Static Array            | Passenger handling simulation      |
|   Stack            | Linked List based       | User navigation/route history      |

🛠️ Technical Complexity Analysis

| Operation               | Implementation         | Time Complexity       |
| ----------------------- | ---------------------- | --------------------- |
|   Shortest Path         | Dijkstra (Custom Heap) | `O((V + E) log V)`    |
|   Citizen Search        | Hash Table (Manual)    | `O(1)` (Average Case) |
|   Hierarchy Traversal   | BFS/DFS (Tree)         | `O(N)`                |
|   Emergency Ranking     | Max-Heap Extract       | `O(log N)`            |


💻 Getting Started
Prerequisites:
  G++ Compiler (GCC
  Any C++ IDE (VS Code, CLion, or Dev-C++)

Installation:
# Clone the Repository
git clone https://github.com/your-username/SmartCity-Islamabad.git

# Navigate to Directory
cd SmartCity-Islamabad

# Compile
g++ main.cpp -o SmartCity

# Run
./SmartCity

📜 Academic Integrity & Design

  OOP Principles: Fully utilized Encapsulation, Abstraction, and Polymorphism.
  No Templates: Explicit type-handling to focus on memory management logic.
  Memory Management: Strictly monitored for leaks using manual destructors and pointer handling.

  
