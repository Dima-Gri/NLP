PCA - способ изменить размерность ебмбендингов


t-SNE https://distill.pub/2016/misread-tsne/  (https://datareview.info/article/algoritm-t-sne-illyustrirovannyiy-vvodnyiy-kurs/)

## Skip gram model

* [word2vec Parameter Learning Explained](https://arxiv.org/pdf/1411.2738.pdf) (**не прочитано**)
* [Efficient Estimation of Word Representations in Vector Space](https://arxiv.org/pdf/1301.3781.pdf) (**не прочитано**)
* [Distributed Representations of Words and Phrases and their Compositionality](https://proceedings.neurips.cc/paper_files/paper/2013/file/9aa42b31882ec039965f3c4923ce901b-Paper.pdf) (прочитано)

Дает очень близкие результаты с SVD


## HAL model
HAL model учитывает дистанцию, на которой контекстное слово находится относительно центрального. Чем ближе к центру, тем больший вклад в контекст, тем больше связи между центральными и контекстными словами.


[HAL model](https://link.springer.com/content/pdf/10.3758/BF03204766.pdf) (прочитано)

## FastText
FastText почти в точности идентичен Word2Vec, за исключением формирования векторов. Общий пайплайн обучения такой же

![image](https://github.com/Dima-Gri/NLP/assets/60757623/e73d216c-3001-43d6-bbac-c60597dddcfe)

В 1.5 раза медленее обычного SGNS


[FastText](https://arxiv.org/pdf/1607.04606.pdf) (прочитано)

