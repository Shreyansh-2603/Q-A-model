
# Question Answering Model

Question answering is a complex task in natural language processing (NLP) that requires a deep understanding of sentence context and emotions to provide accurate responses to queries. Our model demonstrates versatility by performing various tasks such as machine translation, named entity recognition, and parts of speech tagging. It utilizes a Dynamic Memory Network (DMN) architecture with attention mechanisms to generate answers based on input sentences, questions, and correct answers from the Babel dataset.
## Approach
### Methodology
The model consists of four core segments:

- Input Module: Processes raw sentences into distributed vector representations.
-  Question Module: Encodes questions into vector representations.
-  Episodic Memory Module: Iteratively updates memory representations based on input and question representations.
- Answer Module: Utilizes memory representations to address queries.

### Model Architecture

- Input Module: Utilizes a recurrent neural network (RNN) to capture input sequences.
- Question Module: Similar to the input module, encodes questions into vector representations.
- Episodic Memory Module: Employs an attention mechanism paired with a recurrent network to update memory representations iteratively.
- Answer Module: Uses a GRU with an initial state initialized to the last memory slice to generate responses.

### Training Paradigm

The model is trained as a supervised classification challenge, aiming to minimize cross-entropy errors associated with answer sequences. It incorporates gate supervision for datasets like bAbI, enhancing overall performance.
Question Answering

Evaluation is performed on the Facebook bAbI dataset, assessing the model's ability to comprehend and reason based on provided facts. Training objectives include minimizing cross-entropy costs for both gates and answers.
## Results

The model demonstrates proficiency in question answering tasks, with improvements observed through gate supervision modifications.

