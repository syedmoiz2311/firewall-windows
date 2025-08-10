# Task 4 – Setup and Use a Firewall on Windows  

## **Objective**  
Configure and test basic firewall rules to allow or block traffic using **Windows Defender Firewall**.  

---

## **Tools Used**  
- **Windows Defender Firewall with Advanced Security**  
- **Nmap (On Kali Linux)**  

---

## **Steps Performed**  

### **1. Open Windows Firewall**  
- Searched for `Windows Defender Firewall with Advanced Security`

---

### **2️. View Current Firewall Rules**  
- Click **Inbound Rules** (for incoming traffic).  

---

### **3️. Block Inbound Traffic on Port 23 (Telnet)**  
1. **Inbound Rules** → **New Rule…**  
2. Select **Port** → Next.  
3. Choose **TCP**, enter `23` in **Specific local ports** → Next.  
4. Select **Block the connection** → Next.  
5. Apply to **Domain, Private, Public** → Next.  
6. Name it `Block Telnet (Port 23)` → Finish.  

---

### **4️. Test the Rule**  
- Tried to connect to port 23 from Kali using nmap:

---

### **5. Remove the Test Rule**  
- Find `Block Telnet (Port 23)` in Inbound Rules → Right-click → **Delete**.  

---

## **Summary of Learning**  
- **Inbound rules** = control incoming connections.  
- **Outbound rules** = control outgoing connections.  
- Windows Firewall allows blocking or allowing traffic by **port, program, or IP**.  
- Blocking **Telnet (port 23)** improves security since Telnet is insecure and sends data in plain text.  

---

## **Screenshots Included**  
1. Viewing existing firewall rules.  
2. Creating **Block Telnet** rule.  
3. Testing blocked connection.  
4. Deleting the rule.  

---

## **Key Concepts**  
- **Firewall** = network security system that filters traffic.  
- **Stateful firewall** tracks active connections; **stateless** checks each packet individually.  
- **Ports** are communication endpoints (e.g., 23 = Telnet).  

---

**Prepared by:** *[Syed Moizuddin]*  
