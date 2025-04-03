# First_LLM
Trying to build an LLM from scratch

#Day-01
I have built a lightweight and customizable text tokenizer that converts text into numerical representations and vice versa. This tokenizer supports special tokens, handles unknown words, and ensures proper spacing in decoded text.
Features:
Tokenization: Splits text into words and punctuation.
Encoding: Converts text into numerical token IDs.
Decoding: Converts token IDs back into text with proper formatting.
Unknown Token Handling: Replaces out-of-vocabulary words with <|unk|>

# Day-02 - Byte Pair Encoding (BPE)

Byte Pair Encoding (BPE) is a data compression algorithm that is widely used for subword tokenization in Natural Language Processing (NLP). It helps in handling out-of-vocabulary (OOV) words and improving language model performance.

## 🔹 How BPE Works
1. **Initialize**: Start with a vocabulary of individual characters.
2. **Merge Pairs**: Identify the most frequent adjacent pair of symbols and replace them with a new token.
3. **Repeat**: Continue merging until the desired vocabulary size is reached.

## 📌 Example
Consider the word `banana`:
- Initial tokens: `b a n a n a`
- Merge the most frequent pair (`a n` → `an`): `b an an a`
- Merge again (`an a` → `ana`): `b ana ana`
- Final tokens: `b ana ana`
