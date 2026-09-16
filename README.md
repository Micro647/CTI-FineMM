# CTI-FineMM: An Information-Theoretic Visual Extraction Pipeline and Fine-Grained, High-Density Visual Benchmark for Cyber Threat Intelligence

#Intro:

With the continuous escalation of cyberattacks, the volume of Cyber Threat Intelligence (CTI) has grown exponentially, making the extraction of high-value information a critical factor in enhancing Advanced Persistent Threat (APT) attribution capabilities. Existing automated processing pipelines suffer from significant modality deficiencies, often overlooking visual content that encapsulates high-density semantics. Although Multimodal Large Language Models (MLLMs) present new opportunities to address this issue, current research remains severely constrained by the scarcity of high-quality, visually-grounded corpora in the CTI domain. Moreover, large-scale image extraction from massive volumes of unstructured PDFs incurs extremely high computational complexity and is plagued by severe noise from low-quality images.
To address this dual bottleneck of computational resources and data scarcity, the core contribution of this paper is the design of an efficient heuristic extraction pipeline and the subsequent construction and open-source release of CTI-FineMM, a high-quality visual image dataset. At the algorithmic level, this work departs from conventional OCR-based approaches and full-page rendering, both of which incur high latency and substantial resource consumption. Instead, we introduce an early-exit filtering mechanism grounded in pixel-level variance and Shannon entropy, which enables the rapid discarding of low-information noisy images in constant time, thereby ensuring exceptionally high throughput while drastically reducing computational overhead. At the data level, empirical analysis of the constructed corpus demonstrates that, owing to the rigorous filtering enabled by the proposed algorithm, CTI-FineMM successfully eliminates redundant visual noise and retains high-value images that carry rich semantics and directly reveal attacker Tactics, Techniques, and Procedures (TTPs). Theoretical complexity analysis further confirms that the proposed extraction pipeline effectively circumvents the I/O bottlenecks inherent in traditional methods, exhibiting superior scalability. This study not only delivers a highly valuable visual benchmark dataset for CTI but also establishes a low-computation paradigm for large-scale domain-specific data cleaning, providing critical foundational support for advancing data-centric cybersecurity AI research.







```
