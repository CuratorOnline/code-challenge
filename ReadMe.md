## Garmentier Unattended Code
Welcome to the Garmentier Code Test.

Our goals for this take home code test is to get to know how you think through a problem. We are also looking to evaluate what you value when writing code and how that aligns with Garmentier engineering values.

You are free to use any language, tool or framework however be aware we favor the tools and technology we currently use or have mentioned and will be looking for someone to come up to speed quickly.

The engineering team at Garmentier believe in building maintainable code for our applications using industry best practices and will be looking for evidence you share the same beliefs in your solution.

As with all technology solutions and designs there are tradeoffs and concerns that arise and decisions needing to be made. We expect you to make these decision on your own. It would be helpful to provide a documentation of any assumption or decision made to help us understand your solution better. 

Time considerations, we understand that code solutions take personal time and would expect engineers to spend no more than a few hours solving these problems. As we work remotely personal time management is critical for people to be successful.  

The code test is one aspect of our review process, so feel free to submit what you achieved in the time you allocated. We are not looking for perfect just looking to better know you.

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
At Garmentier we deal with a number of sales that are generated from our platform. Through integrations we receive feeds of transactions that are converted and need to associate those identities in our system. To help our customers understand how they are performing we generate visualizations, views and reports based on this associated data that they can interact with.

You will need to create a webhook endpoint(s) that will be called with transaction data. This endpoint will need to process the transactions and associate them to known Company, Stylists and Clients. Information for Company, Stylists and Clients is provided as a json file.

You will also need to create an endpoint(s) (API) that can be used to query the associated transactional. This endpoint will be used for viewing individual transactions, reporting on Company, Stylist performance over a time frame.

Additional points for interactive UI or visualization of this data.

### Concerns
Due to the nature of integrations transaction partners do not provide common formats or consistent data. This means that not all transaction records provide granular identification to associate to all fields.

Also take into consideration that Garmentier is growing and adding new transaction partners frequently and we want to reduce the overhead of turning new partners on.

## Submission
When you have your final solution to all problems, please reply to the email that was sent to you with your solution as a .zip, .tar, or .tar.gz attachment. 

Do not include any binaries, only source code, as this might trigger spam filters or be rejected for size.

Please provide any accompanying documentation on how to build, run and interact (if possible) with you code.

## About Engineering at Garmentier
Engineering at Garmentier is not only about writing code – we are aiming to empower product teams who work collaboratively to conceptualize new features and bring them to life. We aim to build intuitive, user-friendly software using industry best practices and believe that delivering incrementally, using prototypes, and incorporating user feedback early, mitigate risk and help ensure success. We measure ourselves on our customer’s success, doing our best to embrace humility, diversity, and intentionality in how we make technical decisions.

Came across this problem by accident and interested in an engineering role at [Garmentier](http://www.garmentier.co). Send us an email with your resume to careers@garmentier.co
