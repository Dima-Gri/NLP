## Embending geometry

* [The strange geometry of skip-gram with negative sampling](https://aclanthology.org/D17-1308.pdf) (**не прочитано**)
* PCA - способ изменить размерность ебмбендингов (**не прочитано**)
* t-SNE: [статья1](https://distill.pub/2016/misread-tsne/), [статья2](https://datareview.info/article/algoritm-t-sne-illyustrirovannyiy-vvodnyiy-kurs/) (**не прочитано**)

## Skip gram model

The Effect of Window Size
The size of the sliding window has a strong effect on the resulting vector similarities. For example, this paper notes that larger windows tend to produce more topical similarities (i.e. dog, bark and leash will be grouped together, as well as walked, run and walking), while smaller windows tend to produce more functional and syntactic similarities (i.e. Poodle, Pitbull, Rottweiler, or walking, running, approaching).

* [word2vec Parameter Learning Explained](https://arxiv.org/pdf/1411.2738.pdf) (**не прочитано**)
* [Efficient Estimation of Word Representations in Vector Space](https://arxiv.org/pdf/1301.3781.pdf) (**не прочитано**)
* [Distributed Representations of Words and Phrases and their Compositionality](https://proceedings.neurips.cc/paper_files/paper/2013/file/9aa42b31882ec039965f3c4923ce901b-Paper.pdf) (прочитано)


$$\mathbf{Loss} = -\dfrac{1}{T} \sum_{t=1}^T\sum_{|j|\le m}  - s(w_{t+j}, w_t) + \log \sum_{w\in V} exp(s(w, w_t))$$, где $s(a, b) = u_{a}^Tv_b$

Дает очень близкие результаты с SVD

## GLOVE
Объединение Word2Vec и Count-based метода на основе матрицы PMI

[GLOVE](https://aclanthology.org/D14-1162.pdf) (**не прочитано**)


## HAL model
HAL model учитывает дистанцию, на которой контекстное слово находится относительно центрального. Чем ближе к центру, тем больший вклад в контекст, тем больше связи между центральными и контекстными словами. Также HAL учитывает и расположение (слева или справа) относительно центрального слова

![image](https://github.com/Dima-Gri/NLP/assets/60757623/b54a2311-e8e1-48e9-848c-201946212548)

Эта матрица сгенерирована для текста "The Horse Raced Past the Barn Fell"

В строку записаны веса от ключевого слова(выбранная строка) до контекстного слова(в столбце), если оно находится левее в корпусе, иначе ставится 0.


В столбец записаны веса от ключевого слова(выбранный столбец) до контекстного слова(в строке), если оно находится правее в корпусе, иначе ставится 0.



[HAL model](https://link.springer.com/content/pdf/10.3758/BF03204766.pdf) (прочитано)

## FastText
FastText почти в точности идентичен SGNS, за исключением формирования векторов. Общий пайплайн обучения такой же

![image](https://github.com/Dima-Gri/NLP/assets/60757623/e73d216c-3001-43d6-bbac-c60597dddcfe)

Идея в том, чтобы бить слово на n-grams, то есть на некоторые части, дабы добиться морфологических связей. Таким образом набор контекстных векторов будет содержать n-gram. Перед тем, как в SGNS передать какой-то вектор, мы делим нужное слово на части, берем представление каждой части со славаря, суммируем и дальше уже продолжаем работать в SGNS

[FastText](https://arxiv.org/pdf/1607.04606.pdf) (прочитано)


## на досуге
[Man is to Computer Programmer as Woman is to Homemaker? Debiasing Word Embeddings](https://proceedings.neurips.cc/paper_files/paper/2016/file/a486cd07e4ac3d270571622f4f316ec5-Paper.pdf)

