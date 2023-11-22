PCA - способ изменить размерность ебмбендингов


t-SNE https://distill.pub/2016/misread-tsne/  (https://datareview.info/article/algoritm-t-sne-illyustrirovannyiy-vvodnyiy-kurs/)

## Skip gram model

Word2Vec статья: https://arxiv.org/pdf/1411.2738.pdf

Дает очень близкие результаты с SVD


## HAL model
HAL model учитывает дистанцию, на которой контекстное слово находится относительно центрального. Чем ближе к центру, тем больший вклад в контекст, тем больше связи между центральными и контекстными словами.

(https://link.springer.com/content/pdf/10.3758/BF03204766.pdf)



## FastText
FastText почти в точности идентичен Word2Vec, за исключением формирования векторов. Общий пайплайн обучения такой же

![image](https://github.com/Dima-Gri/NLP/assets/60757623/e73d216c-3001-43d6-bbac-c60597dddcfe)

В 1.5 раза медленее обычного SGNS


Статья: https://arxiv.org/pdf/1607.04606.pdf

