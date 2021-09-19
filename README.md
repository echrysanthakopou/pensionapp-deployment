# Pension App Deployment

Το αποθετήριο αυτό περέχει:

- Ένα docker-compose αρχείο που κάνει deploy την εφαρμογή σε docker περιβάλλον.
- Ένα ansible playbook το οποίο εγκαθιστά docker και docker-compose σε ένα μηχάνημα και εκτελούν το docker-compose αρχείο ώστε να γίνει το deployment.

## Εγκατάσταση

Για να εκτελέσετε το docker-compose αρχείο πρέπει να έχετε
docker και docker-compose εγκατεστημένα. Έπειτα εκτελέστε:

```bash
docker-compose up -d
```

Για να εκτέλεσε το ansible script πρέπει να έχετε την ansible 
καθώς και το ansible-galaxy εγκατεστημένα. Εκτελέστε τις παρακάτω εντολές:

```bash
ansible-galaxy install geerlingguy.docker
ansible-playbook deploy.yml
```


