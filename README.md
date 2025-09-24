Encrypted Chat App (Python / Socket)

A simple chat application using Python sockets, with optional message encryption using cryptography.fernet.

Setup:

1. Clone the repository or download the files.

2. Create and activate a Python virtual environment:
   - python3 -m venv venv
   - source venv/bin/activate   (for macOS/Linux)

3. Install dependencies:
   - pip install -r requirements.txt

Run the Server:

- Run server.py to start the server.
- The server listens on port 5555.

Run the Client:

- Open a new terminal for each client.
- Run client.py to connect to the server.
- Messages typed in one client will appear in all connected clients.

Optional Encryption (Fernet):

1. Generate a key (once):
   - python3 -c "from cryptography.fernet import Fernet; open('secret.key','wb').write(Fernet.generate_key())"
2. Keep secret.key private; do not commit it to GitHub.

Notes:

- .gitignore excludes virtual environment files, compiled Python files, and secret keys.
- Tested on macOS/Linux.
