---
published: true
---

## Stable Matching

Stable Matching

In mathematicsLinks to an external site., economicsLinks to an external site., and computer scienceLinks to an external site., the stable marriage problem (also stable matching problem or SMP) is the problem of finding a stable matching between two equally sized sets of elements given an ordering of preferences for each element. A matchingLinks to an external site. is a bijectionLinks to an external site. from the elements of one set to the elements of the other set. A matching is not stable if:

There is an element A of the first matched set which prefers some given element B of the second matched set over the element to which A is already matched, and
B also prefers A over the element to which B is already matched.
In other words, a matching is stable when there does not exist any match (A, B) which both prefer each other to their current partner under the matching.

The stable marriage problem has been stated as follows:

Given n men and n women, where each person has ranked all members of the opposite sex in order of preference, marry the men and women together such that there are no two people of opposite sex who would both rather have each other than their current partners. When there are no such pairs of people, the set of marriages is deemed stable.

The existence of two classes that need to be paired with each other (heterosexual men and women in this example) distinguishes this problem from the stable roommates problemLinks to an external site..

 

Gale–Shapley algorithm
 

In mathematicsLinks to an external site., economicsLinks to an external site., and computer scienceLinks to an external site., the Gale–Shapley algorithm (also known as the deferred acceptance algorithm or propose-and-reject algorithm) is an algorithmLinks to an external site. for finding a solution to the stable matching problemLinks to an external site., named for David GaleLinks to an external site. and Lloyd ShapleyLinks to an external site. who had described it as solving both the college admission problem and the stable marriage problem. It takes polynomial timeLinks to an external site., and the time is linearLinks to an external site. in the size of the input to the algorithm. Depending on how it is used, it can find either the solution that is optimal for the participants on one side of the matching, or for the participants on the other side. It is a truthful mechanismLinks to an external site. from the point of view of the participants for whom it provides the optimal solution.

 

Initialize all men and women to free
while there exist a free man m who still has a woman w to propose to 

        {
            w = m's highest ranked such woman to whom he has not yet proposed
            if w is free
            (m, w) become engaged
            else some pair (m', w) already exists
            if w prefers m to m'
                (m, w) become engaged
                m' becomes free
            else
                (m', w) remain engaged    
        }
        


### The Stable Marriage Problem (Gale-Shapley Algorithm)

<iframe
    width="640"
    height="480"
    src="https://www.youtube.com/watch?v=A7xRZQAQU8s"
    frameborder="0"
    allow="autoplay; encrypted-media"
    allowfullscreen
>
</iframe>


### Stable Marriage Problem - Numberphile

<iframe
    width="640"
    height="480"
    src="https://youtu.be/Qcv1IqHWAzg"
    frameborder="0"
    allow="autoplay; encrypted-media"
    allowfullscreen
>
</iframe>