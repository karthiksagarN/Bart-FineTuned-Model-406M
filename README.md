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

ROUGE Scores:
{'rouge1': AggregateScore(low=Score(precision=0.29231890922960946, recall=0.5755340591660789, fmeasure=0.36452270126617037), mid=Score(precision=0.3012174062385683, recall=0.5880590685871268, fmeasure=0.3721959667623731), high=Score(precision=0.31083014490046085, recall=0.6010687364120285, fmeasure=0.38112972171463944)), 
'rouge2': AggregateScore(low=Score(precision=0.11850674794550704, recall=0.2418211034418429, fmeasure=0.14808409500530648), mid=Score(precision=0.12516700754290633, recall=0.2545193627452707, fmeasure=0.15550558913151516), high=Score(precision=0.13212297153452818, recall=0.26821321492196054, fmeasure=0.16319578693000844)), 'rougeL': AggregateScore(low=Score(precision=0.21821073377249478, recall=0.4433629225420538, fmeasure=0.2744300617502658), mid=Score(precision=0.2250875126650962, recall=0.454741311774031, fmeasure=0.2810128477652416), high=Score(precision=0.23278079521177517, recall=0.4679046460070841, fmeasure=0.2886331732350875)),
'rougeLsum': AggregateScore(low=Score(precision=0.21777541761772454, recall=0.4424980486533571, fmeasure=0.273913514415514), mid=Score(precision=0.2249069295700737, recall=0.45455346599643354, fmeasure=0.28065150515936815), high=Score(precision=0.2320842431711672, recall=0.4679183440028743, fmeasure=0.28834793775815465))}

Framework versions -
Transformers 4.38.2
Pytorch 2.2.1+cu121
Datasets 2.18.0
Tokenizers 0.15.2
