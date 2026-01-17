 Practice Using KodeKloud Labs

You can run all manifests in this repository using **KodeKloud’s free Kubernetes hands-on labs**, which provide a real, preconfigured Kubernetes cluster.

🔗 **KodeKloud Kubernetes Labs:**
[https://kode.wiki/kubernetes-labs](https://kode.wiki/kubernetes-labs)

## 🎥 Video Tutorial

For a guided walkthrough of Kubernetes basics and lab usage, refer to this video:

🎬 [https://youtu.be/XuSQU5Grv1g?si=ytzf-PvvWJ2qq2YO](https://youtu.be/XuSQU5Grv1g?si=ytzf-PvvWJ2qq2YO)

---

## 📂 What’s Inside This Repository

The repository contains Kubernetes YAML manifests that define:

* Application components (Pods / Deployments)
* Networking using Services (ClusterIP / NodePort)
* Supporting services like databases (e.g., Redis, PostgreSQL)

Each file represents a **declarative desired state** that Kubernetes uses to create and manage resources.

---

##  How to Use (Recommended Workflow)

### 1️⃣ Fork the Repository

Forking is recommended so you can:

* Practice safely
* Modify manifests freely
* Save your progress in your own GitHub account

### 2️⃣ Clone Your Fork in the Lab


git clone https://github.com/<your-username>/K8s-voting-app.git
cd K8s-voting-app

### 3️⃣ Apply the Manifests


kubectl apply -f .


### 4️⃣ Verify Resources

kubectl get pods
kubectl get services



##  Accessing the Application

* Use **NodePort** services and the node IP
* Or use **port-forwarding**:


kubectl port-forward svc/<service-name> 8080:80


Then open:


http://localhost:8080


---

## Learning Outcomes

By practicing with this repo, you will understand:

* How Kubernetes schedules and manages pods
* How services enable networking
* How declarative YAML drives application lifecycle
* How real clusters differ from local tools like Minikube

STAR THE REPO IF YOU LIKE THE WORKFLOW
