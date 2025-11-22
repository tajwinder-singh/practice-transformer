# 𝐅𝐫𝐨𝐦 𝐀𝐭𝐭𝐞𝐧𝐭𝐢𝐨𝐧 𝐭𝐨 𝐓𝐫𝐚𝐧𝐬𝐟𝐨𝐫𝐦𝐞𝐫𝐬 — 𝐁𝐮𝐢𝐥𝐝𝐢𝐧𝐠 𝐚 𝐂𝐨𝐦𝐩𝐥𝐞𝐭𝐞 𝐓𝐫𝐚𝐧𝐬𝐥𝐚𝐭𝐢𝐨𝐧 𝐌𝐨𝐝𝐞𝐥 𝐟𝐫𝐨𝐦 𝐒𝐜𝐫𝐚𝐭𝐜𝐡

---

https://github.com/user-attachments/assets/9a5d26fc-2b8b-41a9-9d2d-9da45b0e234d

---

After learning about **Attention** and **Self-Attention**, I wanted to take the next step — implementing a complete **Transformer model** myself.

This project helped me understand how each part — **encoder, decoder, and attention heads** — work together to make translation possible.

---

## 𝐒𝐭𝐞𝐩𝐬 𝐈 𝐅𝐨𝐥𝐥𝐨𝐰𝐞𝐝

### 𝑺𝒕𝒆𝒑 1: 𝑷𝒓𝒆𝒑𝒂𝒓𝒊𝒏𝒈 𝒕𝒉𝒆 𝑫𝒂𝒕𝒂𝒔𝒆𝒕
- I started with **English–French sentence pairs**, saved them in both `.json` and `.txt` formats.  
- Then, I trained **SentencePiece tokenizers** separately for each language to generate subword-level vocabularies.  
  This step ensured compact vocabulary size and efficient training.

---

### 𝑺𝒕𝒆𝒑 2: 𝑴𝒐𝒅𝒆𝒍 𝑪𝒐𝒎𝒑𝒐𝒏𝒆𝒏𝒕𝒔

#### • Encoder Block  
- Implemented **Multi-Head Self-Attention** using the formula:  

- Added a **Feed-Forward Network (FFN)** after attention to capture nonlinear patterns.

#### • Decoder Block  
- Used **Masked Self-Attention** to prevent the model from seeing future tokens.  
- Added **Cross-Attention**, where the decoder’s query interacts with the encoder’s key and value to align predicted words with the input context.

**Example:**
→ Decoder’s query = currently predicted token
→ Encoder’s key/value = actual context from input sentence

This alignment tells the model how “correct” its prediction was at each step.

---

### 𝑺𝒕𝒆𝒑 3: 𝑬𝒎𝒃𝒆𝒅𝒅𝒊𝒏𝒈𝒔 𝒂𝒏𝒅 𝑷𝒐𝒔𝒊𝒕𝒊𝒐𝒏𝒂𝒍 𝑬𝒏𝒄𝒐𝒅𝒊𝒏𝒈
- Used **token embeddings** combined with **positional embeddings**, allowing the model to understand sequence order.  
- Created **padding** and **look-ahead masks** to manage variable-length sequences and prevent information leakage.

---

### 𝑺𝒕𝒆𝒑 4: 𝑻𝒓𝒂𝒊𝒏𝒊𝒏𝒈 𝒕𝒉𝒆 𝑻𝒓𝒂𝒏𝒔𝒇𝒐𝒓𝒎𝒆𝒓
- Defined parameter values such as **embedding size**, **attention heads**, and **depth layers**.  
- (Note: Full model training was skipped due to resource limitations.)

---

## 𝐋𝐞𝐚𝐫𝐧𝐢𝐧𝐠𝐬
⇨ **Multi-Head Attention** captures relationships from multiple perspectives simultaneously.  
⇨ **Masked Self-Attention** ensures proper auto-regressive behavior.  
⇨ **Cross-Attention** bridges input and output context effectively.  
⇨ **Positional Embeddings** are essential since transformers lack recurrence.  
⇨ Building everything from scratch clarified how the Transformer’s elegance lies in **parallelization and contextual awareness**.

---

### 🔗 Linkedin: [https://tajwinder-singh-](https://www.linkedin.com/in/tajwinder-singh-?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base_contact_details%3Bw5O6vzwkRg29EPBIrkLOtg%3D%3D)

---

### 𝐐𝐮𝐞𝐬𝐭𝐢𝐨𝐧 𝐟𝐨𝐫 𝐑𝐞𝐚𝐝𝐞𝐫𝐬
👉 *If you had to explain Transformers in one line, what would you say they do better than RNNs?*

---

> *I didn't train the full model due to resource shortage, but below is the model's summary.*

---

**#DeepLearning #NLP #Transformers #AttentionMechanism #MachineLearning #AI #SequenceModeling #LanguageTranslation #DataScience #NeuralNetworks**



