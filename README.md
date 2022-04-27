# Chinese_wwm

## Load the pre-train LM
1. download `Chinese_wmm` from [GitHub](https://github.com/ymcui/Chinese-BERT-wwm)
2. extract the files and paste them to `opennre/pretrain/chinese_wwm`
3. rename `bert_config.json` to `config.json`

# Train the Model

 ```
 python example/train_supervised_chinese_wwm.py \
     --pretrain_path {os.getcwd()}/OpenNRE/opennre/pretrain/chinese_wwm \
     --dataset people-relation
 ```

 The `ckpt` file will save in `OpenNRE/ckpt` folder.