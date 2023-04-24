What is word embeddings 

Word embeddings are a powerful technique for representing words in a high-dimensional vector space. They assign a numerical vector notation to each word based on its context in a document, allowing the relationships between words to be captured in a dense, low-dimensional representation.

Imagine you have a lot of words, just like you have a lot of bones in your body. But just like you can't see all of your bones from the outside, it's hard to understand all the meanings of the words just by looking at them. That's where word embeddings come in - they're like X-rays for words! Just like how an X-ray helps doctors see inside your body and understand how your bones fit together, word embeddings help computers understand how words fit together and what they mean. They make it easier for computers to understand what you're trying to say, just like X-rays make it easier for doctors to help you feel better.

Why word embeddings are required?

Word embeddings helps to understand the semantic and syntactic relation between the words of the corpus. These are useful when looking for the word similarity, word analogy and sentiment analysis.

Lets take a case where 

1. Take a turn to right 
2. Joe thinks he is always right 

Here the same word “right” has two different meanings.

One more situation :

1. Don’t leave him, Hang him.
2. The cat is hanging on the wall, looking down with curiosity.

In first sentence the word Hang has a serious impact in the context where as in the second sentence the word hangs describes a mere action.

A word can contain different set of meanings based on the context. 

If we try to represent words into numerical vectors similar words have close vector representations. 

Like the values of cat and dog should be similar, cat and car should be dissimilar.

Here is an example of vector representation from Word2Vec embeddings example :

```python
cat = [0.273, -0.087, 0.132, 0.345, -0.712, 0.091, 0.127, -0.386, -0.134, -0.657]
dog = [0.442, -0.721, 0.217, 0.754, -0.082, -0.010, 0.043, -0.114, -0.197, -0.353]
car = [0.096, -0.129, -0.122, 0.200, -0.126, -0.035, -0.305, -0.230, -0.283, -0.235]

Similarity between cat and dog : dot_product(cat,dog) = (0.273 * 0.442) + (-0.087 * -0.721) + (0.132 * 0.217) + (0.345 * 0.754) + (-0.712 * -0.082) + (0.091 * -0.010) + (0.127 * 0.043) + (-0.386 * -0.114) + (-0.134 * -0.197) + (-0.657 * -0.353) = 0.8374
```

Similarity between cat and car : dot_product(cat, car) = (0.273 * 0.096) + (-0.087 * -0.129) + (0.132 * -0.122) + (0.345 * 0.200) + (-0.712 * -0.126) + (0.091 * -0.035) + (0.127 * -0.305) + (-0.386 * -0.230) + (-0.134 * -0.283) + (-0.657 * -0.235) = 0.4192

As we see the similarity between cat and dog is more compared to cat and car.

What are different techniques of word embeddings

Word2Vec

GloVe

FastText

ELMo

BERT

How to apply word embeddings in real life: 

I have worked on Word2Vec on the house rental negotiations for people living in Arizona State. 
Dataset is House_rentals.txt is the rental negotitation between people.
