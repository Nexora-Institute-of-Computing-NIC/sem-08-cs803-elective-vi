# CS803 — Elective VI: Advanced Machine Learning — PLAN

**Semester:** 8 · **Credits:** 3 · **Level:** Professional
**Theory:** 45 hrs · **Lab:** 15 hrs · **Tools:** Python, PyTorch, Hugging Face, vLLM, LangChain, Weights & Biases, Docker

## Syllabus

### Unit 1 — Large Language Models (9 lectures)
1. From transformers to LLMs — a recap
2. Pretraining objectives — causal vs masked
3. Scaling laws — how model size, data, and compute trade off
4. Tokenisation — BPE, SentencePiece, vocabulary
5. Context length — attention's quadratic cost and its workarounds
6. Instruction tuning and supervised fine-tuning
7. RLHF — reward models and policy optimisation
8. Direct Preference Optimisation (DPO) and its variants
9. Evaluating LLMs — benchmarks, contamination, human evals

### Unit 2 — Parameter-Efficient Fine-Tuning and Serving (9 lectures)
1. Why full fine-tuning is often infeasible
2. LoRA and QLoRA — low-rank adaptation
3. Prefix tuning and prompt tuning
4. Adapters and IA3
5. Merging adapters and deploying a fine-tuned model
6. Quantisation — INT8, INT4, GPTQ, AWQ
7. Efficient inference — KV cache, continuous batching, vLLM
8. Serving infrastructure — latency vs throughput, autoscaling
9. Cost engineering — tokens per dollar, caching, routing

### Unit 3 — Multimodal Models (9 lectures)
1. Why multimodal — beyond text
2. Vision-language models — CLIP, BLIP, LLaVA
3. Image-text contrastive training
4. Visual instruction tuning
5. Audio models — speech recognition and synthesis
6. Video understanding (overview)
7. Multimodal RAG — retrieval across modalities
8. Evaluation of multimodal models
9. Applications — document AI, accessibility, creative tools

### Unit 4 — MLOps and Production ML (9 lectures)
1. What MLOps is — the gap between notebook and production
2. Experiment tracking — W&B, MLflow
3. Feature stores — Feast, Tecton (overview)
4. Model versioning and registries
5. Data versioning — DVC, lakeFS
6. CI/CD for ML — testing data, models, and predictions
7. Monitoring — drift, skew, concept change
8. Retraining policies — scheduled vs triggered
9. Incident response for ML systems

### Unit 5 — Responsible and Applied ML (9 lectures)
1. Bias in large models — sources and evaluation
2. Fairness metrics and trade-offs
3. Interpretability — attention, saliency, SHAP for deep models
4. Hallucination — detection, grounding, RAG
5. Safety — red teaming, guardrails, moderation
6. Privacy — differential privacy, membership inference
7. Regulatory landscape — EU AI Act, India DPDP
8. Applied case studies — what actually shipped
9. The frontier — agents, tool use, reasoning models

## Practical Labs (15)

1. Fine-tune a small LLM (e.g. Llama-3-8B or Phi-3) with LoRA on a small dataset
2. QLoRA — fine-tune a 7B model on a single consumer GPU
3. Evaluate a fine-tuned model vs base on a held-out set
4. Merge a LoRA adapter and export a deployable model
5. Quantise the merged model to INT4 and measure quality vs speed
6. Serve the model with vLLM and benchmark throughput
7. Build a RAG pipeline — embed, retrieve, generate
8. Evaluate the RAG pipeline — faithfulness, relevance
9. Fine-tune CLIP on a custom image-text dataset
10. Use LLaVA for visual question answering
11. Set up W&B experiment tracking for a fine-tuning run
12. DVC — version a dataset and a model
13. Build a monitoring dashboard — track drift on a live model
14. Red-team your own model — find 5 failure modes and mitigate
15. Final project — an end-to-end advanced ML system with report

## Assignments

1. LLM evaluation report — benchmark and analyse three models
2. Fine-tuning report — LoRA vs QLoRA vs full fine-tuning on the same task
3. Multimodal application — a working demo with evaluation
4. MLOps report — instrument one model end to end
5. Final project — a complete advanced ML system with ethics section
