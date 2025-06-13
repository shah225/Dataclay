# 👨‍👩‍👧 Hello Family 

HelloFamily is a simple application that registers a list of people info into a persistent collection identified by an alias. Every time this application is executed, it first tries to load the collection by its alias, and if it does not exist the application creates it. Once the collection has been retrieved, or created, the given new person info is added to the collection and the whole set of people is displayed.


## 🏗 Project Structure

```

hello-family/
├── model/
│   └── family.py          # Contains the Person and Family classes
├── client.py              # Application that interacts with the Family object
├── docker-compose.yml     # Docker setup for dataClay environment
└── README.md              # Project documentation

```

## 📦 Requirements

- Docker
- docker-compose
- Python 3.8+ (for local testing if needed)
- dataClay (runs in Docker)

## 🚀 How to Run the Demo

1. Build and run the containers:
   ```bash
   docker-compose up --build
   ```

2. Open a new terminal and run the client script:
   ```bash
   docker exec -it dataclayclient bash
   python3 client.py
   ```

3. You will see log output showing how persons and families are created and persisted.

## 🔒 Security Extension 

We demonstrate a simple JWT-based security mechanism using decorators in a future version (e.g., `secure_Family.py`), simulating access control.



## 📚 References

- 🔗 [dataClay Documentation](https://docs.dataclay.org)
- 🔗 [JWT.io](https://jwt.io)
- 🔗 [Docker Compose Docs](https://docs.docker.com/compose/)

---

## 🧠 Author

Shahed Othman – [GitHub Profile](https://github.com/shah225)
