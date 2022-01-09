# K-NCT
 
K-NCT (Korean Neural grammatical Correction Test set) was created for the development of Korean Grammatical error correction research. K-NCT can be applied to various features of constructs that can be objectively verified. 


## Data Description
The K-NCT consists of 3000 sentences.

Each sentence consisted of nine keys
- "index": The id that distinguishes sentences.
- "error_sentence": A sentence that contains the type of tagged error.
- "correct_sentence": The original sentence before the error was injected.
- "domain": The source of the original text
- "style": Korean text-style(Written / Spoken / Dialog)
- "syllable": The number of syllables in a sentence.
- "phrase": The number of phrases in the sentence.
- "number of error": The number of places where the error occurred.
- "error_type": Of the suggested error types, the error type tagged in the sentence.


## Characteristics
- K-NCT has a fairness configuration of 500 spacings, 500 punctuations, 500 numerical and 1500 spelling and grammatical errors.
- The dataset covers the range of syllable lengths of 2∼20, 21∼29, 30∼50, and 51 syllables or more to ensure diversity.

## Example
 {
   "correct_sentence": "여섯시? 너무 일찍 등교하는 거 아냐?",
   "domain": "일상대화",
   "error_sentence": "<e1>육시?</e1> 너무 일찍 등교하는 거 아냐?",
   "error_type": {
    "e1": "numerical"
   },
   "index": 13,
   "number of error": 1,
   "phrase": 6,
   "style": "conversation",
   "syllable": 16
  }

## License
