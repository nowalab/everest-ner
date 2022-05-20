# EverestNER - The Benchmark Data Set for Nepali NER
We have created the largest human annotated Named Entity Recognition (NER) data set for Nepali available to date. Highlights: 

* EverestNER covers five named entities - Person Name, Location, Organization, Event and Date.
* EverestNER produces high quality annotations through clear annotation guidelines.
* EverestNER has 24,587 entities, 308,353 tokens corresponding to 15,798 sentences. 
* We split the EverestNER data set into EverestNER-train and EverestNER-test. These standard data sets, therefore, become the first benchmark data sets for evaluating Nepali NER systems. 
* We report a comprehensive evaluation of state-of-the-art Neural and Transformer models using these data sets. This is the first study to apply BERT model for mining Named Entities for Nepali.
* We also discuss the remaining challenges for discovering NEs for Nepali (see our paper below).

## Data Set Stats
|Data |Articles |Sentences |Tokens |Avg. Sent.Len| LOC| ORG| PER| EVT| DAT|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Train | 847| 13,848| 268,741| 19.40| 5,148| 4,756| 7,707| 312| 3,394|
|Test| 149| 1,950| 39,612| 20.31| 809| 715| 1,115| 59| 572| 
|Total| 996| 15,798| 308,353| 19.51| 5,957| 5,471| 8,822| 371| 3,966| 


## Data Format
The EverestNER data set is divided into train (EverestNER-train) and test (EverestNER-test) sets. Each data set has character level as well as token leven annotations. Please read [our paper](https://journals.flvc.org/FLAIRS/article/view/130725/133879) to get more information on this.
* Character Level
    * Train: [EverestNER-train-char.txt](EverestNER-train-char.txt)
    * Test:  [EverestNER-test-char.txt](EverestNER-train-char.txt)

* Token Level 
    * Train: [EverestNER-train-bio.txt](EverestNER-train-bio.txt)
    * Test: [EverestNER-test-bio.txt](EverestNER-train-bio.txt)

## Our Results
Model comparision on EverestNER-test. Models (a) baseline (rule-based), (b) BLSTM CRF, and (c) multilingual BERT: 
|Model |Pre. |Rec. |F1-micro|
| --- | --- | --- | --- |
|Baseline (Rule-based)|0.71 |0.55| 0.62|
|BLSTM-CRF-wc.ft|**0.89**| 0.74| 0.81|
|BERT-bbmu|0.87 |**0.84** |**0.85**|

Performance evaluation of the best performing model (BERT-bbmu) per named entities: 
|Model|Pre. |Rec. |F1| Support|
| --- | --- | --- | --- |--- |
|PER|0.90|0.85|0.88|1115|
|LOC|0.85|0.80|0.82|809|
|ORG|0.85|0.83|0.84|715|
|EVT|0.46|0.42|0.44|59|
|DAT|0.91|0.91|0.91|572|


# License 
Non-commercial purposes only. For commercial usages, permissions must be taken from the authors and the relevant parties. See the contact address below. 

Unless required by applicable law or agreed to in writing, software and data distributed here is on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.

# Cite Our Work
If you use the EverestNER data set, please cite [our publication](https://journals.flvc.org/FLAIRS/article/view/130725/133879): 
```bibtex
@inproceedings{niraula2022named,
  title={Named Entity Recognition for Nepali: Data Sets and Algorithms},
  author={Niraula, Nobal and Chapagain, Jeevan},
  booktitle={The International FLAIRS Conference Proceedings},
  volume={35},
  year={2022}
}
```
# Contact 
Feel free to contact nobal @AT nowalab .DOT com for any inquiries regarding this work.

# Acknowledgments
Nepali Shabdakosh - https://nepalishabdakosh.com 


