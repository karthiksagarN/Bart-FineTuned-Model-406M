# Bart-FineTuned-Model-406M
FineTuned facebook's BART-Model with 406 M parameters

Check out the HuggingFace Repository -
https://huggingface.co/karthiksagarn/bart-samsum-finetuned

This model is a fine-tuned version of facebook/bart-large-cnn on the samsum dataset. It achieves the following results on the evaluation set:
Loss: 0.1326

<img width="643" alt="Screenshot 2024-03-19 at 2 30 59 AM" src="https://github.com/karthiksagarN/Bart-FineTuned-Model-406M/assets/111840048/6fb6eb20-b8b2-409d-8ec0-e71f923c0300">

Training hyperparameters
The following hyperparameters were used during training:

learning_rate: 1e-05
train_batch_size: 8
eval_batch_size: 8
seed: 42
optimizer: Adam with betas=(0.9,0.999) and epsilon=1e-08
lr_scheduler_type: linear
lr_scheduler_warmup_steps: 100
num_epochs: 3

ROUGE SCORES:

<img width="689" alt="Screenshot 2024-03-19 at 3 31 44 AM" src="https://github.com/karthiksagarN/Bart-FineTuned-Model-406M/assets/111840048/1ad53794-5e2d-40b8-9ac9-8ac05e161e6a">

BERT SCORE:

<img width="233" alt="Screenshot 2024-03-19 at 4 14 39 AM" src="https://github.com/karthiksagarN/Bart-FineTuned-Model-406M/assets/111840048/7117805e-a711-45ec-af35-e8646af21cfb">


Framework versions
Transformers - 4.38.2
Pytorch - 2.2.1+cu121
Datasets - 2.18.0
Tokenizers - 0.15.2
