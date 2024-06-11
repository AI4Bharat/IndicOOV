# IndicOOV

## Abstract
Publicly available TTS datasets for low-resource languages like
Hindi and Tamil typically contain 10-20 hours of data, lead-
ing to poor vocabulary coverage. This limitation becomes evi-
dent in downstream applications where domain-specific vocab-
ulary coupled with frequent code-mixing with English, results
in many OOV words. To highlight this problem, we create a
benchmark containing OOV words from several real-world ap-
plications. Indeed, state-of-the-art Hindi and Tamil TTS sys-
tems perform poorly on this OOV benchmark, as indicated by
intelligibility tests. To improve the model’s OOV performance,
we propose a low-effort and economically viable strategy to ob-
tain more training data. Specifically, we propose using volun-
teers as opposed to high quality voice artists to record words
containing character bigrams unseen in the training data. We
show that using such inexpensive data, the model’s performance
improves on OOV words, while not affecting voice quality and
in-domain performance.
