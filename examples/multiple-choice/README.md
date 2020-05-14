#### Fine-tuning XLMRoberta on Stance Detection dataset
Term Project for ML 4 NLU Spring 2020

Team Members: Kailin Zheng, Andrew Lee, Daniel Chain


[ML for NLU: Project Proposal Ideas](https://docs.google.com/document/d/12sBCYTukK23mchlKxJwZbAb8vDIgQvKfEPZajhtlcFY/edit)

ML for NLU: Paper

[Fake News Challenge - 1 github repo](https://github.com/FakeNewsChallenge/fnc-1)

[WSDM 2019 - Chinese fake news detection dataset on Kaggle](https://www.kaggle.com/c/fake-news-pair-classification-challenge/data)


## Multiple Choice

Based on the script [`run_multiple_choice.py`]().

First, make sure you install torch

To run the script:
python ./examples/multiple-choice/run_multiple_choice.py \
--task_name stance \
--model_name_or_path xlm-roberta \
--do_train \
--do_eval \
--data_dir '' \
--learning_rate 5e-5 \
--num_train_epochs 3 \
--max_seq_length 80 \
--output_dir models_bert/swag_base \
--per_gpu_eval_batch_size=16 \
--per_gpu_train_batch_size=16 \
--gradient_accumulation_steps 2 \
--overwrite_output
