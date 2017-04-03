# Title

Solving Fake News - From Data Collection to Classification

## Abstract

In 2007, the Journal of Mass Media Ethics had an article with the title: [The Role of Journalist and the Performance of Journalism: Ethical Lessons From “Fake” News (Seriously)](http://www.tandfonline.com/doi/abs/10.1080/08900520701583586). It suggests that that Jon Stewart of The Daily Show with Jon Stewart and Stephen Colbert of The Colbert Report (TCR) are a new kind of journalist - but that they lack the journalists moral commitment, and are not hence restricted to morally report news. Now, while the actual content of the paper may not be relevant to the problem we intend to explore, it is certainly curious to note the word "Seriously" in the title - and only wonder what the authors would exclaim how serious the Fake News problem has become, 10 years from when the article was written!

In the age of post-truth politics where the debate is more of an appeals to emotion as opposed to policies, Fake News is more relevant (and dangerous) before. The 2016 American Presidential elections is perhaps the most pertinent example, where Fake News on social media was a huge debate. 

I propose an attempt to better understand this problem - by crawling for data, organising data, reading relevant scientific and journalistic literature on Fake News, and attempt to solve this problem using a predictive model. As for which model we decide to use, a Neural Network seems like a popular choice, but more discussion on this can be made when our data-set is finalised. No machine learning model is worth anything without data - after all, [garbage in, grabage out](https://en.wikipedia.org/wiki/Garbage_in,_garbage_out)! 

A final product which we would like to see is a thouroughly documented GitHub repository which features all the steps of our project. Regular blog posts/infographics about the findings and illustrative Jupyter Notebooks would help in making the public aware of the project. 

## Technical Details

With the spike in the amount of Fake News articles lately, webites such as [Media Bias Fact Check](https://mediabiasfactcheck.com) and [Fake News Checker](https://www.fakenewschecker.com) are useful in identifying which websites spread fake news or publish/share fake news. Crawling these websites to create a databse of articles and headlines which are biased or have unverified sources would be very useful. 

The [Fakes News Challenge](http://www.fakenewschallenge.org) also serves as a very useful resource - corrdinating with the community of researchers already trying to tackle the problem and using the already annotated dataset will further help. [Snopes](http://www.snopes.com), [Politifact](http://www.politifact.com), and [FactCheck](http://www.factcheck.org) also serve as websites to identify trustworthy sources.

Other interesting sources of data is social media itself - twitter is often used, but it also usually just links to spurious sources, which we can use the above links to verify. [Reddit](https://www.reddit.com) is another very popular online forum, and has a huge community discussing [Fake News](https://www.reddit.com/search?q=fake+news). Crawling on reddit would also leave us with some interesting results. Kaggle is another very important resource - the competition, [Getting Real about Fake News](https://www.kaggle.com/mrisdal/fake-news) is another forum to not only discuss strategies with other data scientists but to compare our models performances - something which will be important in the later stages of our project when we are fine tuning our model.

[Google Scholar](https://scholar.google.fr/scholar?q=fake+news&btnG=&hl=en&as_sdt=0%2C5) offers us access to the exisiting scientific literature on Fake News, helping us with our research project. [Hoaxy](http://hoaxy.iuni.iu.edu) is a research project visualising networks of fake news.

As for training our model and linguistic features, some of the existing literature such as [Social Media and Fake News in the 2016 Election](https://web.stanford.edu/~gentzkow/research/fakenews.pdf) and [Classifying Fake News](http://www.conniefan.com/wp-content/uploads/2017/03/classifying-fake-news.pdf) helps us - ideas such as using sentiment (higher negative or positive sentiment - likely to be fake), writing quality (better writing quality - likely to be real), punctuation (again, similar to writing quality) are some of the many features we can consider choosing. The [project details](http://www.clips.uantwerpen.be/projects/gsoc-2017) in the CLiPS page also asks important questions, some of which have been answered in the papers above.

About the tools we can use, the work will largely be done in python - python boasts a really powerful variety of machine learning and deep learning tools. [Scikit-learn](http://scikit-learn.org/stable/), [Keras](https://keras.io), [Theano](http://deeplearning.net/software/theano/), [Tensorflow](https://www.tensorflow.org) are all libraries which can be used to create models for our problem, and I am comfortable with all of them. In particular, I believe the python library [spaCy](https://spacy.io) will be very useful - it has the fastest pre-processing toolkit available, and it's the deep learning integration is seamless. [Gensim](https://github.com/RaRe-Technologies/gensim), [NLTK](http://www.nltk.org) and [Pattern](http://www.clips.ua.ac.be/pages/pattern) will also serve as useful libraries during our project.

## Open Source Development Experience

I enjoy and regularly contribute to open source scientific computing libraries. I was previously selected to participate in Google Summer of Code 2016 with Gensim under the NumFOCUS umbrella, where I implemented Dynamic Topic Models. My [blog](https://summerofcode2017.wordpress.com/) details my experiences during summer of 2016.

I'm still a regular contributor for [Gensim](https://github.com/RaRe-Technologies/gensim/pulls/bhargavvader) - I have 29 pull requests merged, and actively help on the mailing list and issues. I have given talks at PyCon France 2016 and PyCon Slovakia 2017 about my experience with Gensim and GSoC 2016. I also contribute to [metric-learn](https://github.com/all-umass/metric-learn/pulls?q=is%3Apr+author%3Abhargavvader+is%3Aclosed), [Edward](https://github.com/blei-lab/edward/pulls/bhargavvader), [spaCy](https://github.com/explosion/spacy-notebooks/pulls?q=is%3Apr+author%3Abhargavvader+is%3Aclosed), and [pymc3](https://github.com/pymc-devs/pymc3/issues?q=is%3Aopen+mentions%3Abhargavvader). The links direct to my PRs/issues for the respective repos. My [GitHub profile](https://github.com/bhargavvader) has a more detailed summary of all my contributions. 


## Academic Experience

I am a student researcher at INRIA, France. I work with the MODAL (Models Of Data Analysis and Learning) team, where I work on Predictor Aggregation and Metric Learning problems. I'm finishing up my undergraduate education in Computer Science Engineering from BITS Pilani University, India. My [resume](https://drive.google.com/file/d/0By80y9AXd1WsRUJWTlFfeldITGc/view?usp=sharing) details my previous internships and research experiences, which are all in the field of Machine Learning, Data Science and Software Engineering - and will help in completing this project.

## Why this project? 

My interest in this project is for multiple reasons. While I majored in Computer Science at University, my minor was in Philosophy, Economics, Politics [PEP]. My coursework in the Social Sciences is what sparked my interest in Computational Social Science - solving or understanding social problems with the use of Computational tools. And Computational Linguistics and Natural Language Procsssing is a very powerful way to approach social problems, mainly because of the abundance of textual data and ways to mine them. The Fake News problem in particular is interesting because of how often we feel its affects, or notice it, or talk about it - with the ubiquity of social media, Fake News is everywhere! It directly affects our ruling governements and in some cases the policies - our ability to be informed voters is no longer easy. By making any progress in solving this problem - from gathering, labelling data and documentation to training a model - we are solving an important research and social problem.

A personal reason is my interest in pursuing a PhD in Computational Social Sciences - working with researchers from CLiPS, a top facility for Computational Linguistics would be a great research experience!

## What skills do I have suited for this project?

I have 3 years of experience in python, and have spent a considerable amount of time contributing to open source, particularly in python and machine learning. As I mentioned in the Open Source Development Experience section, I'm very comfortable with open source python NLP/CL tools. My background in the social sciences will also help in better analysing the context of the problem. 

My research experience in Machine Learning means I am familiar with the pipeline of solving such problems - finding and cleaning data, writing clean, reproducable code and keeping the process open source is as important as solving it. 

I have worked with visualisation tools such as D3.js before, and am very comfortable with matplotlib. This [link](https://github.com/bhargavvader/personal/tree/master/notebooks) contains all the Jupyter Notebooks I have made and contributed to.
I also enjoy writing (I have previously linked to my GSoC 2016 blog), and using Jupyter notebooks to explain concepts and ideas. 

If working in a team, I am comfortable in either working in the data collection, curation and cleaning, or in creating the classifier/model, and have experience in doing both. Having completed GSoC before, I understand the importance of clear communication and how to work and behave in an open source community.

## Schedule of Deliverables

### May 1th - May 28th, **Community Bonding Period**

- Meet with project mentors, decide which sources to use and which tools to use - at least for the beginning!
- Literature survey so everyone is comfortable with what has already been done, and discuss what hasn't!


### May 29th - June 9th

- Our first objective is to create a comprehensive dataset. We have discussed possible sources in detail in the Tehcnical Details section.
- The first two weeks could be spent on this task.

### June 12th - June 16th

- Cleaning and pre-processing our dataset is as important as collecting it!
- This week could be spent pre-processing and arranging our data, making it ready for training.

### June 19th - June 23th, **End of Phase 1**

- As phase 1 ends we now have our data ready. Documentation is key - making sure we let people know the sources of our data, and creating a Jupyter notebook to explain our collection and cleaning would make for an interesting blog post!
- We can start in setting up our model.


### June 26 - July 7th, **Begin of Phase 2**

- We now begin exploring possible models to train our data.
- A more complex model is not necessarily a better one - a simple Naive Bayes can give us excellent results if we choose the right features!

### July 10th - July 14th

- We are now midway through the project and should be seeing some results!
- In most machine learning problems, fine tuning and playing with parameters is half the trouble - we should be at this stage now.

### July 17th - July 21th, **End of Phase 2**

- A blog post detailing our progress would be appropriate now.
- Along with progress, it is important to clealry document the difficulties and problems faced - we are contributing to the exisiting scientific literature by doing this!

### July 24th - August 18th, **Begin of Phase 3**

- The last month of the project should be when we are coding less and less - visualisations, write-ups, infographics and blog posts should be the focus!
- Much like a trained sentiment model, a trained Fake News detector would be a very useful open source addition. 
- Even an imperfect machine would be useful to the coummnity, and we can always improve the state-of-the-art.
- Cleaning up what's left of the project, and making sure that it can be accessed again and worked on is a high priority.


### August 21st - August 29th, **Final Week**

- At this point we should have explored the Fake News project in great detail, and from many angles and perspectives.
- A research publication would be an ideal result - with regular blog posts and documentation, we should have enough material ready!

## Future Works

I would like to continue contributing to the research pursued by CLiPS - either by contributing to Pattern, or even considering a career as a researcher or student at CLiPS!

## Appendix

[Fakes News Challenge](http://www.fakenewschallenge.org)

[Media Bias Fact Check](https://mediabiasfactcheck.com)

[Fake News Checker](https://www.fakenewschecker.com)

[Social Media and Fake News in the 2016 Election](https://web.stanford.edu/~gentzkow/research/fakenews.pdf) 

[Classifying Fake News](http://www.conniefan.com/wp-content/uploads/2017/03/classifying-fake-news.pdf) 

