# Round Robin Load Balancer

## 🚀 Overview
This project is a **Round Robin Load Balancer** that efficiently distributes **HTTP traffic** across multiple backend servers. It uses **Flask (Python) and Go (Golang)** for a scalable and high-performance solution. Additionally, it implements a **Reverse Proxy** to manage client requests seamlessly.

## 🛠️ Features
- **Reverse Proxy Implementation** – Acts as an intermediary to forward client requests to backend servers.
- **Round Robin Scheduling** – Ensures fair and even distribution of traffic.
- **Flask & Go Integration** – Combines Python’s flexibility with Go’s speed.
- **Scalability** – Easily handles growing traffic and backend servers.
- **Fault Tolerance** – Ensures smooth traffic distribution even if some servers go down.
- **Easy Deployment** – Simple setup to get started quickly.

## 📁 Project Structure
```
/round-robin-load-balancer
│── backend/              # Backend server implementation (Flask)
│── loadbalancer/         # Load balancer logic (Go)
│── config/               # Configuration files
│── README.md             # Project documentation
│── requirements.txt      # Dependencies for Flask backend
│── main.go               # Go-based load balancer implementation
│── app.py                # Flask app (if applicable)
```

## 🔧 Installation & Setup
### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/round-robin-load-balancer.git
cd round-robin-load-balancer
```

### 2️⃣ Setup & Run Backend Servers (Flask)
```bash
cd backend
python -m venv myenv
source myenv/bin/activate  # On Windows use: myenv\Scripts\activate
pip install -r requirements.txt
python app.py
```

### 3️⃣ Run the Load Balancer (Go)
```bash
cd loadbalancer
go run main.go
```

## 🚀 Usage
Once both the backend servers and the load balancer are running, send HTTP requests to the load balancer:
```bash
curl http://localhost:8080/
```
The requests will be evenly distributed across backend servers using the **Round Robin algorithm**.

## 📌 Future Enhancements
- Implement **Health Checks** to remove unresponsive servers dynamically.
- Add **Weighted Round Robin** for better load management.
- Support for **HTTPS** traffic.

## 📝 License
This project is open-source and available under the **MIT License**.

---
🔗 **Connect with Me:** subhradeepkundu27@gmail.com
