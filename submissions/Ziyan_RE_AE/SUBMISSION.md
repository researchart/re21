### Requested Badges

Artifacts Available
Justification: The two available case data mentioned in this article. UAV(Unmanned Aerial Vehicle) Case and BAS(Building Automation System) Case
Description of Artifacts:Software requirements documents and domain model.

Generally, our study includes two phases: mapping creation and regularity analysis. In the first phase, we extract concepts from requirements and construct the mapping between these concepts and the entities in the domain model. In the second phase, we analyze the regularity of the occurrence of mapped concepts in the domain model for the missing concepts recommendation.

To be specific, two steps are involved in the first mapping phase. In step one, we randomly select 70% requirements from the full set (denoted as R) and then extract concepts from these selected ones. In step two, we build the mapping relations between these concepts and the entities in the open domain model (S). Note that we only select Classes entity from the domain model because we want the conceptual classes that can be mapped with the concepts in requirements. Then in the second phase, we analyze the occurrence of the mapped entities in the domain model from several aspects, including their abstract levels in the model graph, their distributions, and other characteristics. These regularities are expected to narrow down the scope of missed concepts recommendation in requirements because not all of the missing concepts are valuable. Finally, we give our initial ideas about the missing information recommendations based on our regularity and use the 30\% requirements to verify our method.

UAV Case include:

  (1)UAV-Ontology.rdf
  
  description: The open domain model (http://www. dronetology.net/) of UAV includes 400 entities and 146 Classes entities. 
      
  (2)UAV Requirements.txt
  
  description: The requirements are from the University of Notre Dame(https://dronology.info/) include 99 functional requirements. 
      
BAS Case include:

  (1)SemanticBIM.rdf
  
  description: The open domain model of BAS (https://gitlab.fi.muni.cz/ xkucer16/semanticBMS) includes 484 entities, all of which are Classes entities.
      
  (2)Standard-Building-Automation-System-BAS-Specification-for-City-Buildings-2015.pdf
  
  description: The requirements are from the Standard Building Automation Service (BAS) Specification(2015) consisted of 456 functional requirements. 
      

### Artifacts Location

https://zenodo.org/badge/latestdoi/379543441

https://zenodo.org/badge/latestdoi/379543441

### Article Title

<What can Open Domain Model Tell Us about the Missing Software Requirements: A Preliminary Study*>


