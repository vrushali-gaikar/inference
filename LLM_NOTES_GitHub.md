# LLM NOTES

## 1. Frozen Weights

Frozen weights are model parameters (weights and biases) in a machine learning or deep learning network that are locked in place and not updated during training.

### Key Points

- **Transfer Learning:** When adapting a pre-trained model to a new, smaller dataset, early layers are often frozen because they capture universal patterns like basic edges and textures.
- **Speed and Compute:** Locking layers cuts down on memory use and speeds up training because fewer gradients need to be computed.
- **Preventing Overfitting:** Keeping foundational feature-extractors locked stops the model from ruining already-learned representations when training on limited new data.

### Example

`ResNet-50 Base Layers → New Classification Head → Prediction`

**Frozen Weights → Trainable Weights**

---

## 2. Context Window

A context window in artificial intelligence is the maximum amount of information—measured in tokens—that a Large Language Model (LLM) can hold and reference at any single time.

- Includes the prompt, conversation history, and retrieved context.
- Input and generated output must fit within the model’s token limits.
- Capacity is measured in tokens.

### Example

A student uploads a 100-page textbook and asks questions about it. The context window limits how much text the model can process at once.

`Prompt + History + Retrieved Context → Context Window → Output`

### LLM Context Window Allocation & Capacity Limit

---

## 3. External Knowledge

External knowledge in Large Language Models (LLMs) refers to any information, data, or documents not encoded inside the model's neural network weights (parametric memory) that is supplied to the model at inference time.

- Provides updated or domain-specific information.
- **RAG** retrieves relevant information and adds it to the prompt without retraining the LLM.

### Example

A college chatbot retrieves an exam timetable from a PDF or database to answer a student’s question about exam dates.

`Documents → Retriever → Relevant Context + Query → LLM → Answer`

---

## Handwritten Note

