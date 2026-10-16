# BUS5001 Assessment 3 – ESG Analytics Experiments

This repository holds practical evidence for Q3 (LLM ESG incident-message triage) and Q4 (Google NotebookLM evaluation).

## Q3: ESG Message Triage

Notebook: `Q3_ESG_Message_Triage_Colab.ipynb`. Three synthetic messages concerned water leakage, recycling contamination and a blocked accessible entrance. The experiment compared Google Gemini against a simple rule-based baseline.

### Observed evaluation
- Gemini category matches: **3/3**.
- Gemini urgency matches: **1/3** (water leak classified MEDIUM vs reference HIGH; recycling LOW vs reference MEDIUM; accessibility HIGH vs HIGH).
- Rule-based baseline matches: **3/3** on these hand-chosen test cases; this does not establish superior generalisation.

The experiment is a supervised proof of concept, not a deployed Azure system. Any Azure architecture described in the report is a proposal.

## Q4: NotebookLM

The log `Q4_Experiment_Log.md` documents five experiments on GRI reporting standards: comparison, source-grounded Q&A, unsupported-fact handling, study-guide generation and Audio Overview.

## Evidence

Add downloaded Q3 CSVs (`llm_results.csv`, `comparison.csv`) and your actual screenshots to this repository. The Audio Overview may be included as a separate `.m4a` evidence file; review its content before claiming full factual accuracy. The original GRI PDFs may be linked rather than re-uploaded.

## Privacy and reproducibility

All Q3 example messages are synthetic. **Do not commit Gemini API keys, Colab Secrets, personal credentials, or sensitive records.** Execution of the notebook requires the user's own Gemini API key stored in Colab Secrets under `GEMINI_API_KEY`.
