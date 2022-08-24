# Secure code synthesis

## Abstract

Writing Smart Contracts (SCs) are hard. Writing secure SCs is even harder. Automatic code generation is by many considered the ”holy grail” in the field of computer science. Recent advances in transformer models have shown great potential in the area of synthesizing code from code comments. However, it is just as important how these models are best put to use. In this thesis, it is investigated: how to automatically generate Smart Contract code with transformer-based language models, by inputting comments to guide the code generation? Due to the monetary and immutable nature of blockchain, security in SCs is of uttermost importance. This thesis also investigates: how to generate secure Smart Contract code with transformer-based language models? A design science research approach is adopted for answering these research questions. For automatically synthesizing SC code, the 6 billion parameter model GPT-J by EleutherAI is fine-tuned on SC code. For this task, the currently largest dataset of real SC code is constructed, containing 186,397 contracts. To evaluate the comment-aid approach to generate code, the original code was used as the ground truth. This code was then compared with the generated code, and their differences were measured using the BiLingual Evaluation Understudy (BLEU) score. Results of the evaluation show that this approach results in a BLEU score of 0.557, which is beyond the state-of-the-art. For generating secure Smart Contract code with transformer-based language models, a novel method named security conditioning is proposed. From both automatic and manual evaluation of the technique, the evaluation results show that security conditioning produced secure code.

### Building document locally

A `Makefile` is provided for building the document locally. This requires a LaTeX compiler, such as [`texlive`](https://www.tug.org/texlive/), installed locally, which has to provide the commands `pdflatex` and `biber`.


### FAQ
If sources produces an error, try running 
```
rm -rf `biber --cache`
```
