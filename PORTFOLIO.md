# Portfolio guide

Suggested reading order for technical reviewers. Links below point only to public repositories.

## 1. FlowMedic AI — automation operations

[Repository](https://github.com/engdareenbassamesleem/flowmedic-ai)

Start with app/services/health.py for deterministic classification, then app/integrations/n8n/client.py for integration boundaries. The repository also includes persistence, migrations, tests and a Next.js dashboard. Follow its README to run the synthetic demo without credentials.

## 2. RAGSource — document question answering

[Repository](https://github.com/engdareenbassamesleem/ragsource)

Start with src/ragsource/service.py for retrieval orchestration, then the ingestion, embedding and store modules. Review source metadata and the low-retrieval no-answer path. The first actual embedding run requires a model download; tests use fakes.

## 3. Resume Evidence — text matching and explainability

[Repository](https://github.com/engdareenbassamesleem/ai-resume-analyzer)

Run python app.py. The synthetic example returns 62.5% explicit mention coverage. Inspect analyzer.py and tests/test_analyzer.py for aliases, boundaries and unknown results. Negated mentions and optional requirements need human interpretation.

## 4. SourceDesk — information retrieval fundamentals

[Repository](https://github.com/engdareenbassamesleem/AI-Chatbot-WebApp)

Run python app.py. Inspect retrieval.py for BM25 term weighting and source-preserving results. Try both a known FAQ and an unrelated question. This is lexical FAQ retrieval, not a generative chatbot.

## 5. Dentivo AI — application prototype

[Repository](https://github.com/engdareenbassamesleem/dentivo-ai)

React dashboard, Firebase services and Gemini assistant. Review the setup and local-demo limitations before using external credentials or real data.

## 6. Frontend studies

- [GoldCalcPro](https://github.com/engdareenbassamesleem/gold-calcpro): a calculator interface with fixed demo currency factors.
- [Skincare landing page](https://github.com/engdareenbassamesleem/-COSRX-Snail-Mucin-Repairing-Serum-landing-page): component-based product presentation.
- [Git learning exercise](https://github.com/engdareenbassamesleem/GitHub-): introductory Git practice, not a standalone product.

## Interview preparation

For each featured project, be ready to explain the problem, trace one input through the code, run one test, identify a limitation and make a small change yourself. When describing AI-assisted work, distinguish generated scaffolding from your own decisions, testing and modifications.
