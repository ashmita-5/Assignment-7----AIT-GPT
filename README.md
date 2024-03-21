# NLP Assignment-7----AIT-GPT

## Student Info

Ashmita Phuyal(124454)

### Task 1: Source Discovery <br>

### Source: 

For our dataset, we employed web scraping to gather information from various sources, including the official AIT website and other relevant webpages. Additionally, we incorporated data from the AIT brochure PDF file. Furthermore, we included the AIT brochure PDF file in our dataset, extracting information from its contents to enrich our data pool.

## Prompt template: 

The prompt template I used:

"   Hello there! I'm AITBot, your helpful virtual assistant ready to answer any queries
    you might have about the Asian Institute of Technology (AIT).
    Whether you're seeking information about AIT, its array of programs and courses,
    or any related topic, feel free to ask away!
    Simply share your questions with me,
    and I'll provide you with the guidance you need."

### Task 2. Analysis and Problem Solving

For comparing the model performance, we have used T5 model (fastchat-t5-3b-v1.0) and GPT2 model (gpt2-finetuned-cnn-summarization-v1) from Huggingface.

### T5 Model:

The T5 Fast model, a large model of approximately 6.5GB, demonstrates excellent performance due to its extensive training data, providing highly accurate answers to most questions. However, it occasionally lacks in returning related documents, likely because its vast knowledge surpasses the database's scope. 

### GPT2 Model:

On the other hand, the GPT2 Finetuned model, smaller at around 500MB, shows reduced performance compared to T5. This model, based on a decoder architecture, often retrieves answers from the limited database, impacting its overall performance. 

Despite limitations in database size and computational resources, the GPT2 model was selected for its faster inference capabilities, suitable for a web application. 

### Issues

Regarding unrelated information issues, the T5 model generally offers related information, while the GPT model tends to provide answers that match parts of the question without conveying the question's semantic meaning. To address this, enhancing the database's size and quality, along with refining prompt templates to align better with the model's training data, could improve the GPT model's performance in delivering relevant responses.
