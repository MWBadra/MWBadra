# Mohamed Badra

Computer Engineering at Ain Shams & the University of East London, out in 2027.
I like problems where the useful information is sitting in text nobody has bothered to structure yet.

[Writing](https://mwbadra.github.io/) · [LinkedIn](https://linkedin.com/in/mwbadra) · [Email](mailto:MohamedWBadra@gmail.com)

---

## 🔍 What I'm working on

### [Quote-grounded lineup prediction](https://github.com/MWBadra/quote-grounded-lineup-prediction)
*Can a language model read the football press well enough to guess the team sheet?*

Sort of. But the interesting question turned out to be a different one: **the model was trained after
the season ended — so is it reading my articles, or reciting a team sheet it already memorised?**

Everyone in this position cites a knowledge cutoff. I didn't want to take that on faith, so I made every
extracted claim cite a verbatim span, verified it against the retrieved text in code, and then ran the
model with no sources at all to see what it knew unaided.

| Given nothing but a club, a date and a roster | ROC-AUC **0.654** on 68.4% of players |
|:--|--:|
| Same cases, unaided recall vs. quote-grounded | **0.513** vs. **0.713** |
| How often the two agree | **34.1%** |

That first number is the one I'd have most liked not to find. It's also why the rest of the result is
worth anything. Solo-authored paper, full dataset and every extracted quote released.

📖 [The long version](https://mwbadra.github.io/posts/lineup-prediction-contamination.html) — ~20 minutes,
and it explains every metric it uses.

---

## 🛠 Things I've built

**[Distributed LLM serving](https://github.com/3omar146/Distributed-LLM-Serving-System)** · NGINX → FastAPI
masters → workers → remote A100s. 1,000 concurrent requests, 100% success under burst load, zero
client-visible failures even when we killed GPU instances mid-run on purpose.

**[Six classifiers, no libraries](https://github.com/eslamfawzy72/Image-classification-ML-Project)** · KNN,
naive Bayes, multinomial regression, decision trees, linear SVM and random forest — written in NumPy from
scratch, because you don't really understand a model until you've debugged its gradients at 2am. PCA and
HOG pipelines on top. 97.5% macro-F1.

**[Agents that don't hardcode the flow](https://github.com/MWBadra/Cellula)** · ReAct agents orchestrating
tools dynamically, a LangGraph state-machine dev assistant, and a multimodal toxicity classifier. Built
during an NLP internship at Cellula.

---

## 🧰 Reach for most often

`Python` `pandas` `XGBoost` `scikit-learn` `SciPy` `LangChain` `LangGraph` `FastAPI` `Docker` `FAISS`
`SQL` `Java` `Spring Boot` `C++` `React`

<sub>Previously: R&D intern at EL-Sewedy Electric, building smart-meter tooling over serial connections —
which is a very different kind of debugging.</sub>
