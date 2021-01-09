# AMFTWE : Amharic FastText Word Embedding

Word embeddings have been used to represent the features for traditional classi-fiers, or as initializations in deep neural networks. Word embeddings are real valued representations for text by embedding both semantic and syntactic meanings obtained from unlabeled large corpus and are perhaps one of the key advances for the remarka-ble performance of deep learning methods on challenging NLP (natural language pro-cessing) problems such as content based fake news detection [1-3]. They are widely used in NLP tasks, such as sentiment analysis [4]; dependency parsing [5]; machine translation [6]; and fake news detection [7-14]. 

Considering the difficulty of the fake news detection problem, fake news detec-tion methods using deep learning can benefit from good quality word embeddings. Publicly available models, which are pre-trained on large amounts of data, have become a standard tool for many NLP applications, but are mostly available for the English language. Word embeddings for ‘low-resource’ languages are absent or are very limited. For the Amharic language, a fasttext based word embedding (cc_am_300 was trained by [15] using 300 dimensions. However, the number of word vectors are limited and also it contains uncleaned English tokens. 

The distributional hypothesis used in [16-18], utilizes the idea that the mean-ing of a word is captured by the contexts in which it appears, to learn word embeddings. Thus, the quality of word vectors directly depends on the amount and quality of data they were trained on. Based on this fact, in this work, we introduce high quality Amharic fasttext word embedding (AMFTWE ) trained on a huge corpus obtained by merging and deduplicating four corpora. GPAC, am131516, WIC and CACO using fasttext model with subword information [19]. As the quality of word embeddings directly depends on the amount and quality of data used, AMFTWE is of high quality. This is manifested in the superior performance of our fake news detection model when it uses AMFTWE compared with cc_am_300 [15]. The very reason we chose fasttext is because Amharic is one of the morphologi-cally rich languages and it is possible to improve vector representations for morphologically rich languages by using character level information [19].

We evaluated AMFTWE using extrinsic evaluation. In extrinsic word embedding evaluation, we use word embeddings as input features to a downstream task, in our case fake news detection, and measure changes in performance metrics specific to that task. For comparison purpose, we use the only available Amharic word embedding presented in [15]. This fake news detection task oriented evaluation shows that AMFTWE is of quality word embedding. It is also possible to evaluate this word embedding using intrinsic techniques. 

We believe AMFTWE will be a valuable resource for future computational linguistic researches and tool development. 

# AMFTWE Summary
    Dimensions: 50, 100, 200, and 300
    file_format: (.VEC) and (.BIN)
    #(.VEC)_files: 4 (one file for each dimension)
    #(.BIN)_files: 4 (one file for each dimension)
    file names : (.VEC) files: AMFTWE_50.vec, AMFTWE_100.vec, AMFTWE_200.vec, AMFTWE_3000.vec 
                 (.BIN) files: AMFTWE_50.bin, AMFTWE_100.bin, AMFTWE_200.bin, AMFTWE_300.bin
    file sizes: (.VEC) files: AMFTWE_50.vec = , AMFTWE_100.vec = , AMFTWE_200.vec = , AMFTWE_3000.vec =  
                (.BIN) files: AMFTWE_50.bin = , AMFTWE_100.bin = , AMFTWE_200.bin = , AMFTWE_300.bin = 
    repositories: 
    
# Citation
Please cite the following original paper/article associated with this dataset when you use it.

[ Gereme, Fantahun; Zhu, William; Ayall, Tewodros; Alemu, Dagmawi. 2021. "Combating Fake News in “Low-Resource” Languages: Amharic Fake News Detection Accompanied by Resource Crafting". Information 12, no. 1: 20. ]

available at url: [https://www.mdpi.com/2078-2489/12/1/20#cite]

           doi: https://doi.org/10.3390/info12010020


# References 

[1] Gereme F.B. and William Zh. Early detection of fake news, before it flies high. In Proceedings of the 2nd International Con-ference on Big Data Technologies (ICBDT2019), Jinan, China, 2019, ACM: New York, NY, USA, 2019, pp.142-148, 2019, DOI: https://doi.org/10.1145/3358528.3358567.

[2] Gereme F.B. and William Zh. Fighting Fake News Using Deep Learning: Pre-trained Word Embeddings and the Embedding Layer Investigated. In 2020 The 3rd International Conference on Computational Intelligence and Intelligent Systems (CIIS 2020), Tokyo, Japan, November 13–15, 2020, ACM: New York, NY, USA,2020,  DOI:https://doi.org/10.1145/3440840. 3440847.  

[3] Wang W.Y. Liar-Liar pants on fire: a new benchmark dataset for fake news detection, In proceedings of the 55th Annual Meeting of the Association for Computational Linguistics (Volume 2: Short Papers), Vancouver, Canada, 2017, Association for Computational Linguistics: Stroudsburg , USA, 2017, pp. 422–426, DOI: 10.18653/v1/P17-2067

[4] Tang D.; Wei F.; Yang N.; Zhou M.; Liu T. and Qin B. Learning sentiment-specific word embedding for twitter sentiment classification, In Proceedings of the 52nd Annual Meeting of the Association for Computational Linguistics 1, Baltimore, Maryland, 2014, Association for Computational Linguistics, Stroudsburg, USA, 2014. pp.1555-1565.

[5] Ouchi, H.; Duh, K.; Shindo, H. and Matsumoto, Y. Transition-based dependency parsing exploiting supertags, IEEE/ACM Transactions on Audio, Speech, and Language Processing 2016, 24(11), pp.2059–2068.

[6] Chen K.; Zhao T.; Yang M.; Liu L.; Tamura A.; Wang R.; Utiyama M. and Sumita E. A neural approach to source depend-ence based context model for statistical machine translation, IEEE/ACM Trans. Audio, Speech, Language Process 2018, 26(2), pp.266–280, DOI: 10.1109/TASLP.2017.2772846.

[7] Bajaj S. The pope has a new baby! fake news detection using deep learning. Stanford University, 2017.

[8] 12.	Karimi H. and Tanh J. Learning hierarchical discourse-level structure for fake news detection. In Proceedings of the 2019 Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technolo-gies.1, Minneapolis, Minnesota, USA, 2019, Association for Computational Linguistics: Stroudsburg, USA, 2019, pp.3432–3442, DOI:10.18653/v1/N19-1347.

[9] Khan J.Y.; Khondaker T.I.; Iqbal A. and Afroz S. A benchmark study on machine learning methods for fake news detection. arXiv:1905.04749, 2019.

[10] Singhania S.; Fernandez N. and Rao S. 3HAN: a deep neural network for fake news detection, International Conference on Neural Information Processing, Guangzhou, China, 2017, Springer, Cham, 2017, DOI: https://doi.org/10.1007/978-3-319-70096-0_59

[11] Tagami T.; Ouchi H.;  Asano H.; Hanawa K.; Uchiyama K.; Suzuki K.; Inui K.; Komiya A.; Fujimura A.; Yanai H.; Yam-ashita R. and Machino A. Suspicious news detection using micro blog text, Proceedings of the 32nd Pacific Asia Conference on Language, Information and Computation, Hong Kong, China, 2018, Association for Computational Linguistics: Strouds-burg, USA, 2018.

[12] Thota A.; Tilak P.; Ahluwalia S. and Lohia N. Fake news detection: a deep learning approach. SMU Data Science Review 2018, 1(3).

[13] Wang W.Y. Liar-Liar pants on fire: a new benchmark dataset for fake news detection, In proceedings of the 55th Annual Meeting of the Association for Computational Linguistics (Volume 2: Short Papers), Vancouver, Canada, 2017, Association for Computational Linguistics: Stroudsburg , USA, 2017, pp. 422–426, DOI: 10.18653/v1/P17-2067

[14] Yang Y.; Zheng L.; Zhang J.; Cui Q.; Li Z. and Yu P. TI-CNN: convolutional neural networks for fake news detection. arXiv preprint arXiv:1806.00749 2018.

[15] Grave E.; Bojanowski P.; Gupta P.; Joulin A. and Mikolov T. Learning Word Vectors for 157 Languages, Proceedings of the Eleventh International Conference on Language Resources and Evaluation (LREC 2018), Miyazaki, Japan, 2018, European Language Resources Association (ELRA): Paric, France,2018.

[16] Mikolov T.; Chen K.; Corrado G. and Dean J. Efficient estimation of word representations in vector space. Proceedings of the International Conference on Learning Representations (ICLR 2013), Scottsdale, USA, 2013.  

[17] Mikolov T.; Sutskever I.; Chen K.; Corrado G. and Dean J. Distributed representations of words and phrases and their com-positionality. Proceedings of the 26th International Conference on Neural Information Processing Systems - Volume 2, Lake Tahoe, USA, 2013, Curran Associates Inc.: Red Hook, USA, 2013, pp.3111–3119.

[18] Pennington J.; Socher R. and Manning C.D. GloVe-Global Vectors for word representation. In Proceedings of the 2014 Con-ference on Empirical Methods in Natural Language Processing (EMNLP), Doha, Qatar, 2014, Association for Computational Linguistics: Stroudsburg, USA, 2014, pp. 1532-1543, DOI: 10.3115/v1/D14-1162.

[19] Bojanowski P.; Grave E.; Joulin A. and Mikolov T. Enriching word vectors with subword information, TACL 2017, 5, pp.135-146, DOI: 10.1162/tacl_a_00051.

# Download : the embedding files will be uploaded soon


