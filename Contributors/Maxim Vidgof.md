# Maxim Vidgof
[maxim.vidgof@wu.ac.at](mailto:maxim.vidgof@wu.ac.at)

## Ideas

- **Full desktop automation using LLM and RPA.**
    Use screen scraping (+ cursor position and screenshot interpretation from models like GPT-4o) to get current state, use LLM to decide on next action (move pointer, press button, enter text, etc.) and use RPA to perform this action.

  References: 
    - Barba, I., Del Valle, C., Jiménez-Ramírez, A., Weber, B., & Reichert, M. (2024, June). Discovering Two-Level Business Process Models from User Interface Event Logs. In *International Conference on Advanced Information Systems Engineering* (pp. 456-472). Cham: Springer Nature Switzerland.
    - Beerepoot, I., Barenholz, D., Beekhuis, S., Gulden, J., Lee, S., Lu, X., Overbeek, S., van de Weerd, I., van der Werf, J. M. & Reijers, H. A. (2023, October). A window of opportunity: Active window tracking for mining work practices. In *2023 5th International Conference on Process Mining (ICPM)* (pp. 57-64). IEEE.
- **Influence of automation on organization culture**
    What do existing theories say about it? Mention negative impact such as unlearning by automation. Would be best to also conduct a case study.
- **Large Language Models for researchers**
    Inspired by panel discussions like "BPM in the Age of Agents, Assistants, and Co-Pilots" at BPMDS 2024 and "AI Ink: Should we let generative technology transform academic writing?" at CAiSE 2024. While researchers and tech experts argue about whether there is any creativity in LLMs or whether they just recombine existing data, even the latter case can help to look at the body of knowledge and state of the art from a different angle, some suggestions are:
    - Extracting pairs of "research question & method used to answer it" from published papers and fine-tuning an LLM can result in a tool suggesting the most suitable (or at least the most commonly used) research method for a given research question, which can be used by junior researchers to receive additional guidance. But also the other way round, LLM can provide some unorthodox suggestions allowing to study the problem from an unexpected perspective.
    - Using LLMs to generate research questions based on given input (e.g. a collection of papers). Ethical considerations aside, this can result in some unexpected and innovative research ideas.
- **Trace clustering using event data**
    Most variant analysis techniques focus on event sequences, and only a handful uses event data. Recently, a new approach was introduced that generates features based on domain knowledge and uses them to distinguish between variants. It would be interesting to extend this idea in the following ways:
    - Compare this with applying (not process-aware) clustering techniques with selected data attributes as variables and traces as singular observations.
    - Cluster the traces based on combination of attributes and event sequences, i.e. apply a clustering algorithm on a combination of trace distances (e.g. Levenstein distance) + attribute distances (possibly normalized).
    - Use features generated by the algorithm to guide the building of a distance function for clustering, e.g. assign distance of 0 on attribute if it belongs to the same class (e.g. all age > 60) or infinity for traces that must never be in one cluster.
    
  References:
    - Rubensson, C., Mendling, J., & Weidlich, M. (2024, June). Variants of Variants: Context-Based Variant Analysis for Process Mining. In *International Conference on Advanced Information Systems Engineering* (pp. 387-402). Cham: Springer Nature Switzerland.
- **Relationship between multi-perspective and object-centric process mining**
    The two approaches to process mining share at least one crucial feature: they allow to select different case notion dynamically based on the objective of analysis. How are the two conceptually related and what does it mean for the research community?
- **Changes in resources' task preferences over time**
    One possible manifestation of concept drift is when the employees change the order in which they perform assigned tasks or the tasks they choose to perform in general. It is interesting to study such changes in task selection over time in business processes, their contributing factors and also effects, possibly by means of a case study.

  References:
    - Klijn, E. L., Mannhardt, F., & Fahland, D. (2024, June). Multi-perspective Concept Drift Detection: Including the Actor Perspective. In *International Conference on Advanced Information Systems Engineering* (pp. 141-157). Cham: Springer Nature Switzerland.
- **Prescriptive process monitoring as human-actiated digital twin**
    There are different maturity levels for digital twins (DT). Over 50% of state-of-the art digital twin papers only use a *shadow* - a digital twin that only gets data from the real object but does not return anything, does not control the physical twin. Higher levels of maturity include *human-actuated* digital twins - where the DT provides human actor with recommendations, *human-supervised* - where the DT plans some actions on the physical object but requires human permission, and *fully autonomous* DTs - where the DT automatically selects and performs actions on physical objects. Prescriptive process monitoring algorithms can be seen as *human-actuated* (and potentially even *fully autonomous*) digital twins of a process. What can this conceptualization bring for PPM and DT research and practice?

  References:
    - David, I., & Bork, D. (2024, June). Infonomics of Autonomous Digital Twins. In *International Conference on Advanced Information Systems Engineering* (pp. 563-578). Cham: Springer Nature Switzerland.
