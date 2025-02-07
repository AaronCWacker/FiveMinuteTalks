# FiveMinuteTalks
Auto Presentation Teleprompter AI For Teaching in Five Minutes

I am working on a ai app.py which I am using to create audio summaries of research papers and discuss what their impact on learning AI can be for training AI and people at once using audio, text, and speech modalities.  The workflow is voice in (spoken) to present a request, then a frontier model answers the question or request initially and inherits some degree of safety and training of the response from this initial request.  With it it then uses both inputs to search an AI embeddings using semantic search RAG ai which answers with selection of the top twenty research papers of the topic at hand.  This is shown in markdown and also marquee displays like singular teleprompters for each paper.  Then the paper link to abstract, the pdf, and the paper title and authors, and the paper summary are read aloud into wav files using a voice the user selected using the edge TTS voices (7).  Lets create a mermaid model for this.  My ideal would be how to create a live 5 minute talk which is perfectly timed as 15 seconds of read aloud per paper.  Help me with the graph as mermaid model first then I would like to share my code with you and you help me create a csv output for the dataset of assets, we save the assets and then on the interface we prepare the user for recording the five minute video where they read aloud request, each paper summary (abbreviated to match words per minute voice rate) and then crosses the timing finish line at exactly 5 minutes.    

Below is a sample of output for our first test together:   


```mermaid

flowchart TD
    A[User Voice Input: Spoken Request]
    B[Frontier Model: Generate Initial Safe Answer]
    C[Combine Inputs: Voice Request + Frontier Answer]
    D[Semantic Search: Query AI Embeddings via RAG]
    E[Retrieve Top 20 Research Papers]
    F[Extract Paper Details: Title, Authors, Abstract, PDF Link, Summary]
    G[Display Results: Markdown & Marquee Teleprompters]
    H[Audio Generation: Create WAV files via selected Edge TTS voice]
    I[Timing Control: Enforce 15 sec per paper for Total 5 min]
    J[Asset Logging: Generate CSV Dataset with metadata + audio asset links]
    K[Pre-Recording Interface: Prepare 5-Minute Video Session]
    L[Video Recording: User Reads Request & Abbreviated Summaries]
    M[Final Output: Precisely Timed 5-Minute Live Talk]
    
    A --> B
    B --> C
    C --> D
    D --> E
    E --> F
    F --> G
    G --> H
    H --> I
    I --> J
    J --> K
    K --> L
    L --> M
```

```markdown
📄 How to Train Your Agent to Read and Write
### 04 Jan 2021 | How to Train Your Agent to Read and Write — Arxiv Link)

Authors: Li Liu, Mengge He, Guanghui Xu, Mingkui Tan, Qi Wu

Reading and writing research papers is one of the most privileged abilities that a qualified researcher should master. However, it is difficult for new researchers (\eg{students}) to fully {grasp} this ability. It would be fascinating if we could train an intelligent agent to help people read and summarize papers, and perhaps even discover and exploit the potential knowledge clues to write novel papers. Although there have been existing works focusing on summarizing (\emph{i.e.}, reading) the knowledge in a given text or generating (\emph{i.e.}, writing) a text based on the given knowledge, the ability of simultaneously reading and writing is still under development. Typically, this requires an agent to fully understand the knowledge from the given text materials and generate correct and fluent novel paragraphs, which is very challenging in practice. In this paper, we propose a Deep ReAder-Writer (DRAW) network, which consists of a \textit{Reader} that can extract knowledge graphs (KGs) from input paragraphs and discover potential knowledge, a graph-to-text \textit{Writer} that generates a novel paragraph, and a \textit{Reviewer} that reviews the generated paragraph from three different aspects. Extensive experiments show that our DRAW network outperforms considered baselines and several state-of-the-art methods on AGENDA and M-AGENDA datasets. Our code and supplementary are released at https://github.com/menggehe/DRAW. ---------------


📄 TSTR: Too Short to Represent, Summarize with Details! Intro-Guided Extended Summary Generation
### 02 Jun 2022 | TSTR: Too Short to Represent, Summarize with Details! Intro-Guided Extended Summary Generation — Arxiv Link)

Authors: Sajad Sotudeh, Nazli Goharian

Many scientific papers such as those in arXiv and PubMed data collections have abstracts with varying lengths of 50-1000 words and average length of approximately 200 words, where longer abstracts typically convey more information about the source paper. Up to recently, scientific summarization research has typically focused on generating short, abstract-like summaries following the existing datasets used for scientific summarization. In domains where the source text is relatively long-form, such as in scientific documents, such summary is not able to go beyond the general and coarse overview and provide salient information from the source document. The recent interest to tackle this problem motivated curation of scientific datasets, arXiv-Long and PubMed-Long, containing human-written summaries of 400-600 words, hence, providing a venue for research in generating long/extended summaries. Extended summaries facilitate a faster read while providing details beyond coarse information. In this paper, we propose TSTR, an extractive summarizer that utilizes the introductory information of documents as pointers to their salient information. The evaluations on two existing large-scale extended summarization datasets indicate statistically significant improvement in terms of Rouge and average Rouge (F1) scores (except in one case) as compared to strong baselines and state-of-the-art. Comprehensive human evaluations favor our generated extended summaries in terms of cohesion and completeness. ---------------


📄 NarrativeXL: A Large-scale Dataset For Long-Term Memory Models
### 08 Dec 2023 | NarrativeXL: A Large-scale Dataset For Long-Term Memory Models — Arxiv Link)

Authors: Arseny Moskvichev and Ky-Vinh Mai

We propose a new large-scale (nearly a million questions) ultra-long-context (more than 50,000 words average document length) reading comprehension dataset. Using GPT 3.5, we summarized each scene in 1,500 hand-curated fiction books from Project Gutenberg, which resulted in approximately 150 scene-level summaries per book. After that, we created a number of reading comprehension questions based on these summaries, including three types of multiple-choice scene recognition questions, as well as free-form narrative reconstruction questions. With 990,595 total questions, our dataset is an order of magnitude larger than the closest alternatives. Crucially, most questions have a known ``retention demand'', indicating how long-term of a memory is needed to answer them, which should aid long-term memory performance evaluation. We validate our data in four small-scale experiments: one with human labelers, and three with existing language models. We show that our questions 1) adequately represent the source material 2) can be used to diagnose a model's memory capacity 3) are not trivial for modern language models even when the memory demand does not exceed those models' context lengths. Lastly, we provide our code which can be used to further expand the dataset with minimal human labor. ---------------


📄 GigaSpeech: An Evolving, Multi-domain ASR Corpus with 10,000 Hours of Transcribed Audio
### 13 Jun 2021 | GigaSpeech: An Evolving, Multi-domain ASR Corpus with 10,000 Hours of Transcribed Audio — Arxiv Link)

Authors: Guoguo Chen, Shuzhou Chai, Guanbo Wang, Jiayu Du, Wei-Qiang Zhang, Chao Weng, Dan Su, Daniel Povey, Jan Trmal, Junbo Zhang, Mingjie Jin, Sanjeev Khudanpur, Shinji Watanabe, Shuaijiang Zhao, Wei Zou, Xiangang Li, Xuchen Yao, Yongqing Wang, Yujun Wang, Zhao You, Zhiyong Yan

This paper introduces GigaSpeech, an evolving, multi-domain English speech recognition corpus with 10,000 hours of high quality labeled audio suitable for supervised training, and 40,000 hours of total audio suitable for semi-supervised and unsupervised training. Around 40,000 hours of transcribed audio is first collected from audiobooks, podcasts and YouTube, covering both read and spontaneous speaking styles, and a variety of topics, such as arts, science, sports, etc. A new forced alignment and segmentation pipeline is proposed to create sentence segments suitable for speech recognition training, and to filter out segments with low-quality transcription. For system training, GigaSpeech provides five subsets of different sizes, 10h, 250h, 1000h, 2500h, and 10000h. For our 10,000-hour XL training subset, we cap the word error rate at 4% during the filtering/validation stage, and for all our other smaller training subsets, we cap it at 0%. The DEV and TEST evaluation sets, on the other hand, are re-processed by professional human transcribers to ensure high transcription quality. Baseline systems are provided for popular speech recognition toolkits, namely Athena, ESPnet, Kaldi and Pika. ---------------


📄 Leveraging supplementary text data to kick-start automatic speech recognition system development with limited transcriptions
### 09 Feb 2023 | Leveraging supplementary text data to kick-start automatic speech recognition system development with limited transcriptions — Arxiv Link)

Authors: Nay San, Martijn Bartelds, Blaine Billings, Ella de Falco, Hendi Feriza, Johan Safri, Wawan Sahrozi, Ben Foley, Bradley McDonnell, Dan Jurafsky

Recent research using pre-trained transformer models suggests that just 10 minutes of transcribed speech may be enough to fine-tune such a model for automatic speech recognition (ASR) — at least if we can also leverage vast amounts of text data (803 million tokens). But is that much text data necessary? We study the use of different amounts of text data, both for creating a lexicon that constrains ASR decoding to possible words (e.g. *dogz vs. dogs), and for training larger language models that bias the system toward probable word sequences (e.g. too dogs vs. two dogs). We perform experiments using 10 minutes of transcribed speech from English (for replicating prior work) and two additional pairs of languages differing in the availability of supplemental text data: Gronings and Frisian (~7.5M token corpora available), and Besemah and Nasal (only small lexica available). For all languages, we found that using only a lexicon did not appreciably improve ASR performance. For Gronings and Frisian, we found that lexica and language models derived from 'novel-length' 80k token subcorpora reduced the word error rate (WER) to 39% on average. Our findings suggest that where a text corpus in the upper tens of thousands of tokens or more is available, fine-tuning a transformer model with just tens of minutes of transcribed speech holds some promise towards obtaining human-correctable transcriptions near the 30% WER rule-of-thumb. ---------------


📄 QuALITY: Question Answering with Long Input Texts, Yes!
### 11 May 2022 | QuALITY: Question Answering with Long Input Texts, Yes! — Arxiv Link)

Authors: Richard Yuanzhe Pang, Alicia Parrish, Nitish Joshi, Nikita Nangia, Jason Phang, Angelica Chen, Vishakh Padmakumar, Johnny Ma, Jana Thompson, He He, Samuel R. Bowman

To enable building and testing models on long-document comprehension, we introduce QuALITY, a multiple-choice QA dataset with context passages in English that have an average length of about 5,000 tokens, much longer than typical current models can process. Unlike in prior work with passages, our questions are written and validated by contributors who have read the entire passage, rather than relying on summaries or excerpts. In addition, only half of the questions are answerable by annotators working under tight time constraints, indicating that skimming and simple search are not enough to consistently perform well. Our baseline models perform poorly on this task (55.4%) and significantly lag behind human performance (93.5%). ---------------


📄 Augmenting Scientific Papers with Just-in-Time, Position-Sensitive Definitions of Terms and Symbols
### 27 Apr 2021 | Augmenting Scientific Papers with Just-in-Time, Position-Sensitive Definitions of Terms and Symbols — Arxiv Link)

Authors: Andrew Head (UC Berkeley), Kyle Lo (Allen Institute for AI), Dongyeop Kang (UC Berkeley), Raymond Fok (University of Washington), Sam Skjonsberg (Allen Institute for AI), Daniel S. Weld (Allen Institute for AI, University of Washington), Marti A. Hearst (UC Berkeley)

Despite the central importance of research papers to scientific progress, they can be difficult to read. Comprehension is often stymied when the information needed to understand a passage resides somewhere else: in another section, or in another paper. In this work, we envision how interfaces can bring definitions of technical terms and symbols to readers when and where they need them most. We introduce ScholarPhi, an augmented reading interface with four novel features: (1) tooltips that surface position-sensitive definitions from elsewhere in a paper, (2) a filter over the paper that "declutters" it to reveal how the term or symbol is used across the paper, (3) automatic equation diagrams that expose multiple definitions in parallel, and (4) an automatically generated glossary of important terms and symbols. A usability study showed that the tool helps researchers of all experience levels read papers. Furthermore, researchers were eager to have ScholarPhi's definitions available to support their everyday reading. ---------------


📄 Community-Driven Comprehensive Scientific Paper Summarization: Insight from cvpaper.challenge
### 17 Mar 2022 | Community-Driven Comprehensive Scientific Paper Summarization: Insight from cvpaper.challenge — Arxiv Link)

Authors: Shintaro Yamamoto, Hirokatsu Kataoka, Ryota Suzuki, Seitaro Shinagawa, Shigeo Morishima

The present paper introduces a group activity involving writing summaries of conference proceedings by volunteer participants. The rapid increase in scientific papers is a heavy burden for researchers, especially non-native speakers, who need to survey scientific literature. To alleviate this problem, we organized a group of non-native English speakers to write summaries of papers presented at a computer vision conference to share the knowledge of the papers read by the group. We summarized a total of 2,000 papers presented at the Conference on Computer Vision and Pattern Recognition, a top-tier conference on computer vision, in 2019 and 2020. We quantitatively analyzed participants' selection regarding which papers they read among the many available papers. The experimental results suggest that we can summarize a wide range of papers without asking participants to read papers unrelated to their interests. ---------------


📄 A Multiple Choices Reading Comprehension Corpus for Vietnamese Language Education
### 31 Mar 2023 | A Multiple Choices Reading Comprehension Corpus for Vietnamese Language Education — Arxiv Link)

Authors: Son T. Luu, Khoi Trong Hoang, Tuong Quang Pham, Kiet Van Nguyen, Ngan Luu-Thuy Nguyen

Machine reading comprehension has been an interesting and challenging task in recent years, with the purpose of extracting useful information from texts. To attain the computer ability to understand the reading text and answer relevant information, we introduce ViMMRC 2.0 - an extension of the previous ViMMRC for the task of multiple-choice reading comprehension in Vietnamese Textbooks which contain the reading articles for students from Grade 1 to Grade 12. This dataset has 699 reading passages which are prose and poems, and 5,273 questions. The questions in the new dataset are not fixed with four options as in the previous version. Moreover, the difficulty of questions is increased, which challenges the models to find the correct choice. The computer must understand the whole context of the reading passage, the question, and the content of each choice to extract the right answers. Hence, we propose the multi-stage approach that combines the multi-step attention network (MAN) with the natural language inference (NLI) task to enhance the performance of the reading comprehension model. Then, we compare the proposed methodology with the baseline BERTology models on the new dataset and the ViMMRC 1.0. Our multi-stage models achieved 58.81% by Accuracy on the test set, which is 5.34% better than the highest BERTology models. From the results of the error analysis, we found the challenge of the reading comprehension models is understanding the implicit context in texts and linking them together in order to find the correct answers. Finally, we hope our new dataset will motivate further research in enhancing the language understanding ability of computers in the Vietnamese language. ---------------


📄 PubSqueezer: A Text-Mining Web Tool to Transform Unstructured Documents into Structured Data
### 09 Nov 2020 | PubSqueezer: A Text-Mining Web Tool to Transform Unstructured Documents into Structured Data — Arxiv Link)

Authors: Alberto Calderone

The amount of scientific papers published every day is daunting and constantly increasing. Keeping up with literature represents a challenge. If one wants to start exploring new topics it is hard to have a big picture without reading lots of articles. Furthermore, as one reads through literature, making mental connections is crucial to ask new questions which might lead to discoveries. In this work, I present a web tool which uses a Text Mining strategy to transform large collections of unstructured biomedical articles into structured data. Generated results give a quick overview on complex topics which can possibly suggest not explicitly reported information. In particular, I show two Data Science analyses. First, I present a literature based rare diseases network build using this tool in the hope that it will help clarify some aspects of these less popular pathologies. Secondly, I show how a literature based analysis conducted with PubSqueezer results allows to describe known facts about SARS-CoV-2. In one sentence, data generated with PubSqueezer make it easy to use scientific literate in any computational analysis such as machine learning, natural language processing etc. Availability: http://www.pubsqueezer.com ---------------


📄 True Detective: A Deep Abductive Reasoning Benchmark Undoable for GPT-3 and Challenging for GPT-4
### 01 Jun 2023 | True Detective: A Deep Abductive Reasoning Benchmark Undoable for GPT-3 and Challenging for GPT-4 — Arxiv Link)

Authors: Maksym Del and Mark Fishel

Large language models (LLMs) have demonstrated solid zero-shot reasoning capabilities, which is reflected in their performance on the current test tasks. This calls for a more challenging benchmark requiring highly advanced reasoning ability to be solved. In this paper, we introduce such a benchmark, consisting of 191 long-form (1200 words on average) mystery narratives constructed as detective puzzles. Puzzles are sourced from the "5 Minute Mystery" platform and include a multiple-choice question for evaluation. Only 47% of humans solve a puzzle successfully on average, while the best human solvers achieve over 80% success rate. We show that GPT-3 models barely outperform random on this benchmark (with 28% accuracy) while state-of-the-art GPT-4 solves only 38% of puzzles. This indicates that there is still a significant gap in the deep reasoning abilities of LLMs and humans and highlights the need for further research in this area. Our work introduces a challenging benchmark for future studies on reasoning in language models and contributes to a better understanding of the limits of LLMs' abilities. ---------------


📄 A Dataset of Information-Seeking Questions and Answers Anchored in Research Papers
### 07 May 2021 | A Dataset of Information-Seeking Questions and Answers Anchored in Research Papers — Arxiv Link)

Authors: Pradeep Dasigi, Kyle Lo, Iz Beltagy, Arman Cohan, Noah A. Smith, Matt Gardner

Readers of academic research papers often read with the goal of answering specific questions. Question Answering systems that can answer those questions can make consumption of the content much more efficient. However, building such tools requires data that reflect the difficulty of the task arising from complex reasoning about claims made in multiple parts of a paper. In contrast, existing information-seeking question answering datasets usually contain questions about generic factoid-type information. We therefore present QASPER, a dataset of 5,049 questions over 1,585 Natural Language Processing papers. Each question is written by an NLP practitioner who read only the title and abstract of the corresponding paper, and the question seeks information present in the full text. The questions are then answered by a separate set of NLP practitioners who also provide supporting evidence to answers. We find that existing models that do well on other QA tasks do not perform well on answering these questions, underperforming humans by at least 27 F1 points when answering them from entire papers, motivating further research in document-grounded, information-seeking QA, which our dataset is designed to facilitate. ---------------


📄 GPT Takes the Bar Exam
### 29 Dec 2022 | GPT Takes the Bar Exam — Arxiv Link)

Authors: Michael Bommarito II, Daniel Martin Katz

Nearly all jurisdictions in the United States require a professional license exam, commonly referred to as "the Bar Exam," as a precondition for law practice. To even sit for the exam, most jurisdictions require that an applicant completes at least seven years of post-secondary education, including three years at an accredited law school. In addition, most test-takers also undergo weeks to months of further, exam-specific preparation. Despite this significant investment of time and capital, approximately one in five test-takers still score under the rate required to pass the exam on their first try. In the face of a complex task that requires such depth of knowledge, what, then, should we expect of the state of the art in "AI?" In this research, we document our experimental evaluation of the performance of OpenAI's text-davinci-003 model, often-referred to as GPT-3.5, on the multistate multiple choice (MBE) section of the exam. While we find no benefit in fine-tuning over GPT-3.5's zero-shot performance at the scale of our training data, we do find that hyperparameter optimization and prompt engineering positively impacted GPT-3.5's zero-shot performance. For best prompt and parameters, GPT-3.5 achieves a headline correct rate of 50.3% on a complete NCBE MBE practice exam, significantly in excess of the 25% baseline guessing rate, and performs at a passing rate for both Evidence and Torts. GPT-3.5's ranking of responses is also highly-correlated with correctness; its top two and top three choices are correct 71% and 88% of the time, respectively, indicating very strong non-entailment performance. While our ability to interpret these results is limited by nascent scientific understanding of LLMs and the proprietary nature of GPT, we believe that these results strongly suggest that an LLM will pass the MBE component of the Bar Exam in the near future. ---------------


📄 Explaining Relationships Among Research Papers
### 20 Feb 2024 | Explaining Relationships Among Research Papers — Arxiv Link)

Authors: Xiangci Li and Jessica Ouyang

Due to the rapid pace of research publications, keeping up to date with all the latest related papers is very time-consuming, even with daily feed tools. There is a need for automatically generated, short, customized literature reviews of sets of papers to help researchers decide what to read. While several works in the last decade have addressed the task of explaining a single research paper, usually in the context of another paper citing it, the relationship among multiple papers has been ignored; prior works have focused on generating a single citation sentence in isolation, without addressing the expository and transition sentences needed to connect multiple papers in a coherent story. In this work, we explore a feature-based, LLM-prompting approach to generate richer citation texts, as well as generating multiple citations at once to capture the complex relationships among research papers. We perform an expert evaluation to investigate the impact of our proposed features on the quality of the generated paragraphs and find a strong correlation between human preference and integrative writing style, suggesting that humans prefer high-level, abstract citations, with transition sentences between them to provide an overall story. ---------------


📄 Who Said What? An Automated Approach to Analyzing Speech in Preschool Classrooms
### 05 Mar 2024 | Who Said What? An Automated Approach to Analyzing Speech in Preschool Classrooms — Arxiv Link)

Authors: Anchen Sun, Juan J Londono, Batya Elbaum, Luis Estrada, Roberto Jose Lazo, Laura Vitale, Hugo Gonzalez Villasanti, Riccardo Fusaroli, Lynn K Perry, Daniel S Messinger

Young children spend substantial portions of their waking hours in noisy preschool classrooms. In these environments, children's vocal interactions with teachers are critical contributors to their language outcomes, but manually transcribing these interactions is prohibitive. Using audio from child- and teacher-worn recorders, we propose an automated framework that uses open source software both to classify speakers (ALICE) and to transcribe their utterances (Whisper). We compare results from our framework to those from a human expert for 110 minutes of classroom recordings, including 85 minutes from child-word microphones (n=4 children) and 25 minutes from teacher-worn microphones (n=2 teachers). The overall proportion of agreement, that is, the proportion of correctly classified teacher and child utterances, was .76, with an error-corrected kappa of .50 and a weighted F1 of .76. The word error rate for both teacher and child transcriptions was .15, meaning that 15% of words would need to be deleted, added, or changed to equate the Whisper and expert transcriptions. Moreover, speech features such as the mean length of utterances in words, the proportion of teacher and child utterances that were questions, and the proportion of utterances that were responded to within 2.5 seconds were similar when calculated separately from expert and automated transcriptions. The results suggest substantial progress in analyzing classroom speech that may support children's language development. Future research using natural language processing is underway to improve speaker classification and to analyze results from the application of the automated it framework to a larger dataset containing classroom recordings from 13 children and 4 teachers observed on 17 occasions over one year. ---------------


📄 Modeling Task Effects on Meaning Representation in the Brain via Zero-Shot MEG Prediction
### 15 Nov 2020 | Modeling Task Effects on Meaning Representation in the Brain via Zero-Shot MEG Prediction — Arxiv Link)

Authors: Mariya Toneva, Otilia Stretcu, Barnabas Poczos, Leila Wehbe, Tom M. Mitchell

How meaning is represented in the brain is still one of the big open questions in neuroscience. Does a word (e.g., bird) always have the same representation, or does the task under which the word is processed alter its representation (answering "can you eat it?" versus "can it fly?")? The brain activity of subjects who read the same word while performing different semantic tasks has been shown to differ across tasks. However, it is still not understood how the task itself contributes to this difference. In the current work, we study Magnetoencephalography (MEG) brain recordings of participants tasked with answering questions about concrete nouns. We investigate the effect of the task (i.e. the question being asked) on the processing of the concrete noun by predicting the millisecond-resolution MEG recordings as a function of both the semantics of the noun and the task. Using this approach, we test several hypotheses about the task-stimulus interactions by comparing the zero-shot predictions made by these hypotheses for novel tasks and nouns not seen during training. We find that incorporating the task semantics significantly improves the prediction of MEG recordings, across participants. The improvement occurs 475-550ms after the participants first see the word, which corresponds to what is considered to be the ending time of semantic processing for a word. These results suggest that only the end of semantic processing of a word is task-dependent, and pose a challenge for future research to formulate new hypotheses for earlier task effects as a function of the task and stimuli. ---------------


📄 Quiz-Style Question Generation for News Stories
### 18 Feb 2021 | Quiz-Style Question Generation for News Stories — Arxiv Link)

Authors: Adam D. Lelkes, Vinh Q. Tran, Cong Yu

A large majority of American adults get at least some of their news from the Internet. Even though many online news products have the goal of informing their users about the news, they lack scalable and reliable tools for measuring how well they are achieving this goal, and therefore have to resort to noisy proxy metrics (e.g., click-through rates or reading time) to track their performance. As a first step towards measuring news informedness at a scale, we study the problem of quiz-style multiple-choice question generation, which may be used to survey users about their knowledge of recent news. In particular, we formulate the problem as two sequence-to-sequence tasks: question-answer generation (QAG) and distractor, or incorrect answer, generation (DG). We introduce NewsQuizQA, the first dataset intended for quiz-style question-answer generation, containing 20K human written question-answer pairs from 5K news article summaries. Using this dataset, we propose a series of novel techniques for applying large pre-trained Transformer encoder-decoder models, namely PEGASUS and T5, to the tasks of question-answer generation and distractor generation. We show that our models outperform strong baselines using both automated metrics and human raters. We provide a case study of running weekly quizzes on real-world users via the Google Surveys platform over the course of two months. We found that users generally found the automatically generated questions to be educational and enjoyable. Finally, to serve the research community, we are releasing the NewsQuizQA dataset. ---------------


📄 Interpretation of Natural Language Rules in Conversational Machine Reading
### 28 Aug 2018 | Interpretation of Natural Language Rules in Conversational Machine Reading — Arxiv Link)

Authors: Marzieh Saeidi, Max Bartolo, Patrick Lewis, Sameer Singh, Tim Rockt"aschel, Mike Sheldon, Guillaume Bouchard, Sebastian Riedel

Most work in machine reading focuses on question answering problems where the answer is directly expressed in the text to read. However, many real-world question answering problems require the reading of text not because it contains the literal answer, but because it contains a recipe to derive an answer together with the reader's background knowledge. One example is the task of interpreting regulations to answer "Can I...?" or "Do I have to...?" questions such as "I am working in Canada. Do I have to carry on paying UK National Insurance?" after reading a UK government website about this topic. This task requires both the interpretation of rules and the application of background knowledge. It is further complicated due to the fact that, in practice, most questions are underspecified, and a human assistant will regularly have to ask clarification questions such as "How long have you been working abroad?" when the answer cannot be directly derived from the question and text. In this paper, we formalise this task and develop a crowd-sourcing strategy to collect 32k task instances based on real-world rules and crowd-generated questions and scenarios. We analyse the challenges of this task and assess its difficulty by evaluating the performance of rule-based and machine-learning baselines. We observe promising results when no background knowledge is necessary, and substantial room for improvement whenever background knowledge is needed. ---------------


📄 The Semantic Reader Project: Augmenting Scholarly Documents through AI-Powered Interactive Reading Interfaces
### 23 Apr 2023 | The Semantic Reader Project: Augmenting Scholarly Documents through AI-Powered Interactive Reading Interfaces — Arxiv Link)

Authors: Kyle Lo, Joseph Chee Chang, Andrew Head, Jonathan Bragg, Amy X. Zhang, Cassidy Trier, Chloe Anastasiades, Tal August, Russell Authur, Danielle Bragg, Erin Bransom, Isabel Cachola, Stefan Candra, Yoganand Chandrasekhar, Yen-Sung Chen, Evie Yu-Yen Cheng, Yvonne Chou, Doug Downey, Rob Evans, Raymond Fok, Fangzhou Hu, Regan Huff, Dongyeop Kang, Tae Soo Kim, Rodney Kinney, Aniket Kittur, Hyeonsu Kang, Egor Klevak, Bailey Kuehl, Michael Langan, Matt Latzke, Jaron Lochner, Kelsey MacMillan, Eric Marsh, Tyler Murray, Aakanksha Naik, Ngoc-Uyen Nguyen, Srishti Palani, Soya Park, Caroline Paulic, Napol Rachatasumrit, Smita Rao, Paul Sayre, Zejiang Shen, Pao Siangliulue, Luca Soldaini, Huy Tran, Madeleine van Zuylen, Lucy Lu Wang, Christopher Wilhelm, Caroline Wu, Jiangjiang Yang, Angele Zamarron, Marti A. Hearst, Daniel S. Weld

Scholarly publications are key to the transfer of knowledge from scholars to others. However, research papers are information-dense, and as the volume of the scientific literature grows, the need for new technology to support the reading process grows. In contrast to the process of finding papers, which has been transformed by Internet technology, the experience of reading research papers has changed little in decades. The PDF format for sharing research papers is widely used due to its portability, but it has significant downsides including: static content, poor accessibility for low-vision readers, and difficulty reading on mobile devices. This paper explores the question "Can recent advances in AI and HCI power intelligent, interactive, and accessible reading interfaces — even for legacy PDFs?" We describe the Semantic Reader Project, a collaborative effort across multiple institutions to explore automatic creation of dynamic reading interfaces for research papers. Through this project, we've developed ten research prototype interfaces and conducted usability studies with more than 300 participants and real-world users showing improved reading experiences for scholars. We've also released a production reading interface for research papers that will incorporate the best features as they mature. We structure this paper around challenges scholars and the public face when reading research papers — Discovery, Efficiency, Comprehension, Synthesis, and Accessibility — and present an overview of our progress and remaining open challenges. ---------------


📄 Continuous Examination by Automatic Quiz Assessment Using Spiral Codes and Image Processing
### 26 Jan 2022 | Continuous Examination by Automatic Quiz Assessment Using Spiral Codes and Image Processing — Arxiv Link)

Authors: Fernando Alonso-Fernandez, Josef Bigun

We describe a technical solution implemented at Halmstad University to automatise assessment and reporting of results of paper-based quiz exams. Paper quizzes are affordable and within reach of campus education in classrooms. Offering and taking them is accepted as they cause fewer issues with reliability and democratic access, e.g. a large number of students can take them without a trusted mobile device, internet, or battery. By contrast, correction of the quiz is a considerable obstacle. We suggest mitigating the issue by a novel image processing technique using harmonic spirals that aligns answer sheets in sub-pixel accuracy to read student identity and answers and to email results within minutes, all fully automatically. Using the described method, we carry out regular weekly examinations in two master courses at the mentioned centre without a significant workload increase. The employed solution also enables us to assign a unique identifier to each quiz (e.g. week 1, week 2. . . ) while allowing us to have an individualised quiz for each student. ---------------
```

Claude's reply 🧠:

```python
To create a Streamlit app that addresses your request for a 5-minute high-resolution read-aloud and summarizing 20 research papers on assistive devices for speaking, reading, vocalization, and research, I would need access to those 20 research papers. However, since you did not provide the actual papers, I'll create a sample Streamlit app that demonstrates how it could be done.

Here's the app.py file:

import streamlit as st
import pyttsx3

# Initialize the text-to-speech engine
engine = pyttsx3.init()

# Set the voice rate and volume
engine.setProperty('rate', 150)  # Adjust the rate as per your preference
engine.setProperty('volume', 1.0)  # Adjust the volume as per your preference

# Function to read text aloud
def read_aloud(text):
    engine.say(text)
    engine.runAndWait()

# Function to summarize research papers
def summarize_papers(papers):
    summaries = []
    for paper in papers:
        # Placeholder for actual summarization logic
        summary = f"Summary of {paper}: ..."
        summaries.append(summary)
    return summaries

# Sample research papers (replace with actual papers)
research_papers = [
    "Paper 1: Assistive Technology for Speech Impairments",
    "Paper 2: Reading Aids for Visually Impaired Individuals",
    "Paper 3: Voice Recognition in Research and Education",
    # Add more papers here
]

# Streamlit app
def main():
    st.title("Assistive Devices for Speaking, Reading, and Research")

    # Read-aloud section
    st.header("Read Aloud")
    text_to_read = st.text_area("Enter text to be read aloud:")
    if st.button("Read Aloud"):
        read_aloud(text_to_read)

    # Research paper summaries section
    st.header("Research Paper Summaries")
    summaries = summarize_papers(research_papers)
    for summary in summaries:
        st.write(summary)

if __name__ == "__main__":
    main()

And the requirements.txt file:

streamlit
pyttsx3

This Streamlit app has two main sections:

Read Aloud: Users can enter text in a text area, and upon clicking the "Read Aloud" button, the text will be read aloud using the pyttsx3 library for text-to-speech.

Research Paper Summaries: This section assumes that you have a list of research papers. The summarize_papers function is a placeholder for the actual summarization logic, which you would need to implement based on the specific techniques or algorithms you want to use for summarizing the papers. The summaries are then displayed in the app.

To run the app, follow these steps:

Install the required libraries by running pip install -r requirements.txt in your terminal or command prompt.
Save the app.py file in your working directory.
Run the app with streamlit run app.py.
Please note that this is a basic example, and you may need to modify the code to fit your specific requirements, such as incorporating actual research papers and implementing the summarization logic.

Total Elapsed: 26.76 s
```


# Next we share our code with instructions to build on the context we have - shot 2

Here is my code.  The output creates a filename and each part of the research papers has an opportunity  to show a word count of the response with title, authors and summary.  If we just read aloud at normal human speed the paper title and a summary of the summry, say just the right number of words so we can estimate the duration of read aloud for the title and summary together that might work really great.  Then at end of the titles plus summary give a total length estimation.  It actually will be physically possible to save the duration.  Lets modify the file naming outputs to contain something like a small sequence that indicates word count for that paper summary and title (wct200) for word count 200, summary (sw500) is summary had 500 words, (dur15) for duration of words spoken if you read aloud title and high info keyword list (compose new 15 word summary of high info words) from text which best satisfies high rouge score to a summary on the summary which we will use to optimize the read aloud duration.    Here is the app.py.  Good lucck and make me proud.  Score yourself at the end.  Ideally I want just the full code listing back with no explanation.  Also for any comments you would have had, inject those as comments around the new code and ffunctions you create and modify allowing me to easily see what you added.  Thanks and be careful to not break my code and also to show full code listing so I don't have to patch your code in myself.     

```python
import streamlit as st
import anthropic
import openai
import base64
import cv2
import glob
import json
import math
import os
import pytz
import random
import re
import requests
#import textract
import time
import zipfile
import plotly.graph_objects as go
import streamlit.components.v1 as components
from datetime import datetime
from audio_recorder_streamlit import audio_recorder
from bs4 import BeautifulSoup
from collections import defaultdict, deque, Counter
from dotenv import load_dotenv
from gradio_client import Client
from huggingface_hub import InferenceClient
from io import BytesIO
from PIL import Image
from PyPDF2 import PdfReader
from urllib.parse import quote
from xml.etree import ElementTree as ET
from openai import OpenAI
import extra_streamlit_components as stx
from streamlit.runtime.scriptrunner import get_script_run_ctx
import asyncio
import edge_tts
from streamlit_marquee import streamlit_marquee
from typing import Tuple, Optional
import pandas as pd

# ─────────────────────────────────────────────────────────
# 1. CORE CONFIGURATION & SETUP
# ─────────────────────────────────────────────────────────

st.set_page_config(
    page_title="🚲TalkingAIResearcher🏆",
    page_icon="🚲🏆",
    layout="wide",
    initial_sidebar_state="auto",
    menu_items={
        'Get Help': 'https://huggingface.co/awacke1',
        'Report a bug': 'https://huggingface.co/spaces/awacke1',
        'About': "🚲TalkingAIResearcher🏆"
    }
)
load_dotenv()

# ▶ Available English voices for Edge TTS
EDGE_TTS_VOICES = [
    "en-US-AriaNeural",
    "en-US-GuyNeural",
    "en-US-JennyNeural",
    "en-GB-SoniaNeural",
    "en-GB-RyanNeural",
    "en-AU-NatashaNeural",
    "en-AU-WilliamNeural",
    "en-CA-ClaraNeural",
    "en-CA-LiamNeural"
]

# ▶ Initialize Session State
if 'marquee_settings' not in st.session_state:
    st.session_state['marquee_settings'] = {
        "background": "#1E1E1E",
        "color": "#FFFFFF",
        "font-size": "14px",
        "animationDuration": "20s",
        "width": "100%",
        "lineHeight": "35px"
    }
if 'tts_voice' not in st.session_state:
    st.session_state['tts_voice'] = EDGE_TTS_VOICES[0]
if 'audio_format' not in st.session_state:
    st.session_state['audio_format'] = 'mp3'
if 'transcript_history' not in st.session_state:
    st.session_state['transcript_history'] = []
if 'chat_history' not in st.session_state:
    st.session_state['chat_history'] = []
if 'openai_model' not in st.session_state:
    st.session_state['openai_model'] = "gpt-4o-2024-05-13"
if 'messages' not in st.session_state:
    st.session_state['messages'] = []
if 'last_voice_input' not in st.session_state:
    st.session_state['last_voice_input'] = ""
if 'editing_file' not in st.session_state:
    st.session_state['editing_file'] = None
if 'edit_new_name' not in st.session_state:
    st.session_state['edit_new_name'] = ""
if 'edit_new_content' not in st.session_state:
    st.session_state['edit_new_content'] = ""
if 'viewing_prefix' not in st.session_state:
    st.session_state['viewing_prefix'] = None
if 'should_rerun' not in st.session_state:
    st.session_state['should_rerun'] = False
if 'old_val' not in st.session_state:
    st.session_state['old_val'] = None
if 'last_query' not in st.session_state:
    st.session_state['last_query'] = ""
if 'marquee_content' not in st.session_state:
    st.session_state['marquee_content'] = "🚀 Welcome to TalkingAIResearcher | 🤖 Your Research Assistant"

# ▶ Additional keys for performance, caching, etc.
if 'audio_cache' not in st.session_state:
    st.session_state['audio_cache'] = {}
if 'download_link_cache' not in st.session_state:
    st.session_state['download_link_cache'] = {}
if 'operation_timings' not in st.session_state:
    st.session_state['operation_timings'] = {}
if 'performance_metrics' not in st.session_state:
    st.session_state['performance_metrics'] = defaultdict(list)
if 'enable_audio' not in st.session_state:
    st.session_state['enable_audio'] = True  # Turn TTS on/off

# ▶ API Keys
openai_api_key = os.getenv('OPENAI_API_KEY', "")
anthropic_key = os.getenv('ANTHROPIC_API_KEY_3', "")
xai_key = os.getenv('xai',"")
if 'OPENAI_API_KEY' in st.secrets:
    openai_api_key = st.secrets['OPENAI_API_KEY']
if 'ANTHROPIC_API_KEY' in st.secrets:
    anthropic_key = st.secrets["ANTHROPIC_API_KEY"]

openai.api_key = openai_api_key
openai_client = OpenAI(api_key=openai.api_key, organization=os.getenv('OPENAI_ORG_ID'))
HF_KEY = os.getenv('HF_KEY')
API_URL = os.getenv('API_URL')

# ▶ Helper constants
FILE_EMOJIS = {
    "md": "📝",
    "mp3": "🎵",
    "wav": "🔊"
}

# ─────────────────────────────────────────────────────────
# 2. PERFORMANCE MONITORING & TIMING
# ─────────────────────────────────────────────────────────

class PerformanceTimer:
    """
    ⏱️ A context manager for timing operations with automatic logging.
    Usage:
        with PerformanceTimer("my_operation"):
            # do something
    The duration is stored into `st.session_state['operation_timings']`
    and appended to the `performance_metrics` list.
    """
    def __init__(self, operation_name: str):
        self.operation_name = operation_name
        self.start_time = None
        
    def __enter__(self):
        self.start_time = time.time()
        return self
        
    def __exit__(self, exc_type, exc_val, exc_tb):
        if not exc_type:  # Only log if no exception occurred
            duration = time.time() - self.start_time
            st.session_state['operation_timings'][self.operation_name] = duration
            st.session_state['performance_metrics'][self.operation_name].append(duration)

def log_performance_metrics():
    """
    📈 Display performance metrics in the sidebar, including a timing breakdown
    and a small bar chart of average times.
    """
    st.sidebar.markdown("### ⏱️ Performance Metrics")
    
    metrics = st.session_state['operation_timings']
    if metrics:
        total_time = sum(metrics.values())
        st.sidebar.write(f"**Total Processing Time:** {total_time:.2f}s")
        
        # Break down each operation time
        for operation, duration in metrics.items():
            percentage = (duration / total_time) * 100
            st.sidebar.write(f"**{operation}:** {duration:.2f}s ({percentage:.1f}%)")
            
        # Show timing history chart
        history_data = []
        for op, times in st.session_state['performance_metrics'].items():
            if times:  # Only if we have data
                avg_time = sum(times) / len(times)
                history_data.append({"Operation": op, "Avg Time (s)": avg_time})
        
        if history_data:
            st.sidebar.markdown("### 📊 Timing History (Avg)")
            chart_data = pd.DataFrame(history_data)
            st.sidebar.bar_chart(chart_data.set_index("Operation"))

# ─────────────────────────────────────────────────────────
# 3. HELPER FUNCTIONS (FILENAMES, LINKS, MARQUEE, ETC.)
# ─────────────────────────────────────────────────────────

def get_central_time():
    """🌎 Get current time in US Central timezone."""
    central = pytz.timezone('US/Central')
    return datetime.now(central)

def format_timestamp_prefix():
    """📅 Generate a timestamp prefix"""
    ct = get_central_time()
    #return ct.strftime("%m_%d_%y_%I_%M_%p")
    return ct.strftime("%Y%m%d_%H%M%S")

def initialize_marquee_settings():
    """🌈 Initialize marquee defaults if needed."""
    if 'marquee_settings' not in st.session_state:
        st.session_state['marquee_settings'] = {
            "background": "#1E1E1E",
            "color": "#FFFFFF",
            "font-size": "14px",
            "animationDuration": "20s",
            "width": "100%",
            "lineHeight": "35px"
        }

def get_marquee_settings():
    """🔧 Retrieve marquee settings from session."""
    initialize_marquee_settings()
    return st.session_state['marquee_settings']

def update_marquee_settings_ui():
    """🖌 Add color pickers & sliders for marquee config in the sidebar."""
    st.sidebar.markdown("### 🎯 Marquee Settings")
    cols = st.sidebar.columns(2)
    with cols[0]:
        bg_color = st.color_picker("🎨 Background", 
                                  st.session_state['marquee_settings']["background"], 
                                  key="bg_color_picker")
        text_color = st.color_picker("✍️ Text", 
                                    st.session_state['marquee_settings']["color"], 
                                    key="text_color_picker")
    with cols[1]:
        font_size = st.slider("📏 Size", 10, 24, 14, key="font_size_slider")
        duration = st.slider("⏱️ Speed (secs)", 1, 20, 20, key="duration_slider")

    st.session_state['marquee_settings'].update({
        "background": bg_color,
        "color": text_color,
        "font-size": f"{font_size}px",
        "animationDuration": f"{duration}s"
    })

def display_marquee(text, settings, key_suffix=""):
    """
    🎉 Show a marquee text with style from the marquee settings.
    Automatically truncates text to ~280 chars to avoid overflow.
    """
    truncated_text = text[:280] + "..." if len(text) > 280 else text
    streamlit_marquee(
        content=truncated_text,
        **settings,
        key=f"marquee_{key_suffix}"
    )
    st.write("")

def get_high_info_terms(text: str, top_n=10) -> list:
    """
    📌 Extract top_n frequent words & bigrams (excluding common stopwords).
    Useful for generating short descriptive keywords from Q/A content.
    """
    stop_words = set(['the', 'a', 'an', 'and', 'or', 'but', 'in', 'on', 'at', 'to', 'for', 'of', 'with'])
    words = re.findall(r'\b\w+(?:-\w+)*\b', text.lower())
    bi_grams = [' '.join(pair) for pair in zip(words, words[1:])]
    combined = words + bi_grams
    filtered = [term for term in combined if term not in stop_words and len(term.split()) <= 2]
    counter = Counter(filtered)
    return [term for term, freq in counter.most_common(top_n)]

def clean_text_for_filename(text: str) -> str:
    """
    🏷️ Remove special chars & short unhelpful words from text for safer filenames.
    Returns a lowercased, underscore-joined token string.
    """
    text = text.lower()
    text = re.sub(r'[^\w\s-]', '', text)
    words = text.split()
    stop_short = set(['the', 'and', 'for', 'with', 'this', 'that', 'ai', 'library'])
    filtered = [w for w in words if len(w) > 3 and w not in stop_short]
    return '_'.join(filtered)[:200]

def generate_filename(prompt, response, file_type="md", max_length=200):
    """
    📁 Create a shortened filename based on prompt+response content:
      1) Extract top info terms,
      2) Combine snippet from prompt+response,
      3) Remove duplicates,
      4) Truncate if needed.
    """
    prefix = format_timestamp_prefix() + "_"
    combined_text = (prompt + " " + response)[:200]  
    info_terms = get_high_info_terms(combined_text, top_n=5)  
    snippet = (prompt[:40] + " " + response[:40]).strip()
    snippet_cleaned = clean_text_for_filename(snippet)
    
    # Remove duplicates
    name_parts = info_terms + [snippet_cleaned]
    seen = set()
    unique_parts = []
    for part in name_parts:
        if part not in seen:
            seen.add(part)
            unique_parts.append(part)
    
    full_name = '_'.join(unique_parts).strip('_')
    leftover_chars = max_length - len(prefix) - len(file_type) - 1
    if len(full_name) > leftover_chars:
        full_name = full_name[:leftover_chars]
    
    return f"{prefix}{full_name}.{file_type}"

def create_file(prompt, response, file_type="md"):
    """
    📝 Create a text file from prompt + response with a sanitized filename.
    Returns the created filename.
    """
    filename = generate_filename(prompt.strip(), response.strip(), file_type)
    with open(filename, 'w', encoding='utf-8') as f:
        f.write(prompt + "\n\n" + response)
    return filename



def get_download_link(file, file_type="zip"):
    """
    Convert a file to base64 and return an HTML link for download.
    """
    with open(file, "rb") as f:
        b64 = base64.b64encode(f.read()).decode()
    if file_type == "zip":
        return f'<a href="data:application/zip;base64,{b64}" download="{os.path.basename(file)}">📂 Download {os.path.basename(file)}</a>'
    elif file_type == "mp3":
        return f'<a href="data:audio/mpeg;base64,{b64}" download="{os.path.basename(file)}">🎵 Download {os.path.basename(file)}</a>'
    elif file_type == "wav":
        return f'<a href="data:audio/wav;base64,{b64}" download="{os.path.basename(file)}">🔊 Download {os.path.basename(file)}</a>'
    elif file_type == "md":
        return f'<a href="data:text/markdown;base64,{b64}" download="{os.path.basename(file)}">📝 Download {os.path.basename(file)}</a>'
    else:
        return f'<a href="data:application/octet-stream;base64,{b64}" download="{os.path.basename(file)}">Download {os.path.basename(file)}</a>'

def clean_for_speech(text: str) -> str:
    """Clean up text for TTS output."""
    text = text.replace("\n", " ")
    text = text.replace("</s>", " ")
    text = text.replace("#", "")
    text = re.sub(r"\(https?:\/\/[^\)]+\)", "", text)
    text = re.sub(r"\s+", " ", text).strip()
    return text

async def edge_tts_generate_audio(text, voice="en-US-AriaNeural", rate=0, pitch=0, file_format="mp3"):
    """Async TTS generation with edge-tts library."""
    text = clean_for_speech(text)
    if not text.strip():
        return None
    rate_str = f"{rate:+d}%"
    pitch_str = f"{pitch:+d}Hz"
    communicate = edge_tts.Communicate(text, voice, rate=rate_str, pitch=pitch_str)
    out_fn = generate_filename(text, text, file_type=file_format)
    await communicate.save(out_fn)
    return out_fn

def sync_edge_tts_generate_audio(text, voice="en-US-AriaNeural", rate=0, pitch=0, file_format="mp3"):
    """Async TTS generation with edge-tts library."""
    text = clean_for_speech(text)
    if not text.strip():
        return None
    rate_str = f"{rate:+d}%"
    pitch_str = f"{pitch:+d}Hz"
    communicate = edge_tts.Communicate(text, voice, rate=rate_str, pitch=pitch_str)
    out_fn = generate_filename(text, text, file_type=file_format)
    #await communicate.save(out_fn)
    return out_fn

def speak_with_edge_tts(text, voice="en-US-AriaNeural", rate=0, pitch=0, file_format="mp3"):
    """Wrapper for the async TTS generate call."""
    edge_tts_generate_audio(text, voice, rate, pitch, file_format)
    return 

def play_and_download_audio(file_path, file_type="mp3"):
    """Streamlit audio + a quick download link."""
    if file_path and os.path.exists(file_path):
        st.audio(file_path)
        dl_link = get_download_link(file_path, file_type=file_type)
        st.markdown(dl_link, unsafe_allow_html=True)

def save_qa_with_audio(question, answer, voice=None):
    """Save Q&A to markdown and also generate audio."""
    if not voice:
        voice = st.session_state['tts_voice']
    
    combined_text = f"# Question\n{question}\n\n# Answer\n{answer}"
    md_file = create_file(question, answer, "md")
    audio_text = f"{question}\n\nAnswer: {answer}"
    audio_file = speak_with_edge_tts(
        audio_text,
        voice=voice,
        file_format=st.session_state['audio_format']
    )
    return md_file, audio_file

    
# ─────────────────────────────────────────────────────────
# 4. OPTIMIZED AUDIO GENERATION (ASYNC TTS + CACHING)
# ─────────────────────────────────────────────────────────

def clean_for_speech(text: str) -> str:
    """
    🔉 Clean up text for TTS output with enhanced cleaning.
    Removes markdown, code blocks, links, etc.
    """
    with PerformanceTimer("text_cleaning"):
        # Remove markdown headers
        text = re.sub(r'#+ ', '', text)
        # Remove link formats [text](url)
        text = re.sub(r'\[([^\]]+)\]\([^\)]+\)', r'\1', text)
        # Remove emphasis markers (*, _, ~, `)
        text = re.sub(r'[*_~`]', '', text)
        # Remove code blocks
        text = re.sub(r'```[\s\S]*?```', '', text)
        text = re.sub(r'`[^`]*`', '', text)
        # Remove excess whitespace
        text = re.sub(r'\s+', ' ', text).replace("\n", " ")
        # Remove hidden S tokens
        text = text.replace("</s>", " ")
        # Remove URLs
        text = re.sub(r'https?://\S+', '', text)
        text = re.sub(r'\(https?://[^\)]+\)', '', text)
        text = text.strip()
        return text

async def async_edge_tts_generate(
    text: str,
    voice: str,
    rate: int = 0,
    pitch: int = 0,
    file_format: str = "mp3"
) -> Tuple[Optional[str], float]:
    """
    🎶 Asynchronous TTS generation with caching and performance tracking.
    Returns (filename, generation_time).
    """
    with PerformanceTimer("tts_generation") as timer:
        # ▶ Clean & validate text
        text = clean_for_speech(text)
        if not text.strip():
            return None, 0
        
        # ▶ Check cache (avoid regenerating the same TTS)
        cache_key = f"{text[:100]}_{voice}_{rate}_{pitch}_{file_format}"
        if cache_key in st.session_state['audio_cache']:
            return st.session_state['audio_cache'][cache_key], 0
        
        try:
            # ▶ Generate audio
            rate_str = f"{rate:+d}%"
            pitch_str = f"{pitch:+d}Hz"
            communicate = edge_tts.Communicate(text, voice, rate=rate_str, pitch=pitch_str)
            
            # ▶ Generate unique filename
            timestamp = datetime.now().strftime("%Y%m%d_%H%M%S")
            filename = f"audio_{timestamp}_{random.randint(1000, 9999)}.{file_format}"
            
            # ▶ Save audio file
            await communicate.save(filename)
            
            # ▶ Store in cache
            st.session_state['audio_cache'][cache_key] = filename
            
            # ▶ Return path + timing
            return filename, time.time() - timer.start_time
        
        except Exception as e:
            st.error(f"❌ Error generating audio: {str(e)}")
            return None, 0

async def async_save_qa_with_audio(
    question: str,
    answer: str,
    voice: Optional[str] = None
) -> Tuple[str, Optional[str], float, float]:
    """
    📝 Asynchronously save Q&A to markdown, then generate audio if enabled.
    Returns (md_file, audio_file, md_time, audio_time).
    """
    voice = voice or st.session_state['tts_voice']
    
    with PerformanceTimer("qa_save") as timer:
        # ▶ Save Q/A as markdown
        md_start = time.time()
        md_file = create_file(question, answer, "md")
        md_time = time.time() - md_start
        
        # ▶ Generate audio (if globally enabled)
        audio_file = None
        audio_time = 0
        if st.session_state['enable_audio']:
            audio_text = f"{question}\n\nAnswer: {answer}"
            audio_file, audio_time = await async_edge_tts_generate(
                audio_text,
                voice=voice,
                file_format=st.session_state['audio_format']
            )
        
        return md_file, audio_file, md_time, audio_time

def save_qa_with_audio(question, answer, voice=None):
    """Save Q&A to markdown and also generate audio."""
    if not voice:
        voice = st.session_state['tts_voice']
    
    combined_text = f"# Question\n{question}\n\n# Answer\n{answer}"
    md_file = create_file(question, answer, "md")
    audio_text = f"{question}\n\nAnswer: {answer}"
    audio_file = speak_with_edge_tts(
        audio_text,
        voice=voice,
        file_format=st.session_state['audio_format']
    )
    return md_file, audio_file




def create_download_link_with_cache(file_path: str, file_type: str = "mp3") -> str:
    """
    ⬇️ Create a download link for a file with caching & error handling.
    """
    with PerformanceTimer("download_link_generation"):
        cache_key = f"dl_{file_path}"
        if cache_key in st.session_state['download_link_cache']:
            return st.session_state['download_link_cache'][cache_key]
        
        try:
            with open(file_path, "rb") as f:
                b64 = base64.b64encode(f.read()).decode()
            filename = os.path.basename(file_path)
            
            if file_type == "mp3":
                link = f'<a href="data:audio/mpeg;base64,{b64}" download="{filename}">🎵 Download {filename}</a>'
            elif file_type == "wav":
                link = f'<a href="data:audio/wav;base64,{b64}" download="{filename}">🔊 Download {filename}</a>'
            elif file_type == "md":
                link = f'<a href="data:text/markdown;base64,{b64}" download="{filename}">📝 Download {filename}</a>'
            else:
                link = f'<a href="data:application/octet-stream;base64,{b64}" download="{filename}">⬇️ Download {filename}</a>'
            
            st.session_state['download_link_cache'][cache_key] = link
            return link
        
        except Exception as e:
            st.error(f"❌ Error creating download link: {str(e)}")
            return ""

# ─────────────────────────────────────────────────────────
# 5. RESEARCH / ARXIV FUNCTIONS
# ─────────────────────────────────────────────────────────

def parse_arxiv_refs(ref_text: str):
    """
    📜 Given a multi-line markdown with Arxiv references,
    parse them into a list of dicts: {date, title, url, authors, summary}.
    """
    if not ref_text:
        return []
    results = []
    current_paper = {}
    lines = ref_text.split('\n')
    
    for i, line in enumerate(lines):
        if line.count('|') == 2:
            # Found a new paper line
            if current_paper:
                results.append(current_paper)
                if len(results) >= 20:
                    break
            try:
                header_parts = line.strip('* ').split('|')
                date = header_parts[0].strip()
                title = header_parts[1].strip()
                url_match = re.search(r'(https://arxiv.org/\S+)', line)
                url = url_match.group(1) if url_match else f"paper_{len(results)}"
                
                current_paper = {
                    'date': date,
                    'title': title,
                    'url': url,
                    'authors': '',
                    'summary': '',
                    'full_audio': None,
                    'download_base64': '',
                }
            except Exception as e:
                st.warning(f"⚠️ Error parsing paper header: {str(e)}")
                current_paper = {}
                continue
        elif current_paper:
            # If authors not set, fill it; otherwise, fill summary
            if not current_paper['authors']:
                current_paper['authors'] = line.strip('* ')
            else:
                if current_paper['summary']:
                    current_paper['summary'] += ' ' + line.strip()
                else:
                    current_paper['summary'] = line.strip()
    
    if current_paper:
        results.append(current_paper)
    
    return results[:20]

def create_paper_links_md(papers):
    """
    🔗 Create a minimal .md content linking to each paper's Arxiv URL.
    """
    lines = ["# Paper Links\n"]
    for i, p in enumerate(papers, start=1):
        lines.append(f"{i}. **{p['title']}** — [Arxiv]({p['url']})")
    return "\n".join(lines)

async def create_paper_audio_files(papers, input_question):
    """
    🎧 For each paper, generate TTS audio summary and store the path in `paper['full_audio']`.
    Also creates a base64 download link in `paper['download_base64']`.
    """
    for paper in papers:
        try:
            audio_text = f"{paper['title']} by {paper['authors']}. {paper['summary']}"
            audio_text = clean_for_speech(audio_text)
            file_format = st.session_state['audio_format']
            audio_file, _ = await async_edge_tts_generate(
                audio_text, 
                voice=st.session_state['tts_voice'], 
                file_format=file_format
            )
            paper['full_audio'] = audio_file
            
            if audio_file:
                # Convert to base64 link
                ext = file_format
                download_link = create_download_link_with_cache(audio_file, file_type=ext)
                paper['download_base64'] = download_link

        except Exception as e:
            st.warning(f"⚠️ Error processing paper {paper['title']}: {str(e)}")
            paper['full_audio'] = None
            paper['download_base64'] = ''

def display_papers(papers, marquee_settings):
    """
    📑 Display paper info in the main area with marquee + expanders + audio.
    """
    st.write("## 🔎 Research Papers")
    for i, paper in enumerate(papers, start=1):
        marquee_text = f"📄 {paper['title']} | 👤 {paper['authors'][:120]} | 📝 {paper['summary'][:200]}"
        display_marquee(marquee_text, marquee_settings, key_suffix=f"paper_{i}")
        
        with st.expander(f"{i}. 📄 {paper['title']}", expanded=True):
            st.markdown(f"**{paper['date']} | {paper['title']}** — [Arxiv Link]({paper['url']})")
            st.markdown(f"*Authors:* {paper['authors']}")
            st.markdown(paper['summary'])
            if paper.get('full_audio'):
                st.write("📚 **Paper Audio**")
                st.audio(paper['full_audio'])
                if paper['download_base64']:
                    st.markdown(paper['download_base64'], unsafe_allow_html=True)

def display_papers_in_sidebar(papers):
    """
    🔎 Mirrors the paper listing in the sidebar with expanders, audio, etc.
    """
    st.sidebar.title("🎶 Papers & Audio")
    for i, paper in enumerate(papers, start=1):
        with st.sidebar.expander(f"{i}. {paper['title']}"):
            st.markdown(f"**Arxiv:** [Link]({paper['url']})")
            if paper['full_audio']:
                st.audio(paper['full_audio'])
                if paper['download_base64']:
                    st.markdown(paper['download_base64'], unsafe_allow_html=True)
            st.markdown(f"**Authors:** {paper['authors']}")
            if paper['summary']:
                st.markdown(f"**Summary:** {paper['summary'][:300]}...")

# ─────────────────────────────────────────────────────────
# 6. ZIP FUNCTION
# ─────────────────────────────────────────────────────────

def create_zip_of_files(md_files, mp3_files, wav_files, input_question):
    """
    📦 Zip up all relevant files, generating a short name from high-info terms.
    Returns the zip filename if created, else None.
    """
    md_files = [f for f in md_files if os.path.basename(f).lower() != 'readme.md']
    all_files = md_files + mp3_files + wav_files
    if not all_files:
        return None

    all_content = []
    for f in all_files:
        if f.endswith('.md'):
            with open(f, "r", encoding='utf-8') as file:
                all_content.append(file.read())
        elif f.endswith('.mp3') or f.endswith('.wav'):
            basename = os.path.splitext(os.path.basename(f))[0]
            words = basename.replace('_', ' ')
            all_content.append(words)
    
    all_content.append(input_question)
    combined_content = " ".join(all_content)
    info_terms = get_high_info_terms(combined_content, top_n=10)
    
    timestamp = format_timestamp_prefix()
    name_text = '-'.join(term for term in info_terms[:5])  
    short_zip_name = (timestamp + "_" + name_text)[:20] + ".zip"

    with zipfile.ZipFile(short_zip_name, 'w') as z:
        for f in all_files:
            z.write(f)
    return short_zip_name

# ─────────────────────────────────────────────────────────
# 7. MAIN AI LOGIC: LOOKUP & TAB HANDLERS
# ─────────────────────────────────────────────────────────


def perform_ai_lookup(q, vocal_summary=True, extended_refs=False, 
                     titles_summary=True, full_audio=False, useArxiv=True, useArxivAudio=False):
    """Main routine that uses Anthropic (Claude) + Gradio ArXiv RAG pipeline."""
    start = time.time()
    ai_constitution = """
    You are a medical and machine learning review board expert and streamlit python and html5 expert. You are tasked with creating a streamlit app.py and requirements.txt for a solution that answers the questions with a working app to demonstrate. You are to use the paper list below to answer the question thinking through step by step how to create a streamlit app.py and requirements.txt for the solution that answers the questions with a working app to demonstrate.
    """

    # --- 1) Claude API
    client = anthropic.Anthropic(api_key=anthropic_key)
    user_input = q
    response = client.messages.create(
        model="claude-3-sonnet-20240229",
        max_tokens=1000,
        messages=[
            {"role": "user", "content": user_input}
        ])
    st.write("Claude's reply 🧠:")
    st.markdown(response.content[0].text)

    # Save & produce audio
    result = response.content[0].text
    create_file(q, result) 
    md_file, audio_file = save_qa_with_audio(q, result)
    st.subheader("📝 Main Response Audio")
    play_and_download_audio(audio_file, st.session_state['audio_format'])


    if useArxiv:
        q = q + result   # Feed Arxiv the question and Claude's answer for prompt fortification to get better answers and references
        # --- 2) Arxiv RAG
        #st.write("Arxiv's AI this Evening is Mixtral 8x7B...")
        st.write('Running Arxiv RAG with Claude inputs.')
        #st.code(q, language="python", line_numbers=True, wrap_lines=True)
        
        client = Client("awacke1/Arxiv-Paper-Search-And-QA-RAG-Pattern")
        refs = client.predict(
            q, 
            10, 
            "Semantic Search", 
            "mistralai/Mixtral-8x7B-Instruct-v0.1",
            api_name="/update_with_rag_md"
        )[0]

        #r2 = client.predict(
        #    q, 
        #    "mistralai/Mixtral-8x7B-Instruct-v0.1", 
        #    True, 
        #    api_name="/ask_llm"
        #)
        #result = f"### 🔎 {q}\n\n{r2}\n\n{refs}"
        
        result = f"🔎 {q}\n\n{refs}"  # use original question q with result paired with paper references for best prompt fortification
        
        md_file, audio_file = save_qa_with_audio(q, result)
        st.subheader("📝 Main Response Audio")
        play_and_download_audio(audio_file, st.session_state['audio_format'])

        # --- 3) Parse + handle papers
        papers = parse_arxiv_refs(refs)
        if papers:
            # Create minimal links page first
            paper_links = create_paper_links_md(papers)
            links_file = create_file(q, paper_links, "md")
            st.markdown(paper_links)

            # Then create audio for each paper
            if useArxivAudio:
                create_paper_audio_files(papers, input_question=q)

            display_papers(papers, get_marquee_settings()) # scrolling marquee per paper and summary
            
            display_papers_in_sidebar(papers) # sidebar entry per paper and summary
        else:
            st.warning("No papers found in the response.")


        # --- 4) Claude API with arxiv list of papers to app.py
        client = anthropic.Anthropic(api_key=anthropic_key)
        user_input = q + '\n\n' + 'Use the reference papers below to answer the question by creating a python streamlit app.py and requirements.txt with python libraries for creating a single app.py application that answers the questions with working code to demonstrate.'+ '\n\n'
        response = client.messages.create(
            model="claude-3-sonnet-20240229",
            max_tokens=1000,
            messages=[
                {"role": "user", "content": user_input}
            ])
        r2 = response.content[0].text
        st.write("Claude's reply 🧠:")
        st.markdown(r2)
        

    
    elapsed = time.time() - start
    st.write(f"**Total Elapsed:** {elapsed:.2f} s")
    return result







def perform_ai_lookup_old(
    q,
    vocal_summary=True,
    extended_refs=False,
    titles_summary=True,
    full_audio=False
):
    """
    🔮 Main routine that uses Anthropic (Claude) + optional Gradio ArXiv RAG pipeline.
    Currently demonstrates calling Anthropic and returning the text.
    """
    with PerformanceTimer("ai_lookup"):
        start = time.time()
        
        # ▶ Example call to Anthropic (Claude)
        client = anthropic.Anthropic(api_key=anthropic_key)
        user_input = q
        
        # Here we do a minimal prompt, just to show the call
        # (You can enhance your prompt engineering as needed)
        response = client.completions.create(
            model="claude-2",
            max_tokens_to_sample=512,
            prompt=f"{anthropic.HUMAN_PROMPT} {user_input}{anthropic.AI_PROMPT}"
        )
        
        result_text = response.completion.strip()
        
        # ▶ Print and store
        st.write("### Claude's reply 🧠:")
        st.markdown(result_text)


        # Save & produce audio
        #create_file(q, result_text) 
        #md_file, audio_file = save_qa_with_audio(q, result_text)
        #st.subheader("📝 Main Response Audio")
        #play_and_download_audio(audio_file, st.session_state['audio_format'])


        
        # ▶ We'll add to the chat history
        st.session_state.chat_history.append({"user": q, "claude": result_text})
        
        # ▶ Return final text
        end = time.time()
        st.write(f"**Elapsed:** {end - start:.2f}s")

    return result_text

async def process_voice_input(text):
    """
    🎤 When user sends a voice query, we run the AI lookup + Q/A with audio.
    Then we store the resulting markdown & audio in session or disk.
    """
    if not text:
        return
    st.subheader("🔍 Search Results")
    
    # ▶ Call AI
    result = perform_ai_lookup(
        text, 
        vocal_summary=True,
        extended_refs=False,
        titles_summary=True,
        full_audio=True
    )
    
    # ▶ Save Q&A as Markdown + audio (async)
    md_file, audio_file, md_time, audio_time = await async_save_qa_with_audio(text, result)

    st.subheader("📝 Generated Files")
    st.write(f"**Markdown:** {md_file} (saved in {md_time:.2f}s)")
    if audio_file:
        st.write(f"**Audio:** {audio_file} (generated in {audio_time:.2f}s)")
        st.audio(audio_file)
        dl_link = create_download_link_with_cache(audio_file, file_type=st.session_state['audio_format'])
        st.markdown(dl_link, unsafe_allow_html=True)

def display_voice_tab():
    """
    🎙️ Display the voice input tab with TTS settings and real-time usage.
    """
    
    # ▶ Voice Settings
    st.sidebar.markdown("### 🎤 Voice Settings")
    caption_female = 'Top: 🌸 **Aria** – 🎶 **Jenny** – 🌺 **Sonia** – 🌌 **Natasha** – 🌷 **Clara**'
    caption_male   = 'Bottom: 🌟 **Guy** – 🛠️ **Ryan** – 🎻 **William** – 🌟 **Liam**'
    
    # Optionally, replace with your own local image or comment out
    try:
        st.sidebar.image('Group Picture - Voices.png', caption=caption_female + ' | ' + caption_male)
    except:
        st.sidebar.write('.')

    selected_voice = st.sidebar.selectbox(
        "👄 Select TTS Voice:",
        options=EDGE_TTS_VOICES,
        index=EDGE_TTS_VOICES.index(st.session_state['tts_voice'])
    )
    
    st.sidebar.markdown("""
    # 🎙️ Voice Character Agent Selector 🎭
    *Female Voices*:
    - 🌸 **Aria** – Elegant, creative storytelling  
    - 🎶 **Jenny** – Friendly, conversational  
    - 🌺 **Sonia** – Bold, confident  
    - 🌌 **Natasha** – Sophisticated, mysterious  
    - 🌷 **Clara** – Cheerful, empathetic  

    *Male Voices*:
    - 🌟 **Guy** – Authoritative, versatile  
    - 🛠️ **Ryan** – Approachable, casual  
    - 🎻 **William** – Classic, scholarly  
    - 🌟 **Liam** – Energetic, engaging
    """)
    

    # ▶ Audio Format
    st.markdown("### 🔊 Audio Format")
    selected_format = st.radio(
        "Choose Audio Format:",
        options=["MP3", "WAV"],
        index=0
    )

    # ▶ Update session state if changed
    if selected_voice != st.session_state['tts_voice']:
        st.session_state['tts_voice'] = selected_voice
        st.rerun()
    if selected_format.lower() != st.session_state['audio_format']:
        st.session_state['audio_format'] = selected_format.lower()
        st.rerun()

    # ▶ Text Input
    user_text = st.text_area("💬 Message:", height=100)
    user_text = user_text.strip().replace('\n', ' ')

    # ▶ Send Button
    if st.button("📨 Send"):
        # Run our process_voice_input as an async function
        asyncio.run(process_voice_input(user_text))

    # ▶ Chat History
    st.subheader("📜 Chat History")
    for c in st.session_state.chat_history:
        st.write("**You:**", c["user"])
        st.write("**Response:**", c["claude"])

# ─────────────────────────────────────────────────────────
# FILE HISTORY SIDEBAR
# ─────────────────────────────────────────────────────────

def display_file_history_in_sidebar():
    """
    📂 Shows a history of local .md, .mp3, .wav files (newest first),
    with quick icons and optional download links.
    """
    st.sidebar.markdown("---")
    st.sidebar.markdown("### 📂 File History")

    # ▶ Gather all files
    md_files = glob.glob("*.md")
    mp3_files = glob.glob("*.mp3")
    wav_files = glob.glob("*.wav")
    all_files = md_files + mp3_files + wav_files

    if not all_files:
        st.sidebar.write("No files found.")
        return

    # ▶ Sort newest first
    all_files = sorted(all_files, key=os.path.getmtime, reverse=True)

    #for f in all_files:
    #    fname = os.path.basename(f)
    #    ext = os.path.splitext(fname)[1].lower().strip('.')
    #    emoji = FILE_EMOJIS.get(ext, '📦')
    #    time_str = datetime.fromtimestamp(os.path.getmtime(f)).strftime("%Y-%m-%d %H:%M:%S")

        #with st.sidebar.expander(f"{emoji} {fname}"):
        #    st.write(f"**Modified:** {time_str}")
        #    if ext == "md":
        #        with open(f, "r", encoding="utf-8") as file_in:
        #            snippet = file_in.read(200).replace("\n", " ")
        #        if len(snippet) == 200:
        #            snippet += "..."
        #        st.write(snippet)
        #        dl_link = create_download_link_with_cache(f, file_type="md")
        #        st.markdown(dl_link, unsafe_allow_html=True)
        #    elif ext in ["mp3","wav"]:
        #        st.audio(f)
        #        dl_link = create_download_link_with_cache(f, file_type=ext)
        #        st.markdown(dl_link, unsafe_allow_html=True)
        #    else:
        #        dl_link = create_download_link_with_cache(f)
        #        st.markdown(dl_link, unsafe_allow_html=True)



    # Group files by their query prefix (timestamp_query)
    grouped_files = {}
    for f in all_files:
        fname = os.path.basename(f)
        prefix = '_'.join(fname.split('_')[:6])  # Get timestamp part
        if prefix not in grouped_files:
            grouped_files[prefix] = {'md': [], 'audio': [], 'loaded': False}
        
        ext = os.path.splitext(fname)[1].lower()
        if ext == '.md':
            grouped_files[prefix]['md'].append(f)
        elif ext in ['.mp3', '.wav']:
            grouped_files[prefix]['audio'].append(f)

    # Sort groups by timestamp (newest first)
    sorted_groups = sorted(grouped_files.items(), key=lambda x: x[0], reverse=True)

    # 🗑⬇️ Sidebar delete all and zip all download
    col1, col4 = st.sidebar.columns(2)
    with col1:
        if st.button("🗑 Delete All"):
            for f in all_files:
                os.remove(f)
            st.rerun()
            st.session_state.should_rerun = True
    with col4:
        if st.button("⬇️ Zip All"):
            zip_name = create_zip_of_files(md_files, mp3_files, wav_files, 
                                         st.session_state.get('last_query', ''))
            if zip_name:
                st.sidebar.markdown(get_download_link(zip_name, "zip"), 
                                  unsafe_allow_html=True)

    # Display grouped files
    for prefix, files in sorted_groups:
        # Get a preview of content from first MD file
        preview = ""
        if files['md']:
            with open(files['md'][0], "r", encoding="utf-8") as f:
                preview = f.read(200).replace("\n", " ")
                if len(preview) > 200:
                    preview += "..."

        # Create unique key for this group
        group_key = f"group_{prefix}"
        if group_key not in st.session_state:
            st.session_state[group_key] = False

        # Display group expander
        with st.sidebar.expander(f"📑 Query Group: {prefix}"):
            st.write("**Preview:**")
            st.write(preview)
            
            # Load full content button
            if st.button("📖 View Full Content", key=f"btn_{prefix}"):
                st.session_state[group_key] = True

            # Only show full content and audio if button was clicked
            if st.session_state[group_key]:
                # Display markdown files
                for md_file in files['md']:
                    with open(md_file, "r", encoding="utf-8") as f:
                        content = f.read()
                    st.markdown("**Full Content:**")
                    st.markdown(content)
                    st.markdown(get_download_link(md_file, file_type="md"), 
                              unsafe_allow_html=True)

                # Display audio files
                usePlaySidebar=False
                if usePlaySidebar:
                    for audio_file in files['audio']:
                        ext = os.path.splitext(audio_file)[1].replace('.', '')
                        st.audio(audio_file)
                        st.markdown(get_download_link(audio_file, file_type=ext), 
                                  unsafe_allow_html=True)





# ─────────────────────────────────────────────────────────
# MAIN APP
# ─────────────────────────────────────────────────────────

def main():
    # ▶ 1) Setup marquee UI in the sidebar
    update_marquee_settings_ui()
    marquee_settings = get_marquee_settings()

    # ▶ 2) Display the marquee welcome
    display_marquee(
        st.session_state['marquee_content'], 
        {**marquee_settings, "font-size": "28px", "lineHeight": "50px"},
        key_suffix="welcome"
    )

    # ▶ 3) Main action tabs and model use choices
    tab_main = st.radio("Action:", ["🎤 Voice", "📸 Media", "🔍 ArXiv", "📝 Editor"], 
                        horizontal=True)
    
    useArxiv = st.checkbox("Search Arxiv for Research Paper Answers", value=True)
    useArxivAudio = st.checkbox("Generate Audio File for Research Paper Answers", value=False)

    # ▶ 4) Show or hide custom component (optional example)
    mycomponent = components.declare_component("mycomponent", path="mycomponent")
    val = mycomponent(my_input_value="Hello from MyComponent")

    if val:
        val_stripped = val.replace('\\n', ' ')
        edited_input = st.text_area("✏️ Edit Input:", value=val_stripped, height=100)
        run_option = st.selectbox("Model:", ["Arxiv", "Other (demo)"])
        col1, col2 = st.columns(2)
        with col1:
            autorun = st.checkbox("⚙ AutoRun", value=True)
        with col2:
            full_audio = st.checkbox("📚FullAudio", value=False)

        input_changed = (val != st.session_state.old_val)

        if autorun and input_changed:
            st.session_state.old_val = val
            st.session_state.last_query = edited_input
            perform_ai_lookup(edited_input, 
                              vocal_summary=True, 
                              extended_refs=False, 
                              titles_summary=True, 
                              full_audio=full_audio, useArxiv=useArxiv, useArxivAudio=useArxivAudio)
        else:
            if st.button("▶ Run"):
                st.session_state.old_val = val
                st.session_state.last_query = edited_input
                perform_ai_lookup(edited_input, 
                                  vocal_summary=True, 
                                  extended_refs=False, 
                                  titles_summary=True, 
                                  full_audio=full_audio, useArxiv=useArxiv, useArxivAudio=useArxivAudio)

    # ─────────────────────────────────────────────────────────
    # TAB: ArXiv
    # ─────────────────────────────────────────────────────────
    if tab_main == "🔍 ArXiv":
        st.subheader("🔍 Query ArXiv")
        q = st.text_input("🔍 Query:", key="arxiv_query")
        
        st.markdown("### 🎛 Options")
        vocal_summary = st.checkbox("🎙ShortAudio", value=True, key="option_vocal_summary")
        extended_refs = st.checkbox("📜LongRefs", value=False, key="option_extended_refs")
        titles_summary = st.checkbox("🔖TitlesOnly", value=True, key="option_titles_summary")
        full_audio = st.checkbox("📚FullAudio", value=False, key="option_full_audio")
        full_transcript = st.checkbox("🧾FullTranscript", value=False, key="option_full_transcript")
        
        if q and st.button("🔍Run"):
            st.session_state.last_query = q
            result = perform_ai_lookup(q, 
                                       vocal_summary=vocal_summary, 
                                       extended_refs=extended_refs, 
                                       titles_summary=titles_summary, 
                                       full_audio=full_audio)
            if full_transcript:
                create_file(q, result, "md")

    # ─────────────────────────────────────────────────────────
    # TAB: Voice
    # ─────────────────────────────────────────────────────────
    elif tab_main == "🎤 Voice":
        display_voice_tab()

    # ─────────────────────────────────────────────────────────
    # TAB: Media
    # ─────────────────────────────────────────────────────────
    elif tab_main == "📸 Media":
        st.header("📸 Media Gallery")
        tabs = st.tabs(["🎵 Audio", "🖼 Images", "🎥 Video"])
        
        # ▶ AUDIO sub-tab
        with tabs[0]:
            st.subheader("🎵 Audio Files")
            audio_files = glob.glob("*.mp3") + glob.glob("*.wav")
            if audio_files:
                for a in audio_files:
                    with st.expander(os.path.basename(a)):
                        st.audio(a)
                        ext = os.path.splitext(a)[1].replace('.', '')
                        dl_link = create_download_link_with_cache(a, file_type=ext)
                        st.markdown(dl_link, unsafe_allow_html=True)
            else:
                st.write("No audio files found.")
        
        # ▶ IMAGES sub-tab
        with tabs[1]:
            st.subheader("🖼 Image Files")
            imgs = glob.glob("*.png") + glob.glob("*.jpg") + glob.glob("*.jpeg")
            if imgs:
                c = st.slider("Cols", 1, 5, 3, key="cols_images")
                cols = st.columns(c)
                for i, f in enumerate(imgs):
                    with cols[i % c]:
                        st.image(Image.open(f), use_container_width=True)
            else:
                st.write("No images found.")
        
        # ▶ VIDEO sub-tab
        with tabs[2]:
            st.subheader("🎥 Video Files")
            vids = glob.glob("*.mp4") + glob.glob("*.mov") + glob.glob("*.avi")
            if vids:
                for v in vids:
                    with st.expander(os.path.basename(v)):
                        st.video(v)
            else:
                st.write("No videos found.")

    # ─────────────────────────────────────────────────────────
    # TAB: Editor
    # ─────────────────────────────────────────────────────────
    elif tab_main == "📝 Editor":
        st.write("### 📝 File Editor (Minimal Demo)")
        st.write("Select or create a file to edit. More advanced features can be added as needed.")

    # ─────────────────────────────────────────────────────────
    # SIDEBAR: FILE HISTORY + PERFORMANCE METRICS
    # ─────────────────────────────────────────────────────────
    display_file_history_in_sidebar()
    log_performance_metrics()

    # ▶ Some light CSS styling
    st.markdown("""
    <style>
        .main { background: linear-gradient(to right, #1a1a1a, #2d2d2d); color: #fff; }
        .stMarkdown { font-family: 'Helvetica Neue', sans-serif; }
        .stButton>button { margin-right: 0.5rem; }
    </style>
    """, unsafe_allow_html=True)

    # ▶ Rerun if needed
    if st.session_state.should_rerun:
        st.session_state.should_rerun = False
        st.rerun()

# ─────────────────────────────────────────────────────────
# 8. RUN APP
# ─────────────────────────────────────────────────────────

if __name__ == "__main__":
    main()
```



