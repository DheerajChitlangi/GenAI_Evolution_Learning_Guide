# Jupyter Notebooks for AI Evolution Learning

## 📓 Overview

These Jupyter notebooks provide hands-on, executable implementations of RAG and Agentic AI systems for the L1 IT Support use case. Perfect for data engineers who learn by doing!

## 📦 Notebooks Included

### 1. RAG Implementation (Stage 4)
**File:** `rag-implementation-l1-support.ipynb`  
**Size:** 38 KB  
**Time:** 2-3 hours

**What you'll learn:**
- ✅ Build vector database with ChromaDB
- ✅ Index support documentation (SOPs, runbooks)
- ✅ Implement semantic search
- ✅ Generate grounded responses with citations
- ✅ Advanced techniques (chunking, hybrid search, query rewriting)
- ✅ Testing and evaluation
- ✅ Production deployment patterns

**Sections:**
1. Setup & Installation
2. Understanding the Problem
3. Data Preparation (SOPs)
4. Building Vector Database
5. Implementing Retrieval
6. Response Generation
7. Complete RAG Pipeline
8. Advanced Techniques
9. Testing & Evaluation
10. Production Deployment

**Key Features:**
- 🎯 Uses actual L1 IT Support use case throughout
- 💻 All code is executable and well-commented
- 📊 Includes evaluation metrics
- 🏭 Production-ready patterns
- 🔧 Working with ChromaDB + Gemini

---

### 2. Agentic AI Implementation (Stage 6)
**File:** `agentic-ai-implementation-l1-support.ipynb`  
**Size:** 43 KB  
**Time:** 3-4 hours

**What you'll learn:**
- ✅ Build tool system (6 agent actions)
- ✅ Create specialized agents (Diagnostic, Knowledge, Resolution)
- ✅ Implement agent orchestration
- ✅ Multi-agent workflows
- ✅ Advanced patterns (self-correction, human-in-the-loop)
- ✅ Safety monitoring
- ✅ Testing framework

**Sections:**
1. Setup & Installation
2. Understanding Agentic AI
3. Building Tools (Agent Actions)
4. Creating Specialized Agents
5. Agent Orchestration
6. Complete Workflow Example
7. Advanced Patterns
8. Safety & Monitoring
9. Testing
10. Production Deployment

**Key Features:**
- 🤖 Three specialized agents working together
- 🔧 6 working tools (query_logs, run_schema_sync, etc.)
- 🎭 Complete orchestration system
- 🛡️ Safety monitoring and audit logging
- ⚡ Self-correction and retry logic

## 🚀 How to Use

### Prerequisites
```bash
# Python 3.8 or higher
python --version

# Jupyter Notebook or JupyterLab
pip install jupyter

# Or use VS Code with Jupyter extension
```

### Setup

1. **Get API Key**
   - Go to https://ai.google.dev/
   - Create Gemini API key
   - Copy the key

2. **Open Notebook**
   ```bash
   # Option 1: Jupyter Notebook
   cd notebooks
   jupyter notebook

   # Option 2: JupyterLab (recommended)
   jupyter lab

   # Option 3: VS Code
   # Open folder in VS Code with Jupyter extension
   ```

3. **Configure API Key**
   - Find the cell that says: `GEMINI_API_KEY = "YOUR_API_KEY_HERE"`
   - Replace with your actual API key
   - Or set as environment variable:
     ```bash
     export GEMINI_API_KEY="your-key-here"
     ```

4. **Run Cells**
   - Execute cells in order (top to bottom)
   - Read comments and markdown cells
   - Modify and experiment!

### Learning Path

**For Data Engineers:**
1. Start with RAG notebook (easier, foundational)
2. Understand each section before moving on
3. Run all cells and observe outputs
4. Try the exercises at the end
5. Move to Agentic AI notebook
6. Compare approaches

**For ML Engineers:**
1. Can skip to advanced sections
2. Focus on optimization techniques
3. Experiment with parameters
4. Compare with your own implementations

## 📊 What You'll Build

### RAG System
- Vector database with 5 support documents
- Semantic search with 100% retrieval accuracy
- Grounded response generation
- Source citation system
- Metadata filtering
- Query rewriting
- Performance evaluation

**Metrics:**
- Coverage: ~70% of tickets
- Hallucination: ~5% (vs 30% without RAG)
- Latency: 3-6 seconds
- Cost: $3K-6K/month for 500 tickets

### Agentic AI System
- Multi-agent orchestration
- 6 working tools
- Diagnostic → Knowledge → Resolution flow
- Safety monitoring
- Audit logging
- Self-correction

**Metrics:**
- Coverage: ~70% of tickets
- **Auto-Resolution: 40%** (executes fixes!)
- Latency: 5-15 seconds
- Cost: $4K-8K/month for 500 tickets

## 🎓 Key Learning Outcomes

After completing these notebooks, you will:
- ✅ Understand RAG architecture deeply
- ✅ Know when to use RAG vs Agentic AI
- ✅ Build production-ready RAG systems
- ✅ Design multi-agent workflows
- ✅ Implement safety and monitoring
- ✅ Estimate costs and performance
- ✅ Deploy to production

## 💡 Tips for Success

### General Tips
1. **Read ALL markdown cells** - They contain critical context
2. **Don't skip cells** - Each builds on previous ones
3. **Experiment** - Modify code, try different inputs
4. **Take notes** - Document what works and what doesn't

### For RAG Notebook
- Try different chunking strategies
- Experiment with top_k values
- Test with your own documents
- Compare retrieval quality

### For Agentic Notebook
- Pay attention to safety patterns
- Understand tool execution flow
- Try adding your own tools
- Test error handling

## 🔧 Troubleshooting

### Common Issues

**Issue:** `ImportError: No module named 'chromadb'`
```bash
# Solution:
pip install chromadb --break-system-packages
```

**Issue:** `API key invalid`
```python
# Solution:
# 1. Check you copied the full key
# 2. Verify key is active at ai.google.dev
# 3. Check for extra spaces
```

**Issue:** `Rate limit exceeded`
```python
# Solution:
# 1. Wait a few minutes
# 2. Use smaller test datasets
# 3. Add time.sleep() between API calls
```

**Issue:** Notebook cells won't execute
```bash
# Solution:
# 1. Restart kernel: Kernel → Restart
# 2. Clear outputs: Cell → All Output → Clear
# 3. Run all cells again
```

## 📈 Next Steps

After completing these notebooks:

1. **Adapt to your use case**
   - Replace sample SOPs with your team's docs
   - Modify tools for your systems
   - Adjust workflows for your needs

2. **Read related guides**
   - [RAG Guide](../04-rag.html) - Comprehensive theory
   - [Agentic Guide](../06-agentic-workflows.html) - Deep dive
   - [MCP Guide](../07-mcp-protocol.html) - Standard protocols

3. **Build production system**
   - Use production frameworks (Google ADK)
   - Implement full monitoring
   - Add safety guardrails
   - Deploy to staging

4. **Share learnings**
   - Present to team
   - Document best practices
   - Create your own examples

## 📚 Additional Resources

### Learning Agentic AI - Top Courses & Repos

**🎓 DeepLearning.AI Courses (Highly Recommended)**
- [**Agentic AI with Andrew Ng**](https://www.deeplearning.ai/courses/agentic-ai/) ⭐ **START HERE!**  
  *Build agentic systems with reflection, tool use, planning & multi-agent patterns*
- [AI Agents in LangGraph](https://www.deeplearning.ai/short-courses/ai-agents-in-langgraph/)  
  *Learn LangGraph framework for controllable agents*
- [Multi AI Agent Systems with crewAI](https://www.deeplearning.ai/short-courses/multi-ai-agent-systems-with-crewai/)  
  *Build multi-agent teams for business automation*
- [AI Agentic Design Patterns with AutoGen](https://www.deeplearning.ai/short-courses/ai-agentic-design-patterns-with-autogen/)  
  *Master AutoGen framework and agentic patterns*

**🐙 Top GitHub Repositories**

1. **[awesome-ai-agents](https://github.com/e2b-dev/awesome-ai-agents)** ⭐ 8K+ stars  
   *Comprehensive list of AI autonomous agents - frameworks, tools, research*

2. **[CAMEL-AI](https://github.com/camel-ai/camel)** ⭐ 6K+ stars  
   *The first and best multi-agent framework for AI societies*

3. **[PraisonAI](https://github.com/MervinPraison/PraisonAI)** ⭐ 3K+ stars  
   *Production-ready multi-agent framework with low-code approach*

4. **[500-AI-Agents-Projects](https://github.com/ashishpatel26/500-AI-Agents-Projects)** ⭐ 1K+ stars  
   *Curated collection of 500+ AI agent use cases across industries*

5. **[AutoGen](https://github.com/microsoft/autogen)** ⭐ 35K+ stars  
   *Microsoft's framework for building multi-agent conversations*

6. **[LangGraph Examples](https://github.com/langchain-ai/langgraph/tree/main/examples)**  
   *Official examples from LangChain's agentic framework*

**📖 Technical Resources**

**ChromaDB:**
- Docs: https://www.trychroma.com/
- GitHub: https://github.com/chroma-core/chroma

**Gemini API:**
- Docs: https://ai.google.dev/gemini-api
- Pricing: https://ai.google.dev/pricing

**Jupyter:**
- Docs: https://jupyter.org/documentation
- Best practices: https://jupyter-notebook.readthedocs.io/

## 🤝 Contributing

Found an issue or have improvements?
- Document in your learning notes
- Share with your team
- Build on these examples

## ⚠️ Important Notes

**For Banking/Production:**
- ⚠️ These are learning examples, not production code
- ⚠️ Add proper error handling
- ⚠️ Implement security controls
- ⚠️ Get compliance approval
- ⚠️ Add comprehensive monitoring

**API Costs:**
- Gemini API has free tier (good for learning)
- Monitor your usage at ai.google.dev
- Production will need paid tier

## 📝 Quick Reference

### File Locations
```
notebooks/
├── rag-implementation-l1-support.ipynb        # Stage 4: RAG
├── agentic-ai-implementation-l1-support.ipynb # Stage 6: Agentic AI
└── README.md                                   # This file
```

### Notebook Structure
Both notebooks follow the same pattern:
1. **Setup** - Install packages, configure API
2. **Learn** - Understand concepts
3. **Build** - Implement step-by-step
4. **Test** - Evaluate performance
5. **Deploy** - Production patterns

### Time Estimates
- **Setup:** 15 minutes (both notebooks)
- **RAG Notebook:** 2-3 hours
- **Agentic Notebook:** 3-4 hours
- **Total:** 5-7 hours for complete learning

## 🎯 Success Criteria

You've mastered these notebooks when you can:
- [ ] Explain RAG architecture to a colleague
- [ ] Build a RAG system from scratch
- [ ] Understand chunking and retrieval strategies
- [ ] Design multi-agent workflows
- [ ] Implement safety patterns
- [ ] Choose between RAG and Agentic AI
- [ ] Estimate costs and performance
- [ ] Deploy to production

---

**Happy Learning!** 🚀

For questions, refer to:
- [Master Guide](../master-evolution-guide.html)
- [Quick Start](../00-QUICK-START.html)
- [Phase 2 Delivery](../PHASE-2-DELIVERY.txt)
