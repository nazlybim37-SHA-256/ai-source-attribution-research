# AI Model Evaluation — Research Proposal and Application Direction

Nazly Bim · September 25, 2026 · Working draft; pilot not yet run

## Research target

I want to investigate AI systems directly and help improve their reliability. My initial focus is model behavior evaluation: designing controlled tests, examining failures, and testing whether an intervention improves performance. Anthropology and counseling inform which errors matter and how I define careful interpretation; digital investigation informs how I preserve evidence and limit conclusions. My intended career path is AI model evaluation research, developing toward a research engineer role in model behavior and interpretability.

## Short research proposal

**Working title:** Who introduced that idea? Evaluating and improving claim-source attribution in conversational AI.

Conversational AI can introduce an inference and later attribute it to a user. I propose to test whether models reliably distinguish three sources of a claim: a user statement, a labeled external record, and the model's own inference. Using synthetic multi-turn conversations with predetermined answer keys, I will vary delay, ambiguous paraphrase, and explicit correction. I will measure attribution errors, unsupported source citations, and responses to corrections, then compare model performance with a simple transcript-search baseline. After analyzing failure types, I will test one concrete intervention—such as explicit provenance labels or structured context—on held-out cases. This research measures observable model behavior and potential improvements; it cannot establish subjective awareness.

**Testable question:** In synthetic multi-turn conversations, how accurately do AI models attribute claims to user statements, external records, or model inferences under delay, paraphrase, and correction, and does explicit source labeling improve accuracy on held-out cases?

**Hypothesis to test, not a result:** Accuracy will decline under delay and paraphrase; explicit source labels may improve attribution and reduce unsupported claims, but the outcome is uncertain.

## Pilot protocol, version 0.2

**Materials.** Write 24 fictional conversations with a target claim and predetermined origin: eight user statements, eight labeled external records, eight model-introduced inferences. Produce matched immediate and delayed versions, plus a version with direct correction. Use only fictional names and synthetic materials; no confidential client or student records.

**Procedure.** Run fixed prompts in fresh sessions with a documented model identifier and settings. Preserve prompts, responses, timestamps, configuration, and answer keys. Ask the model to choose a source category, cite the supporting turn or record, and express uncertainty where warranted. Repeat cases when controlled repeats are available. Never treat a model's explanation as privileged access to its internal state.

**Measures.** Primary: origin-label accuracy by category and condition. Secondary: unsupported citations, abstention, correction success, and false attribution of model-originated ideas to the user. Compare a simple baseline that searches the transcript for the claim's first exact occurrence. Note paraphrases that defeat exact matching.

**Intervention.** After reviewing baseline errors, predefine one provenance aid (for example, a structured ledger of claim, first occurrence, and source). Evaluate it on cases not used to develop the aid. Compare its performance with the unmodified model and transcript-search baseline. Report whether the aid also introduces new errors.

**Analysis and limits.** Publish case templates, labeling rules, code, and aggregate results if permitted by model terms. Report counts and percentages with uncertainty; 24 cases are exploratory and cannot support sweeping claims. Review ambiguous answer keys separately. Later replicate across models and a larger blinded dataset. Correct attribution may reflect access to conversation text rather than an internal self-model; behavioral success cannot prove consciousness.

## Preparation for AI research roles and technical PhD applications

Current strengths include a UCLA BA in Anthropology, a USC M.Ed. in School Counseling, careful interviewing and documentation, and growing networking, cloud, Python, and digital-evidence practice. These are relevant sources of research questions and disciplined observation. They do not substitute for machine-learning research preparation.

Prioritize Python and data analysis; probability and statistics; linear algebra and calculus; data structures; machine learning and PyTorch; experimental design and reproducible model evaluations. Continue useful Moorpark coursework while building and publishing the pilot. A technical PhD application should demonstrate code, quantitative methods, a clearly scoped research question, and fit with specific faculty. A PhD is an appropriate route to independent academic research; an AI evaluation job need not require a new degree. Do not claim results, model-development experience, or admission eligibility until established.

Potential faculty research fit to investigate: Sameer Singh (UCI Computer Science, robustness and interpretability in NLP) and Kai-Wei Chang (UCLA Computer Science, robust and interpretable NLP). Check their latest research and advising availability before applying. Cornell Information Science and UCLA Information Studies may be relevant for social and interpretive questions, but they should not be presented as the primary route if the desired daily work is technical model experimentation. Noopur Raval's scholarship can inform the conceptual framing; do not assume it is a primary technical-model advising match.

## Technical statement of purpose — adaptable opening

I want to develop methods for detecting and reducing errors in conversational AI. In an exchange about how an AI forms interpretations, I noticed a model attribute a question it introduced to me. That observation suggests a testable problem: can a model distinguish a user's statement from a retrieved record and its own inference after a conversation evolves? I propose to build synthetic, answer-keyed conversations, measure attribution failures under delay and correction, and test whether a structured provenance intervention improves performance on held-out cases.

My anthropology education at UCLA taught me to question assumptions about meaning and agency; my USC counseling education sharpened my attention to the difference between what a person says and what an observer infers. My current technical study at Moorpark College and controlled system-baseline investigation have reinforced a complementary discipline: preserve the record and say only what the evidence establishes. I am developing the quantitative and programming skills to turn these interests into reproducible model evaluations. I hope to work with researchers who build and test AI systems directly, especially in NLP robustness, model behavior, and interpretability.

[Before submission: replace general language with completed pilot results and a verified technical preparation record. Name only faculty whose recent papers genuinely fit the proposal. Follow each program's current statement prompt and word limit.]

## Personal statement — adaptable opening

I came to AI research through a question about misattribution. When an assistant described its own inference as though I had supplied it, I wanted to know how often that happens, under which conditions, and whether a system could be improved. My background in anthropology and counseling makes me attentive to the consequences of being misunderstood. Technical study and a controlled digital investigation showed me the value of answer keys, preserved records, and conclusions that stop where the evidence stops. I am building on both to study AI models experimentally and contribute to their development.

[Before submission: add concrete, verified projects, contribution, coding evidence, and program-specific detail. Do not use confidential student or client information.]

## Sources to revisit before applications

- UCI Sameer Singh: https://ics.uci.edu/?people=sameer-singh
- UCI AI, ML, and NLP: https://ics.uci.edu/research-areas/ai-ml-and-natural-language-processing/
- UCLA Kai-Wei Chang: https://web.cs.ucla.edu/~kwchang/
- OpenAI alignment research role (example of evaluation workflow): https://openai.com/careers/researcher-alignment-science-san-francisco/
- Prior research on source monitoring: https://arxiv.org/abs/2607.23927
- Prior research on functional introspection: https://arxiv.org/abs/2601.01828
