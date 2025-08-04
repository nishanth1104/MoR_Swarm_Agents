# 🧠 MoR Swarm Agents: A Fusion of Mixture-of-Recursions & Modular Agent Delegation

This is a prototype implementation of **MoR Swarm Agents** — a novel framework that combines:

- Google's **Mixture-of-Recursions (MoR)**: a recursive, modular reasoning framework.
- **Swarm Multi-Agent Systems**: specialized agents that collaboratively solve complex tasks.

---

## 🚀 How It Works

- A **Coordinator Agent** receives any user query.
- It **recursively breaks down** the query into subtasks.
- Specialized agents — **MathAgent**, **LogicAgent**, **RetrievalAgent**, **LanguageAgent** — solve their parts.
- Final output is **reassembled** and returned.

### 🧪 Example Input

```
What is the capital of the country whose population is the square of 12?
```

### ✅ Sample Output

```
- Detected subtask: "square of 12" → 144
- Retrieval Agent: Country with population ≈144 million → Russia
- Final Answer: Capital of Russia → Moscow
```

---

## 🤖 Models Used

- [`microsoft/Phi-3-mini-4k-instruct`](https://huggingface.co/microsoft/Phi-3-mini-4k-instruct)
- Accessed via the Hugging Face Inference API using `transformers` and `InferenceApi`

> ⚠️ This model is slow on Colab. You can swap in lighter models or run locally for faster results.

---

## 🛠️ How to Run

1. Open the [Colab notebook](./MoR_Swarm_Agents.ipynb)
2. Set your Hugging Face API key.
3. Run all cells.
4. Enter any question — the coordinator agent will recursively delegate it to the right swarm members.

---

## 📚 Future Work

- Add memory or a scratchpad for more traceable reasoning
- Add dynamic agent routing based on task type
- Optimize runtime and support local GPU execution
- Possibly extend this into a full research paper with benchmarks

---

## 👤 Author

[Nishanth Ayyalasomayajula](www.linkedin.com/in/a-nishanth)
