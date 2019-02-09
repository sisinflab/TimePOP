# TimePOP

## Local Popularity and Time in top-N Recommendation

Items popularity is a strong signal in recommendation algorithms. It strongly affects collaborative filtering approaches and it has been proven to be a very good baseline in terms of results accuracy. As a matter of fact, even though we miss an actual personalization, global popularity of the items in a catalogue can be effectively used to recommend items to users. In this paper we introduce the idea of a _time-aware personalized popularity_ in recommender systems by considering both items popularity among neighbors and how it changes over time. Although the proposed approach results computationally light and exploits only implicit feedback, an experimental evaluation shows its highly competitive behavior, compared to state of the art model-based collaborative approaches, in terms of results accuracy.

Collaborative-Filtering (CF) algorithms, more than others, have gained a key-role among recommendation approaches and have been effectively implemented in commercial systems to help users in dealing with the information overload problem. Some of them also use additional information (hybrid approaches) to build a more precise user profile in order to serve a much more personalized list of items.
However, it is well known that all the algorithms based on a CF approach (either in their pure version or in a hybrid one) are affected by the so called _popularity bias_ meaning that  popular items tend to be recommended more frequently than those in the long tail. 
Initially considered as a shortcoming of collaborative filtering algorithms and then not useful to produce good recommendations, in some works items popularity has been intentionally penalized. Very interestingly, a recommendation algorithm purely based on most popular items, although it does not exploit any actual personalization, has been proven to be a strong baseline. Moreover, a popularity-based recommendation algorithm does not require a heavy computational effort as it just considers the occurrence of an item within the profiles of all the users in a system. More recently, popularity has been also considered as a natural aspect of recommendation that, by measuring the user tendency to diversification, can be exploited to balance the recommender optimization goals. The study of popularity in user tendencies is not completely new in the recommender systems field. Some interesting works explored these criteria for re-ranking purposes, and multiple goals optimization.
In the approach we present here, we change the global perspective of a most popular algorithm and we introduce a more fine-grained personalized version of popularity by assuming that it is conditioned by the items that a user _u_ already experienced _in the past_. To this extent, we look at a specific class of neighbors, that we name _Precursors_, defined as the users who already rated  the same items of _u_ in the past. This led us to the introduction of a time-aware analysis while computing a recommendation list for _u_. 

## Reference
If you publish research that uses TimePOP please use:
~~~
@inproceedings{Anelli2019Local,
  author    = {Vito Walter Anelli and
               Tommaso Di Noia and
               Eugenio Di Sciascio and
               Azzurra Ragone and
               Joseph Trotta},
  title     = {Local Popularity and Time in top-N Recommendation},
  booktitle = {Proceedings of the 41st European Conference on Information Retrieval, 14th - 18th April 2019, Cologne, Germany},
  year      = {2019}
}
~~~
The full paper describing the overall approach is available here [PDF](https://github.com/vitowalteranelli/TimePOP/blob/master/ECIR2019_paper_306.pdf)

## Credits
This algorithm has been developed by Vito Walter Anelli and Joseph Trotta while working at [SisInf Lab](http://sisinflab.poliba.it) under the supervision of Tommaso Di Noia.  

## Contacts

   Tommaso Di Noia, tommaso [dot] dinoia [at] poliba [dot] it  
   
   Vito Walter Anelli, vitowalter [dot] anelli [at] poliba [dot] it 
   
   Joseph Trotta, joseph [dot] trotta [at] poliba [dot] it 
