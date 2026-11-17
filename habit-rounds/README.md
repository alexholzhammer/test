# Habit Rounds

A weekly habit challenge for five friends (Alex, Ali, Keela, Heather and Sully).
Each round runs Monday to Sunday. Everyone picks up to 5 habits, either
"do it X days a week" or "count and stay under a weekly max", and the
highest share of targets hit wins the round.

- Live app: https://habit-rounds-crew.web.app
- `public/index.html` is the whole app (plain HTML/JS, Firebase SDK from the CDN).
- Data lives in Cloud Firestore (`crew/players`, `habits/*`) in the
  `habit-rounds-crew` Firebase project. `firestore.rules` allows anyone with
  the link to read and write, and only checks the shape of the data.

## Deploy

```sh
cd habit-rounds
firebase deploy --only firestore,hosting
```
