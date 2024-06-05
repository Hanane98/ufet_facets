# Ultra fine entity typing

## 1. Training
'''
python ./src/domain_model/main.py -lr 2e-5 -train_batch_size 16 -test_batch_size 16 -bert_version ./bert-base-cased -multitask -tune_all -do_train -optim_th -model_id bert_base_cased_facets_min_clus-5_domain_types_chatgpt_bert-base-uncased_2e-05_20_0.07 -d_goal facets_cluster -dfn_postfix min_clus-5_domain_types_chatgpt_bert-base-uncased_2e-05_20_0.07 -dfc_param facets_clusters20240125\bert_base_cased_dfc_min_clus-5_domain_types_chatgpt_bert-base-uncased_2e-05_20_0.07.pt
'''

## 2. Testing
```
python ./src/domain_model/main.py -train_batch_size 16 -test_batch_size 16 -bert_version ./bert-base-cased -multitask -optim_th -model_id bert_base_cased_facets_min_clus-5_domain_types_chatgpt_bert-base-uncased_2e-05_20_0.07 -d_goal facets_cluster -dfn_postfix min_clus-5_domain_types_chatgpt_bert-base-uncased_2e-05_20_0.07 -dfc_param facets_clusters20240125\bert_base_cased_dfc_min_clus-5_domain_types_chatgpt_bert-base-uncased_2e-05_20_0.07.pt
```


