# Used Sources

Only sources that are actually used and cited in `literature_review.md` should be recorded here.

## Source 1

### Full citation

Agrawal, S., Jamadar, S., Sawant, S., Bidwe, R. V., & Joshi, A. (2025). Optimization of road route alignment: a systematic literature review with meta analysis. *Artificial Intelligence Review, 58*, Article 384. https://doi.org/10.1007/s10462-025-11396-3

### Aim

To systematically review research on road route alignment optimization and identify major methods, trends, and research gaps, with particular attention to GIS, deep learning, multi-criteria decision-making, and route optimization techniques.

### Method

Systematic literature review using a PRISMA-based process. The study screened 370 papers, selected 132 through full-text review, and added 25 through snowball sampling, for a total of 157 records analysed.

### Findings

The review found that deep learning is increasingly used to improve land use and land cover classification, while multi-criteria decision-making methods help incorporate environmental, social, economic, and engineering factors into route selection. It also proposed a generalized framework combining problem definition, criteria selection, data preparation, deep learning-based classification, MCDM, and least-cost path analysis.

### Relevance to road design

This is one of the strongest overview sources for the road-design part of the review because it directly addresses road route alignment and maps the current state of AI-related approaches in that domain.

### Relevance to AI workflow

It is useful for showing how AI can support an integrated workflow rather than a single isolated task, especially by connecting data preparation, classification, decision support, and route optimisation.

### Limitations

As a review paper, it does not test a new design model itself. Its focus is mainly on route alignment and optimization, so it does not fully cover broader road design tasks such as detailed geometric design, drainage, documentation, or AI-assisted explanation writing.

---

## Source 2

### Full citation

Kang, M.-W., Jha, M. K., & Schonfeld, P. (2012). Applicability of highway alignment optimization models. *Transportation Research Part C: Emerging Technologies, 21*(1), 257-286. https://doi.org/10.1016/j.trc.2011.09.006

### Aim

To develop and test an intelligent optimization tool that helps planners and designers identify preferable highway alignments across complex terrain and land-use conditions.

### Method

Model-development and case-study research. The paper integrates genetic algorithms with a geographic information system (GIS), then evaluates the model using two real highway projects in Maryland and sensitivity analysis of major parameters.

### Findings

The study found that the model could effectively optimize highway alignments, generate outputs comparable to conventional manual methods, reduce planning and design time, and produce lower-cost solutions. It also showed that multiple dominant and alignment-sensitive costs need to be evaluated together because important trade-offs exist among them.

### Relevance to road design

This source is directly relevant because it focuses on highway alignment optimization, a core road design task. It provides concrete evidence that AI-style optimization methods were already being applied in road design before current generative AI tools.

### Relevance to AI workflow

It supports the idea that AI can assist engineering workflow by processing large amounts of design and evaluation data, comparing alternatives, and improving decision support in planning and design stages.

### Limitations

The paper focuses on alignment optimization rather than full end-to-end road design automation. It also reflects an earlier optimization-based AI approach, so it does not address newer generative AI capabilities such as explanation writing, knowledge linking, or conversational design support.

---

## Source 3

### Full citation

Daareyni, A., Martikkala, A., Mokhtarian, H., & Flores Ituarte, I. (2025). Generative AI meets CAD: enhancing engineering design to manufacturing processes with large language models. *The International Journal of Advanced Manufacturing Technology*. https://doi.org/10.1007/s00170-025-15830-2

### Aim

To investigate how large language models can support engineering design by translating multimodal user inputs into CAD models and connecting design generation to manufacturing workflows.

### Method

Framework-development and validation study. The authors built a Python- and Streamlit-based generative AI-assisted design system using LLMs, OpenSCAD, computer vision, and multiple feedback loops, then tested it across several 3D generation tasks and a gear-system case study.

### Findings

The study showed that the system could generate CAD models from text and visual inputs, refine results through internal and user feedback loops, and support a design-to-manufacturing workflow. It also found that the approach could work with incomplete inputs, although dimensional precision, complex geometry handling, and execution efficiency remained important challenges.

### Relevance to road design

This source is not about road design specifically, but it is highly relevant conceptually because it shows how AI can transform basic user requirements into technical design outputs through an iterative workflow. That idea is closely related to the long-term goal of automating road design from basic input information.

### Relevance to AI workflow

This is a strong source for the workflow side of the review because it demonstrates how AI can connect requirements, engineering reasoning, model generation, feedback, and final outputs within one design process.

### Limitations

The paper is based in CAD and manufacturing rather than civil or road engineering, so transfer to road design is indirect. It also reports ongoing limitations in geometric accuracy, detail fidelity, and model efficiency, which are important when considering engineering-grade design applications.

---

## Source 4

### Full citation

Naser, M. Z., Tapeh, A. T. G., & Abdalla, J. (2025). A review of generative artificial intelligence in civil and environmental engineering. *Machine Learning for Computational Science and Engineering, 1*, Article 42. https://doi.org/10.1007/s44379-025-00041-z

### Aim

To review the current state of generative artificial intelligence in civil and environmental engineering, identify the most commonly used models and application areas, and highlight barriers to adoption and future research directions.

### Method

Scientometric literature review. The study maps publication trends, model families, application domains, packages, evaluation metrics, and domain-specific challenges across civil and environmental engineering.

### Findings

The review finds that generative AI has growing potential in tasks such as automated layout generation, planning, scheduling, and iterative engineering support. At the same time, it identifies major limitations, including domain-specific data scarcity and heterogeneity, weak integration with existing engineering workflows, lack of suitable datasets, absence of systematic evaluation metrics, and limited codal support.

### Relevance to road design

Although it is not specific to road design, it is highly relevant to road engineering because it provides a civil-engineering-level view of what generative AI can realistically offer and what currently prevents dependable use in standards-constrained design contexts.

### Relevance to AI workflow

This source is very useful for discussing workflow because it directly addresses how generative AI may support planning, scheduling, iterative tasks, and broader engineering processes while also identifying why workflow integration remains difficult.

### Limitations

The review is broad rather than road-design-specific, so its conclusions must be transferred to road design with caution. As a review of a rapidly evolving area, it may also become dated quickly as tools and evaluation practices change.

---

## Source 5

### Full citation

Hasan, M., & Lu, M. (2025). Bridging AI and explainability in civil engineering: the Yin-Yang of predictive power and interpretability. *AI in Civil Engineering, 4*, Article 21. https://doi.org/10.1007/s43503-025-00066-6

### Aim

To examine explainable AI in civil engineering and propose a framework for balancing predictive performance with interpretability, transparency, and accountability in engineering decision support.

### Method

Review-based study focused on machine learning and explainable AI in civil engineering, especially construction engineering and management. The paper analyzes explainability attributes, compares model characteristics, and proposes a tailored XAI assessment framework.

### Findings

The study finds that explainability is critical in safety- and compliance-sensitive engineering applications because end users remain accountable for AI-informed decisions. It argues that predictive power alone is insufficient and that model transparency, interpretability, validation, and deployment monitoring are necessary for trustworthy engineering use.

### Relevance to road design

This source is strongly relevant to road design because road design decisions also involve safety, standards compliance, professional accountability, and the need to justify decisions to stakeholders. It supports discussion of why explainability is essential before AI can be relied on in road design practice.

### Relevance to AI workflow

It is useful for AI workflow because it highlights the importance of transparent outputs, validation processes, and decision traceability when AI tools are integrated into planning, analysis, and reporting workflows.

### Limitations

The paper focuses mainly on civil engineering decision support and construction-related contexts rather than road design specifically. It is also more conceptual and framework-oriented than empirically focused on one deployed road-design workflow.

---

## Source 6

### Full citation

Salah, M., & Alabdullatief, A. (2025). Architecture of tomorrow: The construction industry in the era of artificial intelligence. *Automation in Construction, 178*, 106429. https://doi.org/10.1016/j.autcon.2025.106429

### Aim

To review how artificial intelligence is being applied across the construction industry, identify major application domains and technologies, and highlight future research directions for broader implementation.

### Method

PRISMA-based systematic literature review of 178 studies published between 2015 and 2024, combined with quantitative analysis of AI technologies and application domains in construction.

### Findings

The review finds that AI is being applied across project phases, but most applications remain concentrated in selected domains such as construction management. It also shows that machine learning and deep learning dominate the literature, while areas such as natural language processing, transfer learning, and broader integration remain underexplored. The paper concludes that significant limitations and research gaps still prevent the development of a comprehensive AI framework for the construction sector.

### Relevance to road design

This source is indirectly relevant to road design because road projects sit within the broader built-environment and infrastructure domain. It helps frame road design as part of a wider industry that still lacks comprehensive AI integration across the full project lifecycle.

### Relevance to AI workflow

It is valuable for workflow discussion because it shows that AI adoption remains fragmented across stages and disciplines, which supports the argument that end-to-end AI-enabled workflows are still underdeveloped.

### Limitations

The paper is about construction broadly rather than road design specifically, so its findings need careful transfer. It also focuses on mapping the literature rather than testing a road-design automation system.

---

## Source 7

### Full citation

El-Abbasy, A. A. A. (2025). Artificial intelligence-driven predictive modeling in civil engineering: a comprehensive review. *Journal of Umm Al-Qura University for Engineering and Architecture, 16*, 1322-1345. https://doi.org/10.1007/s43995-025-00166-5

### Aim

To synthesize AI applications across major civil engineering domains and assess how predictive and hybrid AI models are being used to improve analysis, optimization, and decision-making.

### Method

Comprehensive review of AI applications across eight civil engineering domains, including transportation and pavement engineering, construction management, BIM, structural design, and sustainability-related areas.

### Findings

The review concludes that AI improves prediction accuracy, optimization, and decision support across many civil engineering tasks, especially in complex nonlinear problems. It also highlights recurring adoption challenges such as interpretability concerns, computational demands, and the need for better domain-specific datasets and practical deployment pathways.

### Relevance to road design

This source is relevant to road design because it includes transportation and pavement engineering within a broader civil engineering landscape, helping position road design within wider AI adoption trends and limitations.

### Relevance to AI workflow

It supports the workflow perspective by showing that AI is often used in separate predictive and optimization tasks rather than in fully connected end-to-end engineering workflows, which is useful for identifying current gaps.

### Limitations

Because it is a broad civil engineering review, it does not provide deep detail on road design specifically. Its emphasis is also stronger on predictive modeling than on generative AI or integrated explanation-writing workflows.
