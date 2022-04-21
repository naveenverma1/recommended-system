# recommended-system using seldon-core and fastai


there are two types of filterations-  

1.Collaborative Filtering 
2.Content-based filtering

implementation of collaborative filtering -

Types of collaborative filtering techniques
• Memory based
• Model based
* Deep Learning


Python Implementations
• Surprise package
• fast.ai library


Memory-Based Collaborative Filtering-- 
Item-Item Collaborative Filtering: “Users who liked this item also liked …”
User-Item Collaborative Filtering: “Users who are similar to you also liked

 no training or optimization is involved, it is an easy to use approach. But its performance decreases when we have sparse data(amazon example)_ which hinders scalability of this approach for most of the real-world problems.
non parametric ML approaches like KNN come under Memory based approach

links - https://www.ethanrosenthal.com/2015/11/02/intro-to-collaborative-filtering/

Model based

in this approach, CF models are developed using machine learning algorithms to predict user’s rating of unrated items. As per my understanding, the algorithms in this approach can further be broken down into 3 sub-types.

![image](https://user-images.githubusercontent.com/39947864/164454118-2dcd10e4-7a6e-4772-930d-c538d607139d.png)

Matrix Factorization (MF): The idea behind such models is that attitudes or preferences of a user can be determined by a small number of hidden factors. We can call these factors as Embeddings..

these hidden factors can be no. of clicks, impressions ,installs, 
to learn more about embeddings - https://towardsdatascience.com/structured-deep-learning-b8ca4138b848

  Matrix factorization can be done by various methods one of the python library is fastai and also surprise package




Implementation example for fast ai- 

https://medium.com/@shik1470/63b00b9739ce
https://medium.com/@shik1470/919da17ecefb


We can use this algorithm for recommendation and deploy it on seldon core

Seldon core converts your ML models (Tensorflow, Pytorch, H2o, etc.) or language wrappers (Python, Java, etc.) into production REST/GRPC microservices.

Seldon core prodide some endpoints we can process out fast ai logic  in that and it will return us recommendations

They have swagger ui for that to https://codeshare.io/Qnz8Lx  copy this code in swagger editor then you can see swagger ui

https://editor.swagger.io/





important links -- 
1 https://towardsdatascience.com/a-gentle-introduction-to-recommendation-systems-eaddcbde07ce
2 https://towardsdatascience.com/the-best-tool-for-better-recommendations-systems-e57142b45f11
3 https://www.kaggle.com/code/fuzzywizard/rec-sys-collaborative-filtering-dl-techniques/notebook
4 https://github.com/fastai/fastai/tree/master/fastai
5 https://angeleastbengal.medium.com/recommender-system-using-collaborative-filtering-in-pyspark-b98eab2aea75
6 https://github.com/groverpr/Machine-Learning/blob/master/notebooks/02_Collaborative_Filtering.ipynb
7 https://www.ethanrosenthal.com/2015/11/02/intro-to-collaborative-filtering/
8 https://analyticsindiamag.com/a-guide-to-surprise-python-tool-for-recommender-systems/
9 https://surprise.readthedocs.io/en/v1.1.1/prediction_algorithms_package.html
10 https://docs.fast.ai/quick_start.html

intro recommended systems- 
1 https://www.youtube.com/watch?v=giIXNoiqO_U&t=263s&ab_channel=ArtificialIntelligence-AllinOne
2 https://www.youtube.com/watch?v=9siFuMMHNIA&ab_channel=ArtificialIntelligence-AllinOne
3 https://www.youtube.com/watch?v=9AP-DgFBNP4&ab_channel=ArtificialIntelligence-AllinOne
4 https://www.youtube.com/watch?v=YW2b8La2ICo&ab_channel=ArtificialIntelligence-AllinOne

seldon core- 
1 https://docs.seldon.io/projects/seldon-core/en/latest/workflow/github-readme.html
2 https://docs.seldon.io/projects/seldon-core/en/latest/reference/apis/openapi.html?highlight=swagger
3 https://medium.com/analytics-vidhya/manage-ml-deployments-like-a-boss-deploy-your-first-ab-test-with-sklearn-kubernetes-and-b10ae0819dfe
4 https://medium.com/analytics-vidhya/deploy-your-first-deep-learning-model-on-kubernetes-with-python-keras-flask-and-docker-575dc07d9e76
5 https://www.latentview.com/data-engineering-lp/introduction-to-seldon-core/

famous recommended systems- https://github.com/topics/recommender-system

How does Netflix recommend movies? Matrix Factorization - https://www.youtube.com/watch?v=ZspR5PZemcs&ab_channel=Serrano.Academy






