# BBS with Chatroom System



A simple BBS with Chatroom System.

## Usage



```bash
# Start the server
./server [port]

# Start the client
./client [IP address] [port]
```

## Functions



### User Information

| Function                                 | Description                                 |
|:---------------------------------------- |:------------------------------------------- |
| `register <username> <email> <password>` | Register with username, email and password. |
| `login <username> <password>`            | Login with username and password.           |
| `logout`                                 | Logout.                                     |
| `whoami`                                 | Show username.                              |
| `list-user`                              | List all users in BBS.                      |
| `exit`                                   | Close connection.                           |

### Boards and Posts

| Function                                                       | Description                                          |
|:-------------------------------------------------------------- |:---------------------------------------------------- |
| `create-board <name>`                                          | Create a board.                                      |
| `create-post <board-name> --title <title> --content <content>` | Create a post.                                       |
| `list-board`                                                   | List all boards in BBS.                              |
| `list-post <board-name>`                                       | List all posts in a board.                           |
| `read <post-S/N>`                                              | Show the post which S/N is <post-S/N>.               |
| `delete-post <post-S/N>`                                       | Delete the post which S/N is <post-S/N>.             |
| `update-post <post-S/N> --title/content <new>`                 | Update the post which S/N is <post-S/N>.             |
| `comment <post-S/N> <comment>`                                 | Leave a comment at the post which S/N is <post-S/N>. |

### Chat Room

| Function                        | Description                                                      |
|:------------------------------- |:---------------------------------------------------------------- |
| `create-chatroom <port>`        | Create a chatroom which is named in the client-side.             |
| `list-chatroom`                 | List all Chatroom name and chatroom status (open or close).      |
| `join-chatroom <chatroom_name>` | Join a chatroom server.                                          |
| `attach`                        | Attach the chatroom. (The instruction is for the chatroom owner) |
| `restart-chatroom`              | Restart the chatroom, when the chatroom is closed.               |

### In Chatroom

| Function         | Description                                                                                    |
|:---------------- |:---------------------------------------------------------------------------------------------- |
| `leave-chatroom` | Leave chatroom.                                                                                |
| `detach`         | Detach the chatroom but do not close the chatroom. (The instruction is for the chatroom owner) |
