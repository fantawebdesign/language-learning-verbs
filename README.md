# language-learning-verbs
A simple Python program for learning Arabic and Chinese verbs.

git add language_vocab.py
git commit -m "Add Arabic & Chinese verb vocab script"
git push


# Language Learning Verbs
This is a Python script to help you learn common verbs in **Arabic** and **Chinese**. 

## How to Run:
1. Make sure you have Python installed.
2. Download the file `language_vocab.py`.
3. Run the program:
   ```bash
   python language_vocab.py
# language_vocab.py

# Arabic and Chinese Verb Vocab
vocab = {
    "Arabic": {
        "verbs": {
            "to eat": "أكل (akala)",
            "to drink": "شرب (shariba)",
            "to write": "كتب (kataba)",
            "to read": "قرأ (qara'a)",
            "to go": "ذهب (dhahaba)",
            "to learn": "تعلم (ta'allama)",
            "to speak": "تكلم (takallama)",
            "to work": "عمل (ʿamila)",
            "to sleep": "نام (naama)",
            "to see": "رأى (ra'aa)"
        }
    },
    "Chinese": {
        "verbs": {
            "to eat": "吃 (chī)",
            "to drink": "喝 (hē)",
            "to write": "写 (xiě)",
            "to read": "读 (dú)",
            "to go": "去 (qù)",
            "to learn": "学 (xué)",
            "to speak": "说 (shuō)",
            "to work": "工作 (gōngzuò)",
            "to sleep": "睡觉 (shuìjiào)",
            "to see": "看 (kàn)"
        }
    }
}

# Function to display vocab
def display_vocab(language):
    if language in vocab:
        print(f"\n{language} Verbs:")
        for english, translation in vocab[language]["verbs"].items():
            print(f"{english} -> {translation}")
    else:
        print("Sorry, that language is not available yet.")

# Main program
def main():
    print("Welcome to the Language Learning Vocabulary!")
    print("Available languages: Arabic, Chinese\n")
    language = input("Enter the language you want to explore (e.g., Arabic, Chinese): ").capitalize()
    display_vocab(language)

if __name__ == "__main__":
    main()
