# Position-Bias-LLMs

## Pegasus

Main code is in script.py
Command to run script:


```
python script.py --dataset dataset_name --batch_size batch-size --device device# --model model_name

```
Replace dataset_name with either cnn, xsum, news, reddit 
Replace batch-size with number
Replace batch-size with device#
Replace model_name with either the huggingface model name or the local finetuned model name

## Bart

Main code is in script.py
Command to run script:


```
python script.py --dataset dataset_name --batch_size batch-size --device device# --model model_name

```
Replace dataset_name with either cnn, xsum, news, reddit 
Replace batch-size with number
Replace batch-size with device#
Replace model_name with either the huggingface model name or the local finetuned model name

## Dolly-v2-7b

Inference the LLM with simply running data_collection.py.

Main code is in script.py
Command to run script:


```
python script.py --dataset dataset_name --batch_size batch-size --device device# 

```
Replace dataset_name with either cnn, xsum, news, reddit 
Replace batch-size with number
Replace batch-size with device#


## ChatGPT 3.5-T

Inference the LLM with running inference.ipynb
You will need to add a azure-configuration.json that has the Azure OpenAI endpoints.

Main code is in script.py
Command to run script:

```
python script.py --dataset dataset_name --batch_size batch-size --device device# 

```
Replace dataset_name with either cnn, xsum, news, reddit 
Replace batch-size with number
Replace batch-size with device#

## Llama-13b-chat

You will need to download and copy the Llama folder from meta with the weights to the directory first.
Inference can be done by running the file inference_13b_chat.py with the following command.

```
torchrun --nproc_per_node 2 inference_13b_chat.py \
    --ckpt_dir llama-2-13b-chat/ \
    --tokenizer_path tokenizer.model \
    --max_seq_len 2000 --max_batch_size 4
```

Main code is in script.py
Command to run script:

```
python script.py --dataset dataset_name --batch_size batch-size --device device# 

```
Replace dataset_name with either cnn, xsum, news, reddit 
Replace batch-size with number
Replace batch-size with device#


