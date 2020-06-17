# Emojify!

Here, we are going to use word vector representations to build an Emojifier. 

The emojifier app can help add emojis to text messages more expressive.
>"Congratulations on the promotion! Let's get coffee and talk. Love you!"   

The emojifier can automatically turn this into:
>"Congratulations on the promotion! 👍 Let's get coffee and talk. ☕️ Love you! ❤️"

* The implemented model, when inputs a sentence (such as "Let's go see the baseball game tonight!") will find the most appropriate emoji to be used with this sentence (⚾️).

#### Using word vectors to improve emoji lookups
* In many emoji interfaces, you need to remember that ❤️ is the "heart" symbol rather than the "love" symbol. 
    * In other words, you'll have to remember to type "heart" to find the desired emoji, and typing "love" won't bring up that symbol.
* We can make a more flexible emoji interface by using word vectors!
* When using word vectors, even if our training set explicitly relates only a few words to a particular emoji, the algorithm will be able to generalize and associate additional words in the test set to the same emoji.
    * This works even if those additional words don't even appear in the training set. 
    * This allows you to build an accurate classifier mapping from sentences to emojis, even using a small training set. 

#### We have two Emojifier's implemented below
1. A baseline model (Emojifier-V1) using word embeddings.
2. A more sophisticated model (Emojifier-V2) that further incorporates an LSTM. 
