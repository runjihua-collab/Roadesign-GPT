## Development Plan for **RoaDesign GPT**

### 1. Project Aim

My aim is to develop **RoaDesign GPT**, a custom GPT that supports **Australian road design learning and preliminary design guidance**, with the first version focused on **Victoria**. The system will help students answer general road design questions, identify the correct reference documents, explain design concepts clearly, and later perform structured checks through external tools. The technical basis will come from the **Austroads Guide to Road Design**, especially Part 1 and Part 3, together with Victoria's **DTP technical publications**, which include the **Supplement to AGRD** and **Road Design Notes**. ([Austroads][1])

### 2. Overall Development Idea

The core idea is to **separate the user-facing GPT from the backend engineering system**. RoaDesign GPT will act as the front-end teaching assistant, while **Codex** will be used as the development tool to build the backend code, including standards retrieval, calculation functions, and testing. This approach is more practical than trying to fine-tune Codex itself, because OpenAI's current Codex model pages state that fine-tuning is not supported for those Codex models. ([Austroads][1])

In simple terms, the system will work like this:
**RoaDesign GPT talks to the student**;
**Actions connect the GPT to external APIs**;
**Codex helps me build those APIs and the supporting codebase**. This matches OpenAI's platform structure, where custom GPTs are configured with instructions, knowledge, capabilities, and actions, while Actions are used to connect the GPT to external services. ([VicRoads][2])

### 3. Standards Scope

The first version will be based mainly on the following document groups:

* **Austroads Guide to Road Design Part 1: Objectives of Road Design**
* **Austroads Guide to Road Design Part 3: Geometric Design**
* **Victoria DTP Supplement to AGRD**
* **Victoria Road Design Notes**, especially those related to context-sensitive design and design exceptions
* selected lecture notes, worked examples, and assignment materials

This is a strong starting point because Austroads states that the Guide to Road Design provides the framework for efficient, safe, and context-sensitive road design, and Part 3 specifically covers geometric design elements such as design speed, cross-sections, horizontal and vertical alignment, superelevation, and sight distance. Victoria's DTP technical publications page also confirms that current road design documents are managed through DTP and include both **Supplement to AGRD** and **Road Design Notes**, while legacy VicRoads technical publications are also included in the same collection. ([Austroads][1])

### 4. First Version Scope

To keep the project realistic, the first version of RoaDesign GPT will focus on **Victoria geometric design topics** only. It will initially answer three main types of questions:

1. **Standards identification questions**
   Example: "Which Victorian document should I check for this road alignment issue?"

2. **Concept explanation questions**
   Example: "What is superelevation and why is it used?"

3. **Basic design-check questions**
   Example: "How should I check a horizontal curve for a given design speed?"

I am deliberately keeping the first release narrow. Road design is a broad field, so the first goal is to make one part of the system reliable before expanding into intersections, drainage, roadside design, or traffic control devices.

### 5. Phase 1: Build the GPT Prototype

The first phase is to create a working **prototype custom GPT** directly in the GPT editor. In this phase, I will configure:

* the GPT name and description
* system instructions
* uploaded knowledge files
* conversation starters
* a clear teaching-oriented response style

At this stage, the GPT will mainly rely on **uploaded files** and internal reasoning. I will instruct it to:

* classify the user's question as a standards question, a concept question, or a calculation question
* search uploaded documents first when standards are involved
* avoid inventing clause numbers or technical requirements
* explain assumptions, units, and steps when calculations are discussed
* clearly state when the uploaded materials are not sufficient to confirm an answer

The purpose of this phase is to quickly test whether the GPT can already behave like a useful road design tutor before I spend time building external systems.

### 6. Phase 2: Build the Backend With Codex

Once the prototype GPT works reasonably well, I will move to backend development. This is where **Codex** becomes important. I will use Codex to help generate and maintain the backend project, including scripts, APIs, data structures, and tests.

The backend will contain two main parts.

The first part is a **standards retrieval service**. This service will store the standards in a more structured format, such as:

* jurisdiction
* document title
* part number
* topic
* section title
* content summary
* keywords

This will allow the system to search documents more accurately than simply relying on large uploaded PDFs.

The second part is a **calculation engine**. In the first version, it will include simple engineering functions such as:

* horizontal curve checking
* vertical curve checking
* stopping sight distance guidance

These functions will return structured outputs, including inputs, assumptions, intermediate logic, final results, and warnings. This is important because numerical checks should be handled by explicit code rather than only by free-text generation.

### 7. Phase 3: Connect the GPT With Actions

After the backend is available, I will connect RoaDesign GPT to it using **Actions**. This is the key step that turns the GPT from a document-based assistant into a tool-using engineering assistant.

For example, the GPT may call:

* `search_standard`
* `get_section_summary`
* `check_horizontal_curve`
* `check_stopping_sight_distance`

In practice, the workflow will be:

1. the user asks a question in natural language
2. RoaDesign GPT decides whether the answer requires a document lookup or a calculation
3. if needed, it calls the relevant Action
4. the backend returns structured data
5. the GPT converts that result into a clear student-friendly explanation

This architecture is the most logical way to combine GPT, Actions, and Codex in one project.

### 8. Testing Strategy

I will not evaluate the system only by whether the answers sound fluent. I will test it against four practical criteria:

* **Reference accuracy**: does it identify the correct Austroads or Victorian source?
* **Technical accuracy**: are the calculations and engineering explanations reasonable?
* **Teaching quality**: are the steps clear enough for students?
* **Honesty about uncertainty**: does it clearly say when a standard cannot be confirmed?

This is important because the value of RoaDesign GPT is not only in producing polished answers, but in giving answers that are traceable, careful, and useful for learning.

### 9. Final Development Logic

In summary, my development strategy is to start with a **small but working Victoria-focused GPT**, then use **Codex** to build the supporting backend, and finally connect the two through **Actions**. The first release will focus on geometric design and general standards guidance using **Austroads Part 1, Austroads Part 3, and Victorian DTP road design publications**. Once this core workflow is reliable, the system can later be expanded to cover more advanced topics such as intersections, drainage, and design review. ([Austroads][1])

[1]: https://austroads.com.au/safety-and-design/road-design/guide-to-road-design "Guide to Road Design | Austroads"
[2]: https://www.vicroads.vic.gov.au/business-and-industry/technical%20publications "DTP technical publications | vic.gov.au"
