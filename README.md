🚀 SmartTutorAI – Personalized RAG-Based Learning Assistant

SmartTutorAI is a retrieval-augmented tutoring system designed to provide personalized explanations based on user-provided learning material.

The system adapts responses to user-selected learning levels and supports structured content retrieval for context-aware teaching.

🏗 System Architecture

SmartTutorAI follows a Retrieval-Augmented Generation (RAG) architecture:

User Input
→ Content Parsing
→ Embedding Generation
→ Vector Database Retrieval
→ Context Injection
→ LLM Response Generation

Core Components

1️⃣ Document Processing Layer

Parses unstructured content (videos, planned: PDFs, .txt)

Extracts metadata

Segments content into retrievable chunks

2️⃣ Embedding & Retrieval Layer

Generates vector embeddings

Stores them in ChromaDB

Performs similarity search for relevant knowledge chunks

3️⃣ Personalization Layer

Adjusts explanation depth based on user learning level

Supports structured response tuning (beginner → advanced)

4️⃣ Conversational Interface

Maintains dialogue context

Generates text-based explanations

Optional audio output (if implemented)

📊 Evaluation

• Internal testing achieved ~90% relevance in intent-to-response matching
• Retrieval quality evaluated using sample queries across varied content types
• Tested consistency across repeated prompts to ensure stable contextual grounding

🎯 Design Decisions

• RAG architecture selected to reduce hallucination risk and improve contextual grounding
• Vector search (ChromaDB) chosen for lightweight local experimentation
• Modular content pipeline designed to support future multi-format expansion

⚠ Limitations

• Current implementation primarily optimized for video-based content
• Limited domain specialization in present version
• Personalization logic rule-based (not yet adaptive via user feedback loop)

🔮 Roadmap (Future Enhancements)

• Multi-format document ingestion (PDF, .txt, slides)
• Domain-specific tutor specialization
• Adaptive feedback-driven personalization
• Cost-optimized smaller domain models
