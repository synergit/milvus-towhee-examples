From Chloe
# PAY ATTENTION
* The modified code is testing against a Milvus instance on cloud, so prepare the username and password. 
* It is interesting that the Milvus_client class doesn't allow `secure` parameter to be configured, so the workaround is
changing the code of __init__ method
```
/Users/chloe2023/.towhee/operators/ann-search/milvus-client/versions/main/milvus_client.py
```
with hard-coded `secure=False`. 
* You may encounter Milvus version doesn't match PyMilvus version error. Check PyMilvus Github for help:
https://github.com/milvus-io/pymilvus/blob/master/README.md

# Question Answering

Question answering is a classic problem in the field of natural language processing. While it sounds like an easy problem to solve, there is still a lot of research going on to improve the techniques that we have now. A large part of solving questions is finding questions that are similar to the one being asked. 



This example will show you how to find the similar asked question and get the answer. It mainly consists of two notebooks, hoping everyone can learn basic operations of Question Answering System through the [**getting started notebook**](./1_build_question_answering_engine.ipynb).

## Learn from Notebook

- [Getting started](1_build_question_answering_engine.ipynb)

In this notebook you will get the prerequisites, how to complete a simple question answering system and release a showcase.
