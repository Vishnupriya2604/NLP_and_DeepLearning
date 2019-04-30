# textrank_text_summarization
 Automatic Text Summarization using TextRank algorithm for Speeches.
 [Vishnupriya Venkateswaran- 04/22/19]
 
 The speeches used are Commencment Speeches of previous Presidents of USA.
 The Speech_ID for each president are as given below:
 Speech_id 1 : Jimmy Carter
 Speech_id 2 : Ronald Reagan
 Speech_id 3 : Ronald Reagan
 Speech_id 4 : George Bush
 Speech_id 5 : William J. Clinton
 Speech_id 6 : William J. Clinton
 Speech_id 7 : George W.Bush
 Speech_id 8 : George W.Bush
 Speech_id 9 : Barack Obama
 Speech_id 10: Barack Obama
 Speech_id 11: Donald J. Trump

Steps Followed to extract summary combining all the speeches:
Step 1: Read all speeches.
Step 2: Split the text into individual sentences.
Step 3: We will find vector representation (word embeddings) for each and every sentence. [ I used the glove word embedding, it can be downloaded from https://nlp.stanford.edu/data/glove.6B.zip]
Step 4: Similarities between sentence vectors are then calculated and stored in a matrix. We use cosine similarity
Step 5: The similarity matrix is then converted into a graph, with sentences as vertices and similarity scores as edges, for sentence rank calculation.
Step 6:   A certain number of top-ranked sentences form the final summary.
