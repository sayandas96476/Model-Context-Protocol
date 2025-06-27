Reference Tutorial: https://www.youtube.com/watch?v=ASRCJK2aWk0

Reference Github: https://github.com/krishnaik06/MCPSERVERLangchain

## 🧠 Modular Context Protocol with FastMCP

This project demonstrates a **Modular Context Protocol (MCP)** system using the `fastmcp` module. It includes:

* 🧮 `mathserver.py` — a math tool using **stdio transport**
* 🌦️ `weather.py` — a dummy weather tool using **HTTP (streamable-http) transport**
* 🤖 `client.py` — a client script to query and interact with the above tools

---

### 🗂️ Components

| File            | Role                  | Transport                   | Description                                    |
| --------------- | --------------------- | --------------------------- | ---------------------------------------------- |
| `mathserver.py` | Tool (Math Server)    | `stdio`                     | Runs in the terminal, responds to math queries |
| `weather.py`    | Tool (Weather Server) | `http` or `streamable-http` | Exposes a static weather message via URL       |
| `client.py`     | MCP Client            | —                           | Sends queries to both tools as an MCP agent    |

---

### ▶️ How to Run

**1. Start the Tool Servers:**

```bash
# Terminal 1
python mathserver.py

# Terminal 2
python weather.py
```

**2. Start the Client:**

```bash
# Terminal 3
python client.py
```

Then enter your queries when prompted.

---

### 💬 Example Query in client.py

```text
What is 3 plus 5?
Tell me the weather in California.
```

---

Let me know if you'd like to auto-start the servers using a script or want badges, license, or requirements formatting too.
