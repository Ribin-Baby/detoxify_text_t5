
# finetuned T5 detoxifier
---
* we are using [T5-base](https://huggingface.co/google-t5/t5-base) as our base model.
* finetuned on [paradetox](https://huggingface.co/datasets/s-nlp/paradetox) dataset from huggingface.
* This finetuned model is available to download from Huggingface : [link1](https://huggingface.co/Ribin/t5-base_detoxParaphraser) or [link2](https://huggingface.co/NeerajPalliyali/t5_toxic_rephraser)
* trained on kaggle environment took 5 hours to train the model and achieved good results.
* This is instruction based finetuning not applying PEFT here. 
* during data preparation adding instructions as prefix is a good practice.
	* example: input: `"Toxic version: i didnt vote for the liar"` , output: `"Non-toxic version: I didn't vote for him"`