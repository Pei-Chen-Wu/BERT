# BERT
## 介紹
* a method of pretraining language representations
* can use these models to extract high quality language features from your text data
* can fine-tune these models on a specific task (classification, entity recognition, question answering, etc.) with your own data to produce state of the art predictions

## ELMO, BERT, GPT (Hung-yi Lee課程)
https://youtu.be/UYPa347-DdE!
### 機器如何讀懂文字
* 詞語分類

![image](https://user-images.githubusercontent.com/69243911/127823742-82f69675-7283-4301-ba82-58242a0fcb9a.png)
* 同詞語可能有多種意思
  * In typical word embedding,each word type has an embedding
  * 但每個token應該有自己一種type
###　ELMO
＊　RNN-based language models (trained from lots of sentences)
＊　考慮前後文的方法 : 將句子正逆向皆放入model
＊　多層RNN : 使用weighted sum
### BERT
* BERT = Encoder of Transformer

![image](https://user-images.githubusercontent.com/69243911/127824071-0b0ba548-805c-4fb3-85b5-97992b6a809b.png)

* Pre-training(training of BERT):
  * Masked LM
  * Next Sentence Prediction
![image](https://user-images.githubusercontent.com/69243911/127824050-dd731ac0-208e-4e69-8387-a2c847da8898.png)
* Fine-Tuning(How to use BERT) :
  * 單一句子的分類

  ![image](https://user-images.githubusercontent.com/69243911/127824181-9aceacfe-22ca-4eb9-bf90-df90a2342f02.png)
  * 句子中每個詞的分類

  ![image](https://user-images.githubusercontent.com/69243911/127824208-532391bb-bb5f-4ab2-bab3-cfabd3bd3c6f.png)

  * 兩個句子關係的分類

  ![image](https://user-images.githubusercontent.com/69243911/127824228-3e6cd853-18f6-4821-8e3f-2262d189ab04.png)

  * 問答系統

  ![image](https://user-images.githubusercontent.com/69243911/127824257-ed2c1c1d-7a9d-4b11-9f84-6796b69a963b.png)
  ![image](https://user-images.githubusercontent.com/69243911/127824267-0dd8c384-1cc1-47b5-a656-5be0819b983d.png)
  ![image](https://user-images.githubusercontent.com/69243911/127824279-c82c066a-8c70-41ea-89d9-393ea6aab0b6.png)

### ERNIE,GPT
* ERNIE : 
  designed for Chinese
* GPT :
  * GPT = transformer decoder
  * 預測接下來的詞彙
  * Zero-shot learning?
## BERT 實作練習_mask
* 載入中文 BERT 使用的 tokenizer

  ![image](https://user-images.githubusercontent.com/69243911/127824528-526c6fc0-b149-42ed-b365-2eaff82ec95d.png)
* 輸入文本，並使用 tokenizer 將一個中文句子斷詞

  ![image](https://user-images.githubusercontent.com/69243911/127824559-1e2765ce-a7d1-4c08-941d-dc9dfcc8d2df.png)







