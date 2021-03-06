# assignment2-gundeti
# Madhupriya Gundeti
###### Melbourne
It has various restaurants which belongs to different nations but it is pretty expensive.<br>It has kind of varieties which you won't find anywhere else.
**kansas city**
***
## Directions to Taco Bell
1. Nearest airport to tacobel is Tullamarine Airport.
2. After getting  out of airport take Melbourne Dr to Tullamarine Fwy/M2 and continue to Melbourne Dr for about 10 miles.
3. Continue on M2 to Southbank and then take Exit 2 from M2 and drive for 15kms.
4. Merge onto Kings Way/National Route Alt 1 after driving 20kms, you can see Taco Bell towards your right.

### Menu:
* **Fan Favourites:**
    * Grilled Stuft Burrito
    * California Burrito
    * Crunch wrap Supreme
    * Double Taco Supreme
* **Specialties:**
    * Cheesy Double Decker Taco
    * Burrito Bowl
    * Stacked Chips Supreme
    * Stacked Nachos Supreme
* **Snackaritos:**
    * Cheesy swirl
    * Crunchy Taco
    * Mini Chicken Quesadilla
* **Desserts:**
    * Churros
    * Chocodilla
* **Drinks:**
    * Phoenix Lemon Lime Bitters
    * Phoenix Traditional Lemonade
    * Lipton Lemon Iced Tea
    * Ice Break Iced Coffee
    * Pepsi Max
    * Pepsi

**[Add](AboutMe.md)**

***
### Activities

It has three columns with activity name, Location where the activities are going to happen <br> Third column is the price that someone can invest on the equipment.

|    Name    |    Location    |    Amount    |
|    ----    |    --------    |    ------    |
|  Kabaddi   |   Hyderabad    |    $200      |
|  Football  |   Melbourne    |    $600      |
| Basketball |   Sydney       |    $700      |
| Cricket    |   Mumbai       |    $500      |

***
### Quotes
>"All you need in this life is ignorance and confidence; then success is sure."   -*Mark Twain*

>"I don't go by the rule book…I lead from the heart, not the head."        -*Princess Diana*

***
### Code Fencing
>0-1 BFS is a code to search tree data structure for a node that satisfies a property. Its starts at the tree root and travels all nodes at present depth to nodes at next depth level. Extra memory(queue) is required to keep track of all child nodes.
<https://en.wikipedia.org/wiki/Breadth-first_search>
```
d.assign(n, INF);
d[s] = 0;
set<pair<int, int>> q;
q.insert({0, s});
while (!q.empty()) {
    int v = q.begin()->second;
    q.erase(q.begin());

    for (auto edge : adj[v]) {
        int u = edge.first;
        int w = edge.second;

        if (d[v] + w < d[u]) {
            q.erase({d[u], u});
            d[u] = d[v] + w;
            q.insert({d[u], u});
        }
    }
}
```
<https://cp-algorithms.com/graph/01_bfs.html>