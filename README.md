# Distributed Lock System in Python

This project implements a distributed lock management system in Python using modular architecture. It simulates resource locking via a client-server model, supporting multiple resource queries and controls.

## 📌 Project Objective

To design and implement a lock server system with a client interface, using network communication and modular code organization (stub, skeleton, pool).

## 🧱 Architecture

- **Server (`lock_server.py`)**: Main server managing resource locks.
- **Client (`lock_client.py`)**: Sends requests to the server.
- **Stub/Skeleton (`lock_stub.py`, `lock_skel.py`)**: Handle request abstraction and logic routing.
- **Pool Manager (`lock_pool.py`)**: Manages lockable resources.
- **Networking Utils (`net_client.py`, `sock_utils.py`)**: Low-level socket operations.

## 🔧 Technologies Used

- Python 3.x
- `socket` module
- Command-line interface

## 🚀 How to Run

1. Run the server:
```bash
python3 lock_server.py
```

2. In another terminal, run the client:
```bash
python3 lock_client.py
```

3. Use one of the following commands:

| Command   | Description                                    |
|-----------|------------------------------------------------|
| `LOCK`    | Lock a resource                                |
| `RELEASE` | Release a locked resource                      |
| `STATUS`  | Check if a resource is locked                  |
| `STATS`   | View number of times a resource was locked     |
| `YSTATS`  | View how many resources are currently locked   |
| `NSTATS`  | View how many resources are available          |
| `EXIT`    | Terminate client or server                     |

## 📄 Documentation

See `Enunciado.pdf` for assignment requirements and `README.txt` for usage instructions.

## 👩‍💻 Author

- João Nunes

## 📃 License

This project is for academic and educational use only.
