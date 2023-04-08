# Spinetta discography analysis
On this notebook we will explore the lyrics of the brilliant argentinian songwriter Luis Alberto Spinetta. Spinetta has an extensive catalog spanning decades, whethere part of a band or as solo artist. He was a very prolific songwriter, being able to use complex, poetic vocabulary to convey his ideas. 

![Spinetta](https://cdn.wallpapersafari.com/77/90/kqTyzC.jpg)

We will first make an exploratory analysis to identify opportunities of insight generation and ML modeling.

1. Authorship:

    - How many of Spinetta's songs were penned by himself?
        
        - Is it possible to identify which songs are his and which aren't?

            - Tool: binary classification with Tf-Idf.

1. Themes:

    - Which were the main themes of Spinetta's songs in general and by album?
    
        - Tool: bigrams and trigrams.

2. Sentiment analysis:

    - Which albums can be considered sad albums and which can be considered happy albums?

        - Tool: TBD

    - Did the albums get sadder or happier with time?
    
        - Tool: time series.

3. Complexity of vocabulary:

    - Which albums had the most variety of vocabulary?

        - Lexicon frequency.

    - Did vocabulary change with time? Did the albums become simpler or more complex in terms of vocabulary?

        - Tool: time series based on a metric of frequency.

  ## Source of data
  The data we will use is basically all lyrics from all his albums, in a string format. We would have to either webscrap it or obtain it in a file which can be read and persisted into a variable. We chose the latter, obtaining the lyrics through the GeniusAPI, from the genius.com website. It is a website where not only you can find lyrics of most artists available, but also fetch other relevant information. We will use their API to fetch lyrics themselves.
  
