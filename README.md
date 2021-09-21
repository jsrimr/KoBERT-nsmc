# KoBERT-nsmc

- sentiment classification using KoBERT
- used 🤗`Huggingface Tranformers`🤗 library

## Dependencies

- torch==1.4.0
- transformers==2.10.0

## How to use

To check the base flow, Please refer to this [Train_and_Eval.ipynb](notebook)

Also, you can check basic hugging-face usage in this [HuggingFace Practice.ipynb](notebook)

## Usage

```bash
$ python3 main.py --model_type kobert --do_train --do_eval
```

## Prediction

```bash
$ python3 predict.py --input_file {INPUT_FILE_PATH} --output_file {OUTPUT_FILE_PATH} --model_dir {SAVED_CKPT_PATH}
```

## Results
|                   | Accuracy (%) |
| ----------------- | ------------ |
| KoBERT            | **89.63**    |


## References

- [KoBERT](https://github.com/SKTBrain/KoBERT)
- [Huggingface Transformers](https://github.com/huggingface/transformers)
- [NSMC dataset](https://github.com/e9t/nsmc)
