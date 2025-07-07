# manifesto_annotations

*Chandini Tolet - BU CAS Math/CS 26'- ACSS Summer Internship in Paris, France*

In this repository, I analyze the agreement between annotators for the Speeches_Manifesto Project at ACSS. These annotations were created with the goal of training an LLM in the future; however, we need to ensure the training data is meaningful to produce accurate predictions. 

- **File 1: Annotations_Labeling_Statistics**
    Description: This file compares annotations for the field Answer.manifesto_class.labels using the fliess kappa metric. Since fleiss kappa requires that each worker have its own column with annotations, I split up the dataset by label. In this file, each label is its own dataframe such that the rows are speeches and the columns are arbitrary workers 1,2,3. The workers are arbitrary since they changed with each speech. Additionally, the cells are binary values (0,1) where 1 indidcates that a worker chose this label for this speech and 0 indicates this worker did not choose this label for this speech. All-in-all, these fleiss kappa metrics indicate whether annotators agree on each label for different speeches. 

    Instructions: Open Annotations_Labeling_Statistics, create venv in terminal, run file. Realistically, the code can be re-run on different gold_dataset.csv versions if changes were made to the annotations. 

 - **File 2: Annotations_Speech_Statistics**
    Description: This file compares annotations for the field Answer.manifesto_class.labels using the fliess kappa metric. Since fleiss kappa requires that each worker have its own column with annotations, I split up the dataset by Speech. In this file, each Speech is its own dataframe such that the rows are labels and the columns are arbitrary workers 1,2,3. The workers are arbitrary since they changed with each speech. Additionally, the cells are binary values (0,1) where 1 indidcates that a worker chose this label for this speech and 0 indicates this worker did not choose this label for this speech. All-in-all, these fleiss kappa metrics indicate whether annotators agree on different labels for each speech. 

    Instructions: Open Annotations_Speech_Statistics, create venv in terminal, run file. Realistically, the code can be re-run on different gold_dataset.csv versions if changes were made to the annotations. 