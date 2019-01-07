# TimePOP
TimePop is a simple and efficient algorithm that combines the notion of personalized popularity and temporal aspects. 

The main assumption behind a “most popular” approach is that global popularity is a characteristic influencing all the users.
In the approach we introduce here, we change this perspective and we analyze a more fine grained personalized version of  popularity by assuming that it is conditioned by the items that a user u already experienced in the past. To this extent, we look at a specific class of neighbors, that we name Precursors, defined as the users who already rated the same items of u in the past.

## Credits
This algorithm has been developed by Vito Walter Anelli and Joseph Trotta while working at [SisInf Lab](http://sisinflab.poliba.it) under the supervision of Tommaso Di Noia.  

## Contacts

   Tommaso Di Noia, tommaso [dot] dinoia [at] poliba [dot] it  
   
   Vito Walter Anelli, vitowalter [dot] anelli [at] poliba [dot] it 
   
   Joseph Trotta, joseph [dot] trotta [at] poliba [dot] it 


## Usage:

 -b,--beta <arg>                  Beta value for temporal decay
 
 -N,--nItemsRecommended <arg>     Number of items recommended
 
 -rec,--recommender <arg>         Name of recommender
 
 -rf,--resultFile <arg>           Output result file with recommendations
 
 -rt,--referringTimestamp <arg>   Last rating timestamp in the training set
 
 -st,--startingTimestamp <arg>    first rating timestamp in the training set
 
 -tf,--trainfile <arg>            Training set path 

## Example

java -jar timepop.jar --recommender="TimePop" --trainfile="toys_amazon/trainingset.tsv" --nItemsRecommended="100" --resultFile="TimePop.tsv" --referringTimestamp="1377820800" 

## Reference

If you find these implementations useful for your research please cite:

> @article{DBLP:journals/corr/abs-1807-04204,   
>   author    = {Vito Walter Anelli and   
>                Joseph Trotta and   
>                Tommaso Di Noia and   
>                Eugenio Di Sciascio and   
>                Azzurra Ragone},   
>   title     = {Time and Local Popularity in top-N Recommendation},   
>   journal   = {CoRR},   
>   volume    = {abs/1807.04204},   
>   year      = {2018},   
>   url       = {http://arxiv.org/abs/1807.04204},   
>   archivePrefix = {arXiv},   
>   eprint    = {1807.04204},   
>   timestamp = {Mon, 23 Jul 2018 13:39:30 +0200},   
>   biburl    = {https://dblp.org/rec/bib/journals/corr/abs-1807-04204},   
>   bibsource = {dblp computer science bibliography, https://dblp.org}   
> }   
