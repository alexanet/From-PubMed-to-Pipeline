# From-PubMed-to-Pipeline
# From PubMed to Pipeline: Automated Scientific Insight Extraction using LLM

In today’s fast-paced research, staying ahead means making sense of an ever-growing ocean of scientific literature. Every day, thousands of new biomedical papers are published, but extracting actionable insights from them remains a massive bottleneck, especially when time and resources are limited.

To tackle this challenge, I recently built a personal project that automates the journey “From PubMed to Pipeline” — leveraging Large Language Models (LLMs) to transform unstructured scientific abstracts into clear, structured knowledge that can drive R&D decisions.

## Steps of the Project:


<img width="536" height="285" alt="Screenshot 2025-08-11 at 11 27 46" src="https://github.com/user-attachments/assets/9bae7366-bef4-4240-b683-da66f23ff2f5" />

1. Automated Data Retrieval Using PubMed’s API, I programmed a pipeline to fetch relevant biomedical abstracts at scale. This step replaces tedious manual searches with an automated and reproducible process.
2. Extracting Key Scientific Relations with LLMs The core innovation is applying LLMs to extract meaningful relationships between drugs, targets, biomarkers, and diseases directly from text. Instead of relying on complex rule-based NLP, the models interpret context, enabling high-precision extraction of evidence-based relations.
   
<img width="714" height="400" alt="Screenshot 2025-08-11 at 11 28 47" src="https://github.com/user-attachments/assets/ea3b2d67-e6aa-4a11-acae-a3e4cd7fa606" />

3. Summarizing Complex Information Raw data can overwhelm, so I incorporated LLM-powered summarization to generate concise insights that highlight what’s important.

<img width="726" height="177" alt="Screenshot 2025-08-11 at 11 29 53" src="https://github.com/user-attachments/assets/3a6e90cd-9ecd-4a61-8dd2-366e35b5a0f0" />

4. Connecting Insights to Internal Pharma Assets To maximize practical value, we could integrate a matching layer that links extracted scientific entities to internal R&D programs and assets, helping identify strategic opportunities and guide portfolio prioritization. (optional: out of scope of this current work)

5. Building an Interactive Dashboard Finally, I developed a user-friendly Gradio web interface that allows exploration of the extracted knowledge base through simple search and visualization. This makes AI-generated insights actionable and approachable for various stakeholders.

<img width="760" height="467" alt="Screenshot 2025-08-11 at 11 30 20" src="https://github.com/user-attachments/assets/39f17cab-3b69-4d7a-999d-acbf598181f7" />


## Why It Matters
Speed & Scale: Automating literature mining enables teams to quickly keep up with scientific advances — a task that would be impossible to achieve manually.

Data-Driven Decisions: We can enable smarter, faster R&D prioritisation by turning unstructured text into structured, summarised insights.

Cross-Functional Impact: The dashboard promotes collaboration between data scientists, scientists, and decision-makers, breaking down silos.

“Published studies on systematic reviews indicate that manual abstract screening can be time-intensive. For example, Wallace et al. (2013) reported that experienced reviewers can process biomedical abstracts at rates ranging from roughly 30 to 70 per hour, depending on complexity and inclusion criteria. At this pace, reviewing 100+ abstracts may require 1.5–3+ hours, and often more when accounting for preparation, note-taking, and quality checks."

In my prototype pipeline, the same volume was processed in ~1 hour, including automated summarization and relation extraction, suggesting potential for substantial time savings in the screening stage.

<img width="456" height="360" alt="Screenshot 2025-08-11 at 11 34 13" src="https://github.com/user-attachments/assets/da661de7-e88c-4bdd-b6b3-7c661ee927d5" />

### Referances 
- Hugging Face Transformers – Wolf, T., et al. (2020). “Transformers: State-of-the-Art Natural Language Processing.” Proceedings of the 2020 Conference on Empirical Methods in Natural Language Processing: System Demonstrations, 38–45. https://huggingface.co/docs/transformers
- Meta AI – LLaMA 2 – Touvron, H., et al. (2023). LLaMA 2: Open Foundation and Fine-Tuned Chat Models. arXiv:2307.09288.https://huggingface.co/meta-llama/Llama-2-7b-chat-hf
- PubMed / Entrez Programming Utilities (E-utilities) – NCBI. “Entrez Programming Utilities Help.” https://www.ncbi.nlm.nih.gov/books/NBK25501/
- Gradio – Abid, A., et al. (2019). “Gradio: Hassle-Free Sharing and Testing of ML Models.” arXiv preprint arXiv:1906.02569. https://www.gradio.app
- FAISS – Johnson, J., Douze, M., & Jégou, H. (2019). “Billion-scale similarity search with GPUs.” IEEE Transactions on Big Data. https://github.com/facebookresearch/faiss
- Boudin et al., 2010 – Boudin, F., Nie, J.Y., Bartlett, J.C., Grad, R., Pluye, P., Dawes, M. “Combining classifiers for robust PICO element detection.” Journal of Biomedical Informatics, 43(5), 757–765. https://doi.org/10.1016/j.jbi.2010.06.005
- Wallace et al., 2013, “Automated screening for systematic reviews” — reports that reviewing 120 abstracts can take 4–8 hours manually for experienced reviewers.DOI: 10.1186/2046-4053-2-80
- PubMed – National Library of Medicine. “PubMed Overview.” https://pubmed.ncbi.nlm.nih.gov/
- NCBI MeSH Vocabulary – Lipscomb, C.E. “Medical Subject Headings (MeSH).” Bulletin of the Medical Library Association, 88(3), 265–266. https://www.nlm.nih.gov/mesh/meshhome.html
