# 🚀 Day 2/90 — Networking Fundamentals

Welcome back to my **90 Days of DevOps** journey! On Day 1, I covered the basics of DevOps — what it is, why it matters, and the tools involved. Today, I stepped back to build a foundation that every DevOps engineer needs: **Networking**.

You can't manage servers, containers, or cloud infrastructure if you don't understand how machines actually talk to each other. So Day 2 was all about "Networking In One Shot" — here's what I learned. 👇

---

## 🌐 1. How Does the Internet Work?

At its core, the internet is a massive network of interconnected devices that communicate using a common set of rules (protocols). When you open a website:

1. Your browser sends a request to a **DNS server** to resolve the domain name into an IP address.
2. That request travels through your **ISP**, across routers, and eventually reaches the destination **server**.
3. The server processes the request and sends back a response, which your browser renders as a webpage.

It's a chain of small, well-defined handoffs — and understanding each link makes debugging real-world infrastructure issues far easier.

## 📚 2. OSI Model & TCP/IP Model

The **OSI Model** breaks network communication into 7 layers:

| Layer | Name | Example |
|---|---|---|
| 7 | Application | HTTP, DNS |
| 6 | Presentation | Encryption, formatting |
| 5 | Session | Session management |
| 4 | Transport | TCP, UDP |
| 3 | Network | IP, routing |
| 2 | Data Link | MAC addresses, switches |
| 1 | Physical | Cables, signals |

The **TCP/IP Model** is the practical, simplified version actually used on the internet, with 4 layers: **Application, Transport, Internet, and Network Access.**

Knowing these models helps pinpoint *where* a problem lives — is it a DNS issue (Application layer) or a cabling issue (Physical layer)?

## 🔢 3. IP Address & MAC Address

- **IP Address** — a logical address assigned to a device on a network (e.g., `192.168.1.10`). It can change and is used for routing data across networks.
- **MAC Address** — a physical, hardware-burned address unique to a network interface card (e.g., `00:1A:2B:3C:4D:5E`). It never changes and is used for communication within a local network.

**Analogy:** IP address = your home address (changes if you move). MAC address = your fingerprint (permanent).

## 🔀 4. Routers & Switches

- **Switch** — connects devices *within* the same network (LAN) and forwards data using MAC addresses.
- **Router** — connects *different* networks together (e.g., your home network to the internet) and forwards data using IP addresses.

Simple way to remember it: **switches connect devices, routers connect networks.**

## 🔥 5. Firewall, Ports & Protocols

- **Firewall** — a security layer that monitors and controls incoming/outgoing traffic based on defined rules, protecting a network from unauthorized access.
- **Ports** — logical endpoints that let a single device run multiple network services (e.g., `80` for HTTP, `443` for HTTPS, `22` for SSH).
- **Protocols** — the agreed-upon rules for communication (e.g., `TCP`, `UDP`, `HTTP`, `FTP`).

This is where DevOps really connects to networking — configuring security groups, opening/closing ports, and choosing the right protocol are everyday tasks in cloud and server management.

## 🖥️ 6. Client-Server Architecture

A **client** requests resources or services, and a **server** provides them. This model powers almost everything we use daily — websites, APIs, databases.

```
Client  --- request --->  Server
Client  <--- response ---  Server
```

Understanding this flow is essential before diving into load balancers, reverse proxies, and scaling strategies later in this challenge.

---

## 💡 Key Takeaway

Networking isn't just theory — it's the backbone of everything a DevOps engineer touches: cloud VPCs, Kubernetes networking, CI/CD pipelines talking to remote servers, container-to-container communication. Getting these fundamentals right on Day 2 sets up everything that follows.

## 📅 What's Next

Day 3 will build on this by diving deeper into practical networking tools and concepts used in real DevOps workflows.

---

*Following along? I'm documenting all 90 days here on GitHub and on LinkedIn. Feedback and suggestions are always welcome!*

`#DevOps #90DaysOfDevOps #Networking #LearningInPublic`
