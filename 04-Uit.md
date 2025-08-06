# 🧠 UNIT 4: Genetic Algorithms & Evolutionary Computing – Exam-Ready Answers

---

## 🔹 Q1. Traditional Algorithms vs Genetic Algorithms

| Feature                  | Traditional Algorithms        | Genetic Algorithms (GA)         |
|--------------------------|-------------------------------|----------------------------------|
| Nature                   | Deterministic                 | Probabilistic (randomness)       |
| Approach                 | Step-by-step instructions     | Inspired by natural evolution    |
| Solution Search          | Single best solution          | Population-based search          |
| Adaptability             | Less adaptive                 | Highly adaptive                  |
| Memory/State             | Static                        | Evolves & learns                 |

### 🧠 Summary:
Genetic algorithms (GA) use **evolution concepts** (jaise DNA, selection, mutation) to find solutions — especially for problems jaha fixed steps nahi chalti (e.g., scheduling, optimization, AI).

---

## 🔹 Q2. Genetic Operations

Genetic Algorithm me 3 main operations hote hain:

### 1️⃣ Selection:
- Best solutions (parents) select karte hain next generation ke liye
- Aim: Achhe genes pass hone chahiye

### 2️⃣ Crossover:
- Do parents ke parts exchange hote hain to create new offspring
- Example:
  - Parent1: 101100
  - Parent2: 110010
  - Crossover → 101010

### 3️⃣ Mutation:
- Random change in child
- Purpose: Diversity maintain karna
- Example: 101010 → 100010

---

## 🔹 Q3. What is Fitness Function?

Fitness function decide karta hai ki **solution kitna acha hai**.

- High fitness = better solution
- GA tries to improve fitness over generations

### 📦 Example (Hindi Style):
Agar tumhare pass ek timetable banana hai aur koi schedule sab teachers ko match karta hai → uska fitness high hoga.  
Agar clash ho → fitness low.

---

## 🔹 Q4. Selection Mechanisms in GA

### 1️⃣ Roulette Wheel Selection:
- Probability based on fitness
- High fitness = more chance
- Example: Jaise lottery draw jisme higher fitness wale ke naam zyada baar likhe gaye ho

### 2️⃣ Tournament Selection:
- Random group bana ke best select
- Example: 4 solutions me se best choose

### 3️⃣ Rank Selection:
- Solutions ko rank diya jata hai, not actual fitness
- Smooth selection chance milta hai sabko

### 4️⃣ Elitism:
- Best solution(s) directly next generation me bhej dete hain
- Quality guarantee karta hai

---

## 🔹 Q5. Types of Crossover & Mutation Techniques

### 🔁 Crossover Types:
| Type             | Description |
|------------------|-------------|
| Single Point     | Ek point pe cut |
| Two Point        | Do points pe cut |
| Uniform          | Har bit randomly choose |

### 🔁 Mutation Types:
| Type              | Description |
|-------------------|-------------|
| Bit Flip          | 0 → 1 or 1 → 0 |
| Swap              | Do values swap kar do |
| Scramble          | Random rearrangement |
| Inversion         | Sub-segment ulta karna |

---

## 📌 Short Notes

### 📎 Swarm Intelligence:

Swarm Intelligence inspired hoti hai **ants, birds, bees** jaise insects ke group behavior se.

- Local rules follow karke group global solution find karta hai
- Example Algorithms:
  - Ant Colony Optimization (ACO)
  - Particle Swarm Optimization (PSO)

### 🔧 Real Life Example:
- Google Maps: traffic-based routing (many users ka data consider karke best path)
- Robotics: multiple bots coordinate karte hain without central control

---

