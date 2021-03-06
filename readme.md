## Bookatable's coding test

Welcome to Bookatable's coding test.

The solution comprises a message publishing mechanism (OffersPublisher), an event-queue mechanism (OffersQueue), 
a subscriber (OffersSubscriber) and a repository (OffersRepository) implementing a simple No-Sql DB solution.

We have already set up OffersPublisher to publish messages to OffersQueue, and OffersSubscriber to listen for messages from OffersQueue. 
What we would like of you is to implement the actual OffersSubscriber class, and ensure the following:

1. Using the OffersRepository class, check for existing records with the incoming message's Id. If none exist, use the Repository class to insert a new record in the DB comprising all the fields of the incoming message.
2. Using the OffersRepository class, check for existing records with the incoming message's Id. If one exists, use the Repository class to update the existing record.

You should not need to modify any of the interfaces, or any of the classes other than OffersSubscriber. However, you are welcome to modify parts of the code that are affected
by changes you introduce to the OffersSubscriber class (e.g. if you add a constructor to OffersSubscriber, you are welcome to change parts of the code
that instantiate OffersSubscriber).

You are also welcome to create your own interfaces and classes complementing your implementation should you feel that doing so leads to a cleaner, more scalable design.

### How to submit your solution to us:

1. Puublish the extracted solution as a new repo to your github/bitbucket account.
2. Create a branch off master, and start working on that branch. 
2. Try and work on the newly created repo as you normally would in a professional environment - name your commits as you normally would, push as often as you normally would. 
This will allow us to better understand your ways of working as a developer.
3. Once done, create a pull request towards master and send us the URL of that pull request. We will do our best to get back to you ASAP.

Thank you and good luck.