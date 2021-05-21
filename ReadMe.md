## Garmentier Unattended Code
Welcome to the Garmentier Code Test.

Our goals for this take home code test is to get to know how you think through a problem. We are also looking to evaluate what you value when writing code and how that aligns with Garmentier engineering values.

You are free to use any language, tool or framework however be aware we favor the tools and technology we currently use or have mentioned and will be looking for someone to come up to speed quickly.

The engineering team at Garmentier believe in building maintainable code for our applications using industry best practices and will be looking for evidence you share the same beliefs in your solution.

As with all technology solutions and designs there are tradeoffs and concerns that arise and decisions needing to be made. We expect you to make these decision on your own. It would be helpful to provide a documentation of any assumption or decision made to help us understand your solution better. 

Time considerations, we understand that code solutions take personal time and would expect engineers to spend no more than a few hours solving these problems. As we work remotely personal time management is critical for people to be successful.  

The code test is one aspect of our review process, so feel free to submit what you achieved in the time you allocated. Obviously, the seniority of the role you are applying sets expectations for your solution. Just know we are not looking for perfect just looking to know you.

To keep the recruitment process moving we would expect to receive a submission in a few days of sending out the invitation. Please let us know if you would need longer.

## Problem One - Pangram
The sentence "A quick brown fox jumps over the lazy dog" contains every single letter in the alphabet. Such sentences are called pangrams. 

You are to write a method getMissingLetters, which takes as input a string containing a sentence and returns all the letters not present at all in the sentence (i.e., the letters that prevent it from being a pangram). You should ignore the case of the letters in sentence, and your return should be all lower case letters, in alphabetical order. You should also ignore all non-alphabet characters as well as all non-US-ASCII characters.

### Concerns
Imagine that the method you write will be called many thousands of times in rapid succession on strings with length ranging from 0 to 50. Accordingly, you should try to write code that runs as quickly as possible. Also, imagine the case when the input string is quite large (e.g., tens of megabytes). See if you can develop an algorithm that handles this case efficiently while still running very quickly on smaller inputs.

### Examples
1. "A quick brown fox jumps over the lazy dog"
Returns: ""
2. "A slow yellow fox crawls under the proactive dog"
Returns: "bjkmqz"
3. "Lions, and tigers, and bears, oh my!"
Returns: "cfjkpquvwxz"
4. ""
Returns: "abcdefghijklmnopqrstuvwxyz"

## Problem Two - Transaction Accounting
At Garmentier we deal with a number of sales that are generated from our platform. Through integrations we receive feeds of transactions that have converted and need to be associated to identities within our system. This data is then used to generate visualizations, views and reports to better help Garmentier and our customers understand their business.

### Concerns
Garmentier integrates with Third Party providers which we have little control over. This means integrations may vary by:-
- Data formats (field names, data types etc)
- Data granularity (which identifiers are provided in a feed)
- Integration Types (Polling vs Notification, Event vs Batch)

Other considerations include that Garmentier is growing and continually adding new transaction partners, as well as company and clients. These means we are looking for a scalable system where:-
- overhead of turning on new partners is low
- ability to process and store an increasing number of transactions

### Deliverables
#### Design 
Taking into account the above concerns please present a design system to support them.

Ideally, outlining the tradeoffs you have considered and how you came to your decision. The level of detail is left up to you. Diagrams are a great medium to help build understanding.

#### POC Implementation
Provided in this repo is a couple example partner transaction data files along with Garmentier's company config. 

Please provide a code example of how you would process these data sets, associating it to different Garmentier identities, as well as normalizing the data for internal querying later. Please remember to take the considerations of growth and scale mentioned above.

Along with code please provide documentation on how to build and execute your solution. Implementation is left up to you this could be a script, API or application.

#### Data Considerations (Query and Reporting)
The combination of the two datasets provides a lot of opportunity for future product features. We would like to get your thoughts on what could be achieved with this data.

Please document the schema of the data you will be storing (ie. JSON scheme, Entity Diagram). Also provide some documentation on what you decided to keep and why?

Here are some other questions for you to consider around your design and solution:-
- What type of data storage would you use?
- How would you interact with this data?
- What question can be asked from data you have stored?
- What question do you think are valuable to ask and why?
- Do data considerations have any impact on your design or POC implementation?
- What further questions would you ask to help ensure your design stands the test of time?
- What other considerations should we take into account?

## Submission
When you have your final solution to all problems, please reply to the email that was sent to you with your solution as a .zip, .tar, or .tar.gz attachment. 

Do not include any binaries, only source code, as this might trigger spam filters or be rejected for size.

Please provide any accompanying documentation on how to build, run and interact (if possible) with your code.

## About Engineering at Garmentier
Engineering at Garmentier is not only about writing code – we are aiming to empower product teams who work collaboratively to conceptualize new features and bring them to life. We aim to build intuitive, user-friendly software using industry best practices and believe that delivering incrementally, using prototypes, and incorporating user feedback early, mitigate risk and help ensure success. We measure ourselves on our customer’s success, doing our best to embrace humility, diversity, and intentionality in how we make technical decisions.

Came across this problem by accident and interested in an engineering role at [Garmentier](http://www.garmentier.co)? Send us an email with your resume to careers@garmentier.co
