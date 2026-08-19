<div align="center">

# Round-Robin Load Balancer

*A lightweight reverse proxy for fair, fault-tolerant traffic distribution*

![Go](https://img.shields.io/badge/Go-1.20%2B-00ADD8?style=flat-square&logo=go&logoColor=white)
![Python](https://img.shields.io/badge/Python-3.9%2B-3776AB?style=flat-square&logo=python&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-lightgrey?style=flat-square)

</div>

---

# Round-Robin Load Balancer

A lightweight, high-performance load balancer that distributes HTTP traffic evenly across multiple backend servers. The load balancer is implemented in Go for speed and concurrency, with backend services built using Flask (Python), and traffic is routed through a reverse proxy using the round-robin scheduling algorithm.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Project Structure](#project-structure)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Roadmap](#roadmap)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

---

## Overview

This project implements a round-robin load balancer that distributes incoming HTTP requests fairly across a pool of backend servers. It pairs the concurrency and performance of Go with the simplicity of Flask-based Python services, offering a clean, practical reference for reverse proxying and load-balancing design.

## Features

- **Reverse Proxy** — forwards client requests to backend servers transparently
- **Round-Robin Scheduling** — distributes traffic evenly across all available servers
- **Flask & Go Integration** — Python's flexibility, paired with Go's performance
- **Scalability** — accommodates additional backend servers with minimal configuration
- **Fault Tolerance** — sustains traffic distribution when individual servers go down
- **Simple Deployment** — minimal setup to get running locally
## Overview

This project implements a round-robin load balancer designed to distribute incoming HTTP requests fairly across a pool of backend servers. It combines the performance and concurrency strengths of Go with the flexibility of Flask-based Python backends, making it a practical reference implementation for understanding reverse proxying and load-balancing concepts.

## Features

| Feature | Description |
|---|---|
| **Reverse Proxy** | Forwards client requests to backend servers transparently. |
| **Round-Robin Scheduling** | Distributes traffic evenly and fairly across all available servers. |
| **Flask & Go Integration** | Combines Python's flexibility with Go's performance and concurrency. |
| **Scalability** | Designed to accommodate additional backend servers with minimal configuration. |
| **Fault Tolerance** | Maintains traffic distribution even when individual servers become unavailable. |
| **Simple Deployment** | Minimal setup required to get the system running locally. |

## Project Structure

```
round-robin-load-balancer/
├── backend/            # Flask backend server implementation
├── loadbalancer/       # Go-based load balancer logic
├── config/             # Configuration files
├── main.go             # Load balancer entry point
├── app.py              # Flask application entry point
├── requirements.txt    # Python dependencies
└── README.md           # Project documentation
```

## Prerequisites

- [Go](https://go.dev/dl/) 1.20 or later
- [Python](https://www.python.org/downloads/) 3.9 or later
- pip (Python package manager)

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/subhradeepkundu270305/Round_Robin_Load_Balancer_in_GO.git
cd Round_Robin_Load_Balancer_in_GO
```

### 2. Set up and run the backend servers (Flask)

```bash
cd backend
python -m venv myenv
source myenv/bin/activate    # On Windows: myenv\Scripts\activate
pip install -r requirements.txt
python app.py
```

### 3. Run the load balancer (Go)

```bash
cd loadbalancer
go run main.go
```

## Usage

Once the backend servers and load balancer are running, send requests to the load balancer's endpoint:

```bash
curl http://localhost:8080/
```

Incoming requests are distributed evenly across all registered backend servers using the round-robin algorithm.

## Roadmap

- [ ] Add active health checks to automatically remove unresponsive servers
- [ ] Implement weighted round-robin for more granular load management
- [ ] Add HTTPS support
- [ ] Add configurable server pools via a config file

## Contributing

Contributions are welcome. If you'd like to improve this project:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes
4. Push to the branch and open a pull request

## License

This project is licensed under the [MIT License](LICENSE).

---

## Contact

<div align="center">

**Subhradeep Kundu**

[Email](mailto:subhradeepkundu27@gmail.com) · [GitHub](https://github.com/subhradeepkundu270305)

</div>

Contributions are welcome. If you'd like to improve this project:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes
4. Push to the branch and open a pull request

## License

This project is licensed under the [MIT License](LICENSE).

## Contact

**Subhradeep Kundu**
Email: subhradeepkundu27@gmail.com
GitHub: [@subhradeepkundu270305](https://github.com/subhradeepkundu270305)
