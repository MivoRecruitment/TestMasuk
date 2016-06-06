# Capital To Mansion

In the Capital, Subaru found that his friend's (?) Mansion will soon be under attack of the Witch's familiar.  
However, being time-sliper, subaru isn't used to this world yet, thus, he doesn't know the fastest route to reach the mansion.  
Luckily, he has a simplified accurate map showing the path between the Capital, and the Mansion.  
However, Despite having that map, figuring the fastest route isn't simple because there could be  over 1000 junction between the Capital and the Mansion.  
His special ability, return by death, is especially useless here, because each time he dies, the map changes.  

However, there's a special rule, that will never be broken in any paralell universe, and that is:  
> There's always 3 route he can take, top, middle and bottom. And, at each junction, he can either switch route, or continue going forward.  

As he doesn't want to waste any time, Subaru need your help to find the shortest route, and the minimum distance between Capital to the Mansion.  

##### Input

- The first line is a single integer N (1 < N < 10000), the amount of track in a single route.
- The second line consist of N integer, (T1...Tn (50 <= Ti <= 199)) the distance between each junction in the top route.
- The third line consist of (N - 1) integer, (JT1...JTn (50 <= JTi <= 199))the distance between n-th junction at top route, with the n-th junction at the middle route.
- The fourth line consist of N integer, (M1...Mn (50 <= Mi <= 199) the distance between each junction in the middle route.
- The fifth line consist of (N - 1) integer, (JB1...JBn (50 <= JBi <= 199)) the distance between n-th junction at the middle route, with the n-th junction at the bottom route.
- The last line consist of N integer, (B1...Bn (50 <= Bi <= 199)) the distance between each junction in the bottom route.

##### Output:
The first line is a single integer, the minimum distance between the Capital and the Mansion.

The second line consist of first route he take(top/middle/bottom), spaces, and then the subsequent direction (v for go down, ^ for up, > for go forward, < for going backward) the path that Subaru had to choose

sample input:

    5
    50 60 199 50 50
    51 52 52 50
    160 51 60 50 199
    50 81 103 150
    153 103 71 100 150

sample output:

    362
    top v>>>^>

explanation:  
in the example above, the graph can be represented as below,

                50  --- 60  --- 199 --- 50  --- 50
              /      |       |       |       |     \
             /       51      52      52      50     \
            /        |       |       |       |       \
    Capital -- 160  --- 51  --- 60  ---  50 --- 199 --- Mansion
            \        |       |       |       |       /
             \       50      81     103     150     /
              \      |       |       |       |     /
                153 --- 103  --- 71 --- 100 --- 150

And the shortest distance can be achieved by:

- first take the top route (50)
- go downward (v) to middle route (51)
- go forward (>) in the middle route (51)
- go forward (>) in the middle route (60)
- go forward (>) in the middle route (50)
- go back upward (^) the top route (50)
- go forward (>) to reach the mansion (50).

(50 + 51 + 51 + 60 + 50 + 50 + 50) = 362

Find the minimum distance with [this dataset](dataset.txt).  
Submit your solution in your favorite programming language to recruitment-**#{minimum distance}** @mivo.com.  
e.g: recruitment-362@mivo.com.

Additionally, you might also want to include your:
- CV
- link to GitHub Account
- link to StackOverflow Account
- link to LinkedIn Account
