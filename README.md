# AI vs ML vs Deep Learning

A simple comparison of Artificial Intelligence (AI), Machine Learning (ML), and Deep Learning (DL), covering definitions, differences, real-world examples, and how they relate.

## Definitions

- **Artificial Intelligence (AI)** is the broad field of building machines that perform tasks that normally need human intelligence, such as reasoning, planning, language, and perception.
- **Machine Learning (ML)** is a subset of AI in which a system learns patterns from data instead of following hand-written rules.
- **Deep Learning (DL)** is a subset of ML that uses neural networks with many layers to learn complex patterns, especially from images, audio, and text.

## Comparison

| | AI | Machine Learning | Deep Learning |
|---|---|---|---|
| Scope | Broadest field | Subset of AI | Subset of ML |
| How it works | Rules, search, learning, or a mix | Learns patterns from data using algorithms such as decision trees or linear models | Learns features automatically with multi-layer neural networks |
| Data needs | Varies | Moderate | Large amounts of data |
| Compute needs | Varies | Usually modest | Usually high (GPUs) |
| Feature engineering | Varies | Often done by hand | Largely automatic |
| Interpretability | Varies | Often easier to explain | Harder to explain |

## Real-world examples

- **AI:** a chess engine that plans moves, or a customer-support chatbot that routes questions.
- **Machine Learning:** a spam filter that learns from labelled emails, or a model that predicts house prices from past sales.
- **Deep Learning:** image recognition that tags faces in photos, or speech recognition in a voice assistant.

## How they are related

Think of them as nested circles. AI is the largest circle. Machine Learning sits inside AI, because it is one of the main ways to build AI systems. Deep Learning sits inside Machine Learning, because it is one specific family of ML methods that relies on neural networks.

Recommendation systems are a good example that touches all three: the overall product is AI, a model that learns user preferences from past behaviour is ML, and a deep neural network that learns from raw images or text to match products is DL.

## Tools

- Python
- Jupyter Notebook
- Markdown

## Deliverables

- A comparison table (above)
- Real-world examples of AI, ML, and Deep Learning (above)
- A short explanation of how they are related (above)

## Deployment

Platform: Vercel (production, team `shreyas-sarkar-s-projects`, project `ai-ml-dl-comparison`).

Live URL: https://ai-ml-dl-comparison.vercel.app

Configuration: `vercel.json` sets `"cleanUrls": true` and `"outputDirectory": "public"`. The site is a single static page at `public/index.html`.

Steps:
1. Put `public/index.html` and `vercel.json` in the project folder.
2. Create a deployment with the Vercel API (`create_deployment`, target `production`, `outputDirectory` set to `public`). The first deployment was `dpl_Hb7gMh9JN2q2WfESYoDbX7aeDCtY` and reached READY in about 5 seconds.

## Rollback evidence

1. Version 1 was deployed as `dpl_Hb7gMh9JN2q2WfESYoDbX7aeDCtY` (READY, 24 Nov 2026).
2. A second deployment, `dpl_ELsJA7ZKro7zq2oAAJSgEAtArkpu`, was made with a visible change ("Version 2" line) and went READY.
3. A rollback to `dpl_Hb7gMh9JN2q2WfESYoDbX7aeDCtY` was requested with `request_rollback`, with the reason "restoring version 1 after testing version 2".
4. Checked afterwards: https://ai-ml-dl-comparison.vercel.app returns the version 1 page with no "Version 2" line, so the rollback is confirmed.
