# Open Source Spam Filter
An easy to use spam filter that can be selfhosted and be trained by yourself. It allows you to have full control over what is spam for your mail inbox.

## Architecture
The initial version of OSSF is going to be using the Naive Bayes Algorithm to determine if something is spam or not. It will come with a pre-trained English dataset that can be used out of the box. After the initial version it will be turned into an API that can be hooked into your own mail boxed through the use plugins.

### Pros of Naive Bayes
- It relies of the words of a mail and not the entire context. _Spammers/scammers tend to be dumb and use the same type of words in their spam mails_.
- It can be trained FAST and constantly improve based on new data.

### Cons
- If a scammer uses an image instead of text, it will not work. A way around this is to implement something like OCR to check the contents of an image.
- [Bayesian Poisoning](https://en.wikipedia.org/wiki/Bayesian_poisoning) is a technique that scammers might use to pollute the model. There are ways around it, more research from me is needed on this.

## Development
### Tools
In the beginning Jupyter Notebooks will be used located in the `Sandbox` folder to test implementations and rapidly develop a filter

### Dataset
In order to have an idea if our implementation will be working or not. We're going to use the "Spam Mails Dataset" from Kaggle. It can be downloaded [here](https://www.kaggle.com/venky73/spam-mails-dataset)

## Sources
- [Naive Bayes Spam Filtering](https://en.wikipedia.org/wiki/Naive_Bayes_spam_filtering) on Wikipedia

## License
The filter is released under an Apache 2.0 License.