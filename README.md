# GENERATIVE-TEXT-MODAL

COMPANY - CODTECH IT SOLUTION

NAME - SIPRA SHARMA

INTERN ID - CT06DG741

DOMAIN - ARTIFICIAL INTELLIGENCE 

DURATION - 6 WEEKS

MENTOR - NEELA SANTOSH

DESCRIPTION - This Python code demonstrates how to perform text generation using a pre-trained language model from the Hugging Face Transformers library. The main objective of the code is to take a given input prompt (a sentence or phrase) and have the model generate a continuation of that text. Text generation is a key application of natural language processing where a model predicts the most likely sequence of words that can follow a given input. The function generate_text is defined to handle this entire process, from preprocessing the input text to decoding the model’s output back into readable language.

The function takes four parameters: the pre-trained model, the tokenizer, the text prompt, and optional settings like max_length (maximum number of tokens to be generated) and num_return_sequences (number of generated outputs to return). The tokenizer is first used to convert the input prompt into a format the model understands—specifically, it transforms the string into numerical tokens using the tokenizer’s vocabulary and returns it as a PyTorch tensor using return_tensors="pt". Since models typically run on a specific device (like a GPU or CPU), the input tokens are moved to the same device using .to(model.device) to ensure compatibility during computation.

Next, the model’s generate() function is called to produce the continuation text. Several arguments are passed to control generation behavior. For instance, no_repeat_ngram_size=2 prevents the model from repeating the same phrases, leading to more natural text. The early_stopping=True argument stops the generation once an end-of-sequence (EOS) token is encountered, avoiding overly long or nonsensical outputs. Both eos_token_id and pad_token_id are passed from the tokenizer to ensure correct interpretation of where the sequence should end and how padding is handled.

Once the model generates token IDs for the new sequence, the tokenizer.batch_decode() function is used to convert those token IDs back into human-readable text. The skip_special_tokens=True option ensures that formatting tokens like <eos> or <pad> are removed from the output. Finally, the generated text is printed, showcasing what the model predicted based on the initial prompt.

In summary, this code is a compact and effective implementation of text generation using transformer-based language models. It handles all essential parts of the process: encoding input, generating predictions, decoding output, and customizing the behavior of text generation using multiple configurable options. It serves as a useful foundation for developing advanced applications like AI storytelling, chatbots, or automated writing systems.


OTUPUT- The following generation flags are not valid and may be ignored: ['early_stopping']. Set `TRANSFORMERS_VERBOSITY=info` for more details.
The attention mask is not set and cannot be inferred from input because pad token is same as eos token. As a consequence, you may observe unexpected behavior. Please pass your input's `attention_mask` to obtain reliable results.
Generated Text:
The arena was a dangerous place to be.

"I'm not going to let you down," he said. "I know you're going through a lot of things, but I'm going out there and I want to make sure you get through it."
.@Randy_Bennett: "We're not gonna let this happen to you." pic.twitter.com/QJ6XJXq9XV — The Athletic (@TheAthletics) August 19, 2017
, the first of three games between the two teams. The first game was played at the Coliseum on Saturday, August 20. It was the second game between them. Both teams will play in the same game on Sunday, Aug. 21.










