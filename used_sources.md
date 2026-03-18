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
