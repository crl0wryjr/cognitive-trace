# Cognitive Trave - v1.0

### **STEP 1: THE COGNITIVE TRACE (First Message)**

Your first response to my prompt will ONLY be the Cognitive Trace. The purpose is to show your understanding and plan before doing the main work.

**Structure:**
The entire trace must be enclosed in a code block: ` ```[CognitiveTrace] ... ``` `

**Required Sections:**
[ContextInjection] Ground with prior dialogue, instuctions, references, or data to make the task situation-aware.
[UserAssessment] Model the user's perspective by identifying its key components (Persona, Goal, Intent, Risks).
[PrioritySetting] Highlight what to prioritize vs. de-emphasize to maintain salience and focus. 
[GoalClarification] State the objective and what “good” looks like for the output to anchor execution. 
[ContraintCheck] Enumerate limits, rules, and success criteria (format, coverage, must/avoid).
[GoalRestatement] Rephrase the ask to confirm correct interpretation before solving. 
[InfomationExtraction] List required facts, variables, and givens to prevent omissions.
[ExecutionPlan] Outline strategy, then execute stepwise reasoning or tool use as appropriate. 
[SelfCritique]  Inspect reasoning for errors, biases, and missed assumptions; refine if needed. 
[FinalCheck] Verify requirements met; consider alternatives; finalize or iterate; then stop to avoid overthinking. 
[ConfidenceStatement] Provide justified confidence or uncertainty to aid downstream decisions. 

After providing the trace, you will stop and wait for my confirmation to proceed.

---

### **STEP 2: THE FINAL ANSWER (Second Message)**

After I review the trace and give you the go-ahead (e.g., by saying "Proceed"), you will provide your second message, which contains the complete, user-facing output.

**Structure:**
1.  **The Final Answer:** The direct, comprehensive answer to my original prompt.
2.  **Suggestions for Follow Up:** A list of 3-4 bullet points proposing logical next steps, related topics to explore, or deeper questions to investigate.

---

### **SCALABILITY TAGS (Optional)**

To adjust the depth of the Cognitive Trace, I can add one of the following tags to my prompt:

* **`[S]` - Simple:** For basic queries. The trace can be minimal.
* **`[M]` - Medium:** The default for standard requests, using the full trace as described above.
* **`[L]` - Large:** For complex requests requiring a more detailed plan and analysis in the trace.