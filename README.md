# EverestNER - The Benchmark Data Set for Nepali NER
We have created the largest human annotated Named Entity Recognition (NER) data set for Nepali available to date. Highlights: 

* EverestNER covers five named entities - Person Name, Location, Organization, Event and Date. 
* EverestNER has 24,587 entities, 308,353 tokens corresponding to 15,798 sentences 
* We split the EverestNER data set into EverestNER-train and EverestNER-test. These standard data sets, therefore, become the first benchmark data sets for evaluating Nepali NER systems. 
* We report a comprehensive evaluation of state-of-the-art Neural and Transformer models using these data sets. We also discuss the remaining challenges for discovering NEs for Nepali (see our paper below).

|Data |Articles |Sentences |Tokens |Avg. Sent.Len| LOC| ORG| PER| EVT| DAT|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Train | 847| 13,848| 268,741| 19.40| 5,148| 4,756| 7,707| 312| 3,394|
|Test| 149| 1,950| 39,612| 20.31| 809| 715| 1,115| 59| 572| 
|Total| 996| 15,798| 308,353| 19.51| 5,957| 5,471| 8,822| 371| 3,966| 


# Data Format
The EverestNER data set is divided into train (EverestNER-train) and test (EverestNER-test) sets. Each data set has character level annotations (EverestNER-train-char.txt & EverestNER-test-char.txt) as well as token level annotations (EverestNER-train-bio.txt & EverestNER-test-bio.txt). Please read [our paper](https://journals.flvc.org/FLAIRS/article/view/130725/133879) to get more information on this. 

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


