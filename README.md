# Multi-Turn Response Selection in Retrieval-Based Chatbots

Multi-turn response selection in retrieval-based chatbots is a task which aims to select the best-matched response from a set of candidates, given the context of a conversation. This task is attracting more and more attention in academia and industry. However, no one has maintained a leaderboard and a collection of popular papers and datasets yet. The main objective of this repository is to provide the reader with a quick overview of benchmark datasets and the state-of-the-art studies on this task, which serves as a stepping stone for further research. 


## Datasets

### Ubuntu Dialogue Corpus V1

- [Lowe et al. (2015)](https://www.aclweb.org/anthology/W15-4640.pdf) released the original version. [[Download]](https://github.com/npow/ubottu) <br>
- [Xu et al. (2016)](https://arxiv.org/pdf/1605.05110.pdf) released a version in which numbers, paths and URLs were replaced by placeholders. [[Download]](https://www.dropbox.com/s/2fdn26rj6h9bpvl/ubuntu_data.zip) <br>
- [Gu et al. (2019)](https://dl.acm.org/citation.cfm?id=3358140) released a version based on Xu et al. (2016) in which contexts and responses are assigned ids to track them. [[Download]](https://drive.google.com/file/d/1-rNv34hLoZr300JF3v7nuLswM7GRqeNc/view)

### Ubuntu Dialogue Corpus V2

- [Lowe et al. (2017)](http://dad.uni-bielefeld.de/index.php/dad/article/view/3698) released the original version. [[Download]](https://github.com/rkadlec/ubuntu-ranking-dataset-creator) <br>
- [Gu et al. (2019)](https://dl.acm.org/citation.cfm?id=3358140) released a version in which contexts and responses are assigned ids to track them. [[Download]](https://drive.google.com/file/d/1tS_VC47z8CVPr-tZu0U4JEEwBT04N6ks/view)

### Douban Conversation Corpus

- [Wu et al. (2017)](https://www.aclweb.org/anthology/P17-1046.pdf) released the original version. [[Download]](https://github.com/MarkWuNLP/MultiTurnResponseSelection) <br>
- [Gu et al. (2019)](https://dl.acm.org/citation.cfm?id=3358140) released a version in which contexts and responses are assigned ids to track them. [[Download]](https://drive.google.com/file/d/1Cwt5BC_WDr1N_-TYaOMSHuOXLKAxXoMQ/view)

### E-commerce Corpus

- [Zhang et al. (2018)](https://www.aclweb.org/anthology/C18-1317.pdf) released the original version. [[Download]](https://drive.google.com/file/d/154J-neBo20ABtSmJDvm7DK0eTuieAuvw/view) <br>
- [Gu et al. (2019)](https://dl.acm.org/citation.cfm?id=3358140) released a version in which contexts and responses are assigned ids to track them. [[Download]](https://drive.google.com/file/d/1vy2bcTCLm1Dzsdvh0cvPIw0XzrTK06us/view)



## Leaderboard

### Ubuntu Dialogue Corpus V1

| Model                    |  R_2@1  |  R_10@1  |  R_10@2  |  R_10@5  |  Paper and Code  |
| ------------------------ | ------- | -------- | -------- | -------- | ---------------- |
| BERT-FP (Han et al., 2021)| -      |  0.911   |  0.962   |  0.994   | Fine-grained Post-training for Improving Retrieval-based Dialogue Systems. NAACL 2021. [[paper]](https://www.aclweb.org/anthology/2021.naacl-main.122.pdf) [[code]](https://github.com/hanjanghoon/BERT_FP) |
| BERT-SL (Xu et al., 2021)| 0.975   |  0.884   |  0.946   |  0.990   | Learning an Effective Context-Response Matching Model with Self-Supervised Tasks for Retrieval-based Dialogues. AAAI 2021. [[paper]](https://arxiv.org/pdf/2009.06265.pdf) |
| UMS_BERT+ (Whang et al., 2021) | - |  0.875   |  0.942   |  0.988   | Do Response Selection Models Really Know What’s Next? Utterance Manipulation Strategies for Multi-turn Response Selection. AAAI 2021. [[paper]](https://arxiv.org/pdf/2009.04703.pdf) [[code]](https://github.com/taesunwhang/UMS-ResSel) |
| BERT-SPIDER (Zhang et al., 2021)| - | 0.869   |  0.938   |  0.987   | Structural Pre-training for Dialogue Comprehension. ACL 2021. [[paper]](https://arxiv.org/pdf/2105.10956.pdf) [[code]](https://github.com/cooelf/SPIDER) |
| SA-BERT+HCL (Su et al., 2021) | 0.977 | 0.867 |  0.940   |  0.992   | Dialogue Response Selection with Hierarchical Curriculum Learning. ACL 2021. [[paper]](https://arxiv.org/pdf/2012.14756.pdf) [[code]](https://github.com/yxuansu/HCL/) |
| DCM (Li et al., 2020)    |    -    |  0.868   |  0.936   |  0.987   | Deep context modeling for multi-turn response selection in dialogue systems. Information Processing & Management 2020. [[paper]](https://www.sciencedirect.com/science/article/pii/S0306457320309109?casa_token=H6-Tl7WVdycAAAAA:u1ncofokUVOFK-VZacatzgEDUtYEDggjEV5cXonnHjQQgdaGTt7qNMnX04eYJzvRr71Uf_ZIUcaj) [[code]](https://github.com/LeaLiLu/DeepContextModeling) |
| SA-BERT (Gu et al., 2020) |  0.965 |  0.855   |  0.928   |  0.983   | Speaker-Aware BERT for Multi-Turn Response Selection in Retrieval-Based Chatbots. CIKM 2020. [[paper]](https://arxiv.org/pdf/2004.03588.pdf) [[code]](https://github.com/JasonForJoy/SA-BERT) |
| BERT-VFT (Whang et al., 2019)| -   |  0.855   |  0.928   |  0.985   | An Effective Domain Adaptive Post-Training Method for BERT in Response Selection. INTERSPEECH 2020. [[paper]](https://arxiv.org/pdf/1908.04812.pdf) [[code]](https://github.com/taesunwhang/BERT-ResSel) |
| RoBERTa-BASE-SS-DA (Lu et al., 2020)| 0.955| 0.826| 0.909|  0.978   | Improving Contextual Language Models for Response Retrieval in Multi-Turn Conversation. SIGIR 2020. [[paper]](https://dl.acm.org/doi/10.1145/3397271.3401255) [[code]](https://github.com/CSLujunyu/Improving-Contextual-Language-Modelsfor-Response-Retrieval-in-Multi-Turn-Conversation) |
| TADAM (Xu et al., 2020)  |    -    |  0.821   |  0.906   |  0.978   | Topic-Aware Multi-turn Dialogue Modeling. AAAI 2021. [[paper]](https://arxiv.org/pdf/2009.12539.pdf) [[code]](https://github.com/xyease/TADAM) |
| G-MSN (Lin et al., 2020) |  0.958  |  0.812   |  0.911   |  0.987   | The World is Not Binary: Learning to Rank with Grayscale Data for Dialogue Response Selection. EMNLP 2020. [[paper]](https://arxiv.org/pdf/2004.02421.pdf) |
| MSN (Yuan et al., 2019)  |    -    |  0.800   |  0.899   |  0.978   | Multi-hop Selector Network for Multi-turn Response Selection in Retrieval-based Chatbots. EMNLP 2019. [[paper]](https://www.aclweb.org/anthology/D19-1011.pdf) [[code]](https://github.com/chunyuanY/Dialogue) |
| IOI (Tao et al., 2019)   |  0.947  |  0.796   |  0.894   |  0.974   | One Time of Interaction May Not Be Enough: Go Deep with an Interaction-over-Interaction Network for Response Selection in Dialogues. ACL 2019. [[paper]](https://www.aclweb.org/anthology/P19-1001.pdf) [[code]](https://github.com/chongyangtao/IOI) |
| IMN (Gu et al., 2019)    |  0.946  |  0.794   |  0.889   |  0.974   | Interactive Matching Network for Multi-Turn Response Selection in Retrieval-Based Chatbots. CIKM 2019. [[paper]](https://arxiv.org/pdf/1901.01824.pdf) [[code]](https://github.com/JasonForJoy/IMN) |
| U2U-IMN (Gu et al., 2019)|  0.945  |  0.790   |  0.886   |  0.973   | Utterance-to-Utterance Interactive Matching Network for Multi-Turn Response Selection in Retrieval-Based Chatbots. TASLP 2019. [[paper]](https://arxiv.org/pdf/1911.06940.pdf) [[code]](https://github.com/JasonForJoy/U2U-IMN) |
| MRFN (Tao et al., 2019)  |  0.945  |  0.786   |  0.886   |  0.976   | Multi-Representation Fusion Network for Multi-Turn Response Selection in Retrieval-Based Chatbots. WSDM 2019. [[paper]](https://dl.acm.org/doi/10.1145/3289600.3290985) [[code]](https://github.com/chongyangtao/MRFN) |
| IACMN (Wang et al., 2019)|  0.944  |  0.782   |  0.886   |  0.973   | Multi-Turn Response Selection in Retrieval-Based Chatbots with Iterated Attentive Convolution Matching Network. CIKM 2019. [[paper]](https://dl.acm.org/doi/10.1145/3357384.3357928) [[code]](https://github.com/heyuanw/IACMN) |
| DAM (Zhou et al., 2018)  |  0.938  |  0.767   |  0.874   |  0.969   | Multi-Turn Response Selection for Chatbots with Deep Attention Matching Network. ACL 2018. [[paper]](https://www.aclweb.org/anthology/P18-1103.pdf) [[code]](https://github.com/baidu/Dialogue/tree/master/DAM) |
| DUA (Zhang et al., 2018) |  -      |  0.752   |  0.868   |  0.962   | Modeling Multi-Turn Conversation with Deep Utterance Aggregation. COLING 2018. [[code]](https://github.com/cooelf/DeepUtteranceAggregation) |
| SMN (Wu et al., 2017)    |  0.926  |  0.726   |  0.847   |  0.961   | Sequential Matching Network: A New Architecture for Multi-Turn Response Selection in Retrieval-Based Chatbots. ACL 2017. [[paper]](https://www.aclweb.org/anthology/P17-1046.pdf) [[code]](https://github.com/MarkWuNLP/MultiTurnResponseSelection) |


### Ubuntu Dialogue Corpus V2

| Model                        |  R_2@1  |  R_10@1  |  R_10@2  |  R_10@5  |  Paper and Code  |
| ---------------------------- | ------- | -------- | -------- | -------- | ---------------- |
| Cross-encoder (Humeau et al., 2020)| - |  0.865   |  -       |  0.991   | Poly-encoders: Transformer Architectures and Pre-training Strategies for Fast and Accurate Multi-sentence Scoring. ICLR 2020. [[paper]](https://openreview.net/pdf?id=SkxgnnNFvH) [[code]](https://github.com/sfzhou5678/PolyEncoder) |
| Thread-bi (Jia et al., 2020) |  -      |  0.838   |  0.924   |  0.985   | Multi-turn Response Selection using Dialogue Dependency Relations. EMNLP 2020. [[paper]](https://www.aclweb.org/anthology/2020.emnlp-main.150.pdf) [[code]](https://github.com/JiaQiSJTU/ResponseSelection) |
| SA-BERT (Gu et al., 2020)    |  0.963  |  0.830   |  0.919   |  0.985   | Speaker-Aware BERT for Multi-Turn Response Selection in Retrieval-Based Chatbots. CIKM 2020. [[paper]](https://arxiv.org/pdf/2004.03588.pdf) [[code]](https://github.com/JasonForJoy/SA-BERT) |
| IMN (Gu et al., 2019)        |  0.945  |  0.771   |  0.886   |  0.979   | Interactive Matching Network for Multi-Turn Response Selection in Retrieval-Based Chatbots. CIKM 2019. [[paper]](https://arxiv.org/pdf/1901.01824.pdf) [[code]](https://github.com/JasonForJoy/IMN) |
| U2U-IMN (Gu et al., 2019)    |  0.943  |  0.762   |  0.877   |  0.975   | Utterance-to-Utterance Interactive Matching Network for Multi-Turn Response Selection in Retrieval-Based Chatbots. TASLP 2019. [[paper]](https://arxiv.org/pdf/1911.06940.pdf) [[code]](https://github.com/JasonForJoy/U2U-IMN) |
| HRDE-LTC (Yoon et al., 2018) |  0.915  |  0.652   |  0.815   |  0.966   | Learning to Rank Question-Answer Pairs using Hierarchical Recurrent Encoder with Latent Topic Clustering. NAACL 2018. [[paper]](https://www.aclweb.org/anthology/N18-1142.pdf) [[code]](https://github.com/david-yoon/QA_HRDE_LTC) |


### Douban Conversation Corpus

| Model                    |  MAP  |  MRR  |  P@1  |  R_10@1  |  R_10@2  |  R_10@5  |  Paper and Code  |
| ------------------------ | ----- | ----- | ----- | -------- | -------- | -------- | ---------------- |
| BERT-FP (Han et al., 2021)| 0.644| 0.680 | 0.512 |  0.324   |  0.542   |  0.870   | Fine-grained Post-training for Improving Retrieval-based Dialogue Systems. NAACL 2021. [[paper]](https://www.aclweb.org/anthology/2021.naacl-main.122.pdf) [[code]](https://github.com/hanjanghoon/BERT_FP) |
| SA-BERT+HCL (Su et al., 2021) | 0.639 | 0.681 | 0.514| 0.330| 0.531    |  0.858   | Dialogue Response Selection with Hierarchical Curriculum Learning. ACL 2021. [[paper]](https://arxiv.org/pdf/2012.14756.pdf) [[code]](https://github.com/yxuansu/HCL/) |
| UMS_BERT+ (Whang et al., 2020)| 0.625| 0.664| 0.499| 0.318  |  0.482   |  0.858   | Do Response Selection Models Really Know What’s Next? Utterance Manipulation Strategies for Multi-turn Response Selection. AAAI 2021. [[paper]](https://arxiv.org/pdf/2009.04703.pdf) [[code]](https://github.com/taesunwhang/UMS-ResSel) |
| SA-BERT (Gu et al., 2020)| 0.619 | 0.659 | 0.496 |  0.313   |  0.481   |  0.847   | Speaker-Aware BERT for Multi-Turn Response Selection in Retrieval-Based Chatbots. CIKM 2020. [[paper]](https://arxiv.org/pdf/2004.03588.pdf) [[code]](https://github.com/JasonForJoy/SA-BERT) |
| DCM (Li et al., 2020)    | 0.611 | 0.649 |   -   |  0.294   |  0.498   |  0.842   | Deep context modeling for multi-turn response selection in dialogue systems. Information Processing & Management 2020. [[paper]](https://www.sciencedirect.com/science/article/pii/S0306457320309109?casa_token=H6-Tl7WVdycAAAAA:u1ncofokUVOFK-VZacatzgEDUtYEDggjEV5cXonnHjQQgdaGTt7qNMnX04eYJzvRr71Uf_ZIUcaj) [[code]](https://github.com/LeaLiLu/DeepContextModeling) |
| BERT-SPIDER (Zhang et al., 2021)| 0.609| 0.650| 0.475| 0.296|  0.488   |  0.836   | Structural Pre-training for Dialogue Comprehension. ACL 2021. [[paper]](https://arxiv.org/pdf/2105.10956.pdf) [[code]](https://github.com/cooelf/SPIDER) |
| RoBERTa-BASE-SS-DA (Lu et al., 2020)| 0.602| 0.646| 0.460| 0.280| 0.495|  0.847   | Improving Contextual Language Models for Response Retrieval in Multi-Turn Conversation. SIGIR 2020. [[paper]](https://dl.acm.org/doi/10.1145/3397271.3401255) [[code]](https://github.com/CSLujunyu/Improving-Contextual-Language-Modelsfor-Response-Retrieval-in-Multi-Turn-Conversation) |
| G-MSN (Lin et al., 2020) | 0.599 | 0.645 | 0.476 |  0.308   |  0.468   |  0.826   | The World is Not Binary: Learning to Rank with Grayscale Data for Dialogue Response Selection. EMNLP 2020. [[paper]](https://arxiv.org/pdf/2004.02421.pdf) |
| TADAM (Xu et al., 2020)  | 0.594 | 0.633 | 0.453 |  0.282   |  0.472   |  0.828   | Topic-Aware Multi-turn Dialogue Modeling. AAAI 2021. [[paper]](https://arxiv.org/pdf/2009.12539.pdf) [[code]](https://github.com/xyease/TADAM) |
| MSN (Yuan et al., 2019)  | 0.587 | 0.632 | 0.470 |  0.295   |  0.452   |  0.788   | Multi-hop Selector Network for Multi-turn Response Selection in Retrieval-based Chatbots. EMNLP 2019. [[paper]](https://www.aclweb.org/anthology/D19-1011.pdf) [[code]](https://github.com/chunyuanY/Dialogue) |
| IOI (Tao et al., 2019)   | 0.573 | 0.621 | 0.444 |  0.269   |  0.451   |  0.786   | One Time of Interaction May Not Be Enough: Go Deep with an Interaction-over-Interaction Network for Response Selection in Dialogues. ACL 2019. [[paper]](https://www.aclweb.org/anthology/P19-1001.pdf) [[code]](https://github.com/chongyangtao/IOI) |
| IACMN (Wang et al., 2019)| 0.571 | 0.621 | 0.448 |  0.269   |  0.453   |  0.783   | Multi-Turn Response Selection in Retrieval-Based Chatbots with Iterated Attentive Convolution Matching Network. CIKM 2019. [[paper]](https://dl.acm.org/doi/10.1145/3357384.3357928) [[code]](https://github.com/heyuanw/IACMN) |
| MRFN (Tao et al., 2019)  | 0.571 | 0.617 | 0.448 |  0.276   |  0.435   |  0.783   | Multi-Representation Fusion Network for Multi-Turn Response Selection in Retrieval-Based Chatbots. WSDM 2019. [[paper]](https://dl.acm.org/doi/10.1145/3289600.3290985) [[code]](https://github.com/chongyangtao/MRFN) |
| IMN (Gu et al., 2019)    | 0.570 | 0.615 | 0.433 |  0.262   |  0.452   |  0.789   | Interactive Matching Network for Multi-Turn Response Selection in Retrieval-Based Chatbots. CIKM 2019. [[paper]](https://arxiv.org/pdf/1901.01824.pdf) [[code]](https://github.com/JasonForJoy/IMN) |
| U2U-IMN (Gu et al., 2019)| 0.564 | 0.611 | 0.429 |  0.259   |  0.430   |  0.791   | Utterance-to-Utterance Interactive Matching Network for Multi-Turn Response Selection in Retrieval-Based Chatbots. TASLP 2019. [[paper]](https://arxiv.org/pdf/1911.06940.pdf) [[code]](https://github.com/JasonForJoy/U2U-IMN) |
| DAM (Zhou et al., 2018)  | 0.550 | 0.601 | 0.427 |  0.254   |  0.410   |  0.757   | Multi-Turn Response Selection for Chatbots with Deep Attention Matching Network. ACL 2018. [[paper]](https://www.aclweb.org/anthology/P18-1103.pdf) [[code]](https://github.com/baidu/Dialogue/tree/master/DAM) |
| DUA (Zhang et al., 2018) | 0.551 | 0.599 | 0.421 |  0.243   |  0.421   |  0.780   | Modeling Multi-Turn Conversation with Deep Utterance Aggregation. COLING 2018. [[code]](https://github.com/cooelf/DeepUtteranceAggregation) |
| SMN (Wu et al., 2017)    | 0.529 | 0.569 | 0.397 |  0.233   |  0.396   |  0.724   | Sequential Matching Network: A New Architecture for Multi-Turn Response Selection in Retrieval-Based Chatbots. ACL 2017. [[paper]](https://www.aclweb.org/anthology/P17-1046.pdf) [[code]](https://github.com/MarkWuNLP/MultiTurnResponseSelection) |


### E-commerce Corpus

| Model                    |  R_10@1  |  R_10@2  |  R_10@5  |  Paper and Code  |
| ------------------------ | -------- | -------- | -------- | ---------------- |
| BERT-FP (Han et al., 2021)| 0.870   |  0.956   |  0.993   | Fine-grained Post-training for Improving Retrieval-based Dialogue Systems. NAACL 2021. [[paper]](https://www.aclweb.org/anthology/2021.naacl-main.122.pdf) [[code]](https://github.com/hanjanghoon/BERT_FP) |
| BERT-SL (Xu et al., 2020)|  0.776   |  0.919   |  0.991   | Learning an Effective Context-Response Matching Model with Self-Supervised Tasks for Retrieval-based Dialogues. AAAI 2021. [[paper]](https://arxiv.org/pdf/2009.06265.pdf) |
| UMS_BERT+ (Whang et al., 2020) |0.762| 0.905   |  0.986   | Do Response Selection Models Really Know What’s Next? Utterance Manipulation Strategies for Multi-turn Response Selection. AAAI 2021. [[paper]](https://arxiv.org/pdf/2009.04703.pdf) [[code]](https://github.com/taesunwhang/UMS-ResSel) |
| SA-BERT+HCL (Su et al., 2021) | 0.721 | 0.896  |  0.993   | Dialogue Response Selection with Hierarchical Curriculum Learning. ACL 2021. [[paper]](https://arxiv.org/pdf/2012.14756.pdf) [[code]](https://github.com/yxuansu/HCL/) |
| BERT-SPIDER (Zhang et al., 2021)| 0.708 | 0.853|  0.986   | Structural Pre-training for Dialogue Comprehension. ACL 2021. [[paper]](https://arxiv.org/pdf/2105.10956.pdf) [[code]](https://github.com/cooelf/SPIDER) |
| SA-BERT (Gu et al., 2020)|  0.704   |  0.879   |  0.985   | Speaker-Aware BERT for Multi-Turn Response Selection in Retrieval-Based Chatbots. CIKM 2020. [[paper]](https://arxiv.org/pdf/2004.03588.pdf) [[code]](https://github.com/JasonForJoy/SA-BERT) |
| DCM (Li et al., 2020)    |  0.685   |  0.864   |  0.982   | Deep context modeling for multi-turn response selection in dialogue systems. Information Processing & Management 2020. [[paper]](https://www.sciencedirect.com/science/article/pii/S0306457320309109?casa_token=H6-Tl7WVdycAAAAA:u1ncofokUVOFK-VZacatzgEDUtYEDggjEV5cXonnHjQQgdaGTt7qNMnX04eYJzvRr71Uf_ZIUcaj) [[code]](https://github.com/LeaLiLu/DeepContextModeling) |
| TADAM (Xu et al., 2020)  |  0.660   |  0.834   |  0.975   | Topic-Aware Multi-turn Dialogue Modeling. AAAI 2021. [[paper]](https://arxiv.org/pdf/2009.12539.pdf) [[code]](https://github.com/xyease/TADAM) |
| RoBERTa-BASE-SS-DA (Lu et al., 2020)| 0.627| 0.835| 0.980 | Improving Contextual Language Models for Response Retrieval in Multi-Turn Conversation. SIGIR 2020. [[paper]](https://dl.acm.org/doi/10.1145/3397271.3401255) [[code]](https://github.com/CSLujunyu/Improving-Contextual-Language-Modelsfor-Response-Retrieval-in-Multi-Turn-Conversation) |
| IMN (Gu et al., 2019)    |  0.621   |  0.797   |  0.964   | Interactive Matching Network for Multi-Turn Response Selection in Retrieval-Based Chatbots. CIKM 2019. [[paper]](https://arxiv.org/pdf/1901.01824.pdf) [[code]](https://github.com/JasonForJoy/IMN) |
| U2U-IMN (Gu et al., 2019)|  0.616   |  0.806   |  0.966   | Utterance-to-Utterance Interactive Matching Network for Multi-Turn Response Selection in Retrieval-Based Chatbots. TASLP 2019. [[paper]](https://arxiv.org/pdf/1911.06940.pdf) [[code]](https://github.com/JasonForJoy/U2U-IMN) |
| G-MSN (Lin et al., 2020) |  0.613   |  0.786   |  0.964   | The World is Not Binary: Learning to Rank with Grayscale Data for Dialogue Response Selection. EMNLP 2020. [[paper]](https://arxiv.org/pdf/2004.02421.pdf) |
| MSN (Yuan et al., 2019)  |  0.606   |  0.770   |  0.937   | Multi-hop Selector Network for Multi-turn Response Selection in Retrieval-based Chatbots. EMNLP 2019. [[paper]](https://www.aclweb.org/anthology/D19-1011.pdf) [[code]](https://github.com/chunyuanY/Dialogue) |
| IOI (Tao et al., 2019)   |  0.563   |  0.768   |  0.950   | One Time of Interaction May Not Be Enough: Go Deep with an Interaction-over-Interaction Network for Response Selection in Dialogues. ACL 2019. [[paper]](https://www.aclweb.org/anthology/P19-1001.pdf) [[code]](https://github.com/chongyangtao/IOI) |
| DUA (Zhang et al., 2018) |  0.501   |  0.700   |  0.921   | Modeling Multi-Turn Conversation with Deep Utterance Aggregation. COLING 2018. [[code]](https://github.com/cooelf/DeepUtteranceAggregation) |
| SMN (Wu et al., 2017)    |  0.453   |  0.654   |  0.886   | Sequential Matching Network: A New Architecture for Multi-Turn Response Selection in Retrieval-Based Chatbots. ACL 2017. [[paper]](https://www.aclweb.org/anthology/P17-1046.pdf) [[code]](https://github.com/MarkWuNLP/MultiTurnResponseSelection) |



## Papers
In addition to the studies mentioned above, there are stil a lot of great studies on multi-turn response selection worth reading. We list a part of them below. <br>

- **Distilling Knowledge for Fast Retrieval-based Chat-bots**. *Amir Vakili Tahami, Kamyar Ghajar, Azadeh Shakery*. SIGIR 2020.
- **Improving Matching Models with Hierarchical Contextualized Representations for Multi-turn Response Selection**. *Chongyang Tao, Wei Wu, Yansong Feng, Dongyan Zhao, Rui Yan*. SIGIR 2020.
- **Conversational Word Embedding for Retrieval-Based Dialog System**. *Wentao Ma, Yiming Cui, Ting Liu, Dong Wang, ShijinWang, Guoping Hu*. ACL 2020.
- **IART: Intent-aware Response Ranking with Transformers in Information-seeking Conversation Systems**. *Liu Yang, Minghui Qiu, Chen Qu, Cen Chen, Jiafeng Guo, Yongfeng Zhang, W. Bruce Croft, Haiqing Chen*. WWW 2020.
- **Dually Interactive Matching Network for Personalized Response Selection in Retrieval-Based Chatbots**. *Jia-Chen Gu, Zhen-Hua Ling, Xiaodan Zhu, Quan Liu*. EMNLP 2019.
- **Sampling Matters! An Empirical Study of Negative Sampling Strategies for Learning of Matching Models in Retrieval-based Dialogue Systems**. *Jia Li, Chongyang Tao, wei wu, Yansong Feng, Dongyan Zhao, Rui Yan*. EMNLP 2019.
- **Learning a Matching Model with Co-teaching for Multi-turn Response Selection in Retrieval-based Dialogue Systems**. *Jiazhan Feng, Chongyang Tao, Wei Wu, Yansong Feng, Dongyan Zhao, Rui Yan*. ACL 2019.
- **Training Neural Response Selection for Task-Oriented Dialogue Systems**. *Matthew Henderson, Ivan Vulić, Daniela Gerz, Iñigo Casanueva, Paweł Budzianowski, Sam Coope, Georgios Spithourakis, Tsung-Hsien Wen, Nikola Mrkšić, Pei-Hao Su*. ACL 2019.
- **DSTC7 Task 1: Noetic End-to-End Response Selection**. *Chulaka Gunasekara, Jonathan K. Kummerfeld, Lazaros Polymenakos, Walter Lasecki*. ACL 2019 Workshop.
- **A Document-grounded Matching Network for Response Selection in Retrieval-based Chatbots**. *Xueliang Zhao, Chongyang Tao, Wei Wu, Can Xu, Dongyan Zhao, Rui Yan*. IJCAI 2019.
- **Sequential Attention-based Network for Noetic End-to-End Response Selection**. *Qian Chen, Wen Wang*. AAAI 2019 Workshop on DSTC 7.
- **Building Sequential Inference Models for End-to-End Response Selection**. *Jia-Chen Gu, Zhen-Hua Ling, Yuping Ruan, Quan Liu*. AAAI 2019 Workshop on DSTC 7.
- **Training Millions of Personalized Dialogue Agents**. *Pierre-Emmanuel Mazaré, Samuel Humeau, Martin Raison, Antoine Bordes*. EMNLP 2018.
- **Personalizing Dialogue Agents: I have a dog, do you have pets too?**. *Saizheng Zhang, Emily Dinan, Jack Urbanek, Arthur Szlam, Douwe Kiela, Jason Weston*. ACL 2018.
- **Learning Matching Models with Weak Supervision for Response Selection in Retrieval-based Chatbots**. *Yu Wu, Wei Wu, Zhoujun Li, Ming Zhou*. ACL 2018.
- **Response Ranking with Deep Matching Networks and External Knowledge in Information-seeking Conversation Systems**. *Liu Yang, Minghui Qiu, Chen Qu, Jiafeng Guo, Yongfeng Zhang, W. Bruce Croft, Jun Huang, Haiqing Chen*. SIGIR 2018.
- **Improving Response Selection in Multi-turn Dialogue Systems by Incorporating Domain Knowledge**. *Debanjan Chaudhuri, Agustinus Kristiadi, Jens Lehmann, Asja Fischer*. CONLL 2018.
- **Enhance word representation for out-of-vocabulary on Ubuntu dialogue corpus**. *Jianxiong Dong, Jim Huang*. ArXiv.
- **Multi-view Response Selection for Human-Computer Conversation**. *Xiangyang Zhou, Daxiang Dong, Hua Wu, Shiqi Zhao, Dianhai Yu, Hao Tian, Xuan Liu, Rui Yan*. EMNLP 2016.
- **Learning to Respond with Deep Neural Networks for Retrieval-Based Human-Computer Conversation System**. *Rui Yan, Yiping Song, Hua Wu*. SIGIR 2016.



## Update
Although we work very hard to list more work, the studies we select to present in this repository are by no means complete. To this end, we welcome more people to participate in the maintenance of this project. Please feel free to open issues, pull requests or contact us (gujc@mail.ustc.edu.cn).
