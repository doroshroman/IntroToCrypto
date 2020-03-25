## Cryptographic Hash Functions
### Hash function:
* takes any string as input
* fixed-size output (256 bits like Bitcoin)
* efficiently computable

### Security properties:
* collision-free
* hiding
* puzzle-friendly

![Collision-free](./collision_free.png)

It's possibly to find collisions because there are lots of input and much less outputs (Different inputs map to one output)

![Collision](./collision.png)

### Real world example
![Collision](./application.png)

![Collision](./hiding_problem.png)
<p><i> Problem here - easy to find x, because you   need to find hashes of two string and compare to hash of our function.</i></p>

So
![Collision](./hiding.png)

![Collision](./api.png)

![Collision](./third.png)
