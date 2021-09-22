# KoBERT-nsmc

- sentiment classification using KoBERT
- used 🤗`Huggingface Tranformers`🤗 library
- for more explanation, please visit https://medium.com/@jsrimr2/classifying-movie-reviews-in-your-language-using-hugging-face-model-9197eaea669d

## Branches
- using alternative model(kykim_model) : features/kykim_model
- using alternative preprocessing method : features/preprocessing

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
you can check visulized results on
https://app.neptune.ai/jeffrey/nsmc/experiments?compare=EwBgNAzGCMQ&split=tbl&dash=charts&viewId=standard-view&sortBy=%5B%22sys%2Fcreation_time%22%5D&sortFieldType=%5B%22datetime%22%5D&sortFieldAggregationMode=%5B%22auto%22%5D&sortDirection=%5B%22descending%22%5D&suggestionsEnabled=false&lbViewUnpacked=true

|                   | Accuracy (%) |
| ----------------- | ------------ |
| KoBERT            | **89.63**    |


## References

- [KoBERT](https://github.com/SKTBrain/KoBERT)
- [Huggingface Transformers](https://github.com/huggingface/transformers)
- [NSMC dataset](https://github.com/e9t/nsmc)
