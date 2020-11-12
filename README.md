# budgettracker

# Our goal

Take a working budget tracker and add PWA functionality so that the user can deposit or withdraw from their account while offline. When the user returns online, the app will then post those transactions.

## How this is done

Essentially the job here was to turn our app into a PWA (progressive web app)
We do this by creating a file (db.js) that tells the app how to behave when offline.

The DB does the following

* Creates a db for pending objects
* Checks if the app is online 
* If not online, creates a transaction on the pending db
* once back online, grabs all the pending transactions and posts them

