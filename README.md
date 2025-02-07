# FiveMinuteTalks
Auto Presentation Teleprompter AI For Teaching in Five Minutes

I am working on a ai app.py which I am using to create audio summaries of research papers and discuss what their impact on learning AI can be for training AI and people at once using audio, text, and speech modalities.  The workflow is voice in (spoken) to present a request, then a frontier model answers the question or request initially and inherits some degree of safety and training of the response from this initial request.  With it it then uses both inputs to search an AI embeddings using semantic search RAG ai which answers with selection of the top twenty research papers of the topic at hand.  This is shown in markdown and also marquee displays like singular teleprompters for each paper.  Then the paper link to abstract, the pdf, and the paper title and authors, and the paper summary are read aloud into wav files using a voice the user selected using the edge TTS voices (7).  Lets create a mermaid model for this.  My ideal would be how to create a live 5 minute talk which is perfecctly timed as 15 seconds of read aloud per paper.  Help me with the graph as mermaid model first then I would like to share my code with you and you help me create a csv output for the dataset of assets, we save the assets and then on the interface we prepare the user for recording the five minute video where they read aloud request, each paper summary (abbreviated to match words per minute voice rate) and then crosses the timing finish line at exactly 5 minutes.    Below is a sample of output for our first test together:   

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

Claude's reply 🧠:

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
