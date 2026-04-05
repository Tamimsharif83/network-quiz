# VLSM (Variable Length Subnet Mask) MCQ Quiz

---

## EASY LEVEL

### Q1: What does VLSM stand for?
A) Virtual Local Subnet Mask
B) Variable Length Subnet Mask
C) Very Large Subnet Manager
D) Virtual Layer Subnet Module

**Answer: B**

---

### Q2: What is the main advantage of VLSM?
A) Faster routing
B) More secure networks
C) Efficient use of IP address space
D) Easier DNS resolution

**Answer: C**

---

### Q3: Which routing protocol DOES NOT support VLSM?
A) OSPF
B) RIPv2
C) RIPv1
D) EIGRP

**Answer: C**

---

### Q4: In VLSM, can different subnets have different subnet masks?
A) No, all must be the same
B) Yes, each subnet can have its own mask
C) Only two different masks allowed
D) Only in private networks

**Answer: B**

---

### Q5: What subnet mask would you use for a subnet needing 30 hosts?
A) /25
B) /26
C) /27
D) /28

**Answer: B** (provides 62 usable hosts)

---

### Q6: How many usable host addresses are available in /29?
A) 4
B) 6
C) 8
D) 10

**Answer: B** (8 total - 2 reserved = 6 usable)

---

### Q7: What is the network address of 192.168.1.130/25?
A) 192.168.1.0
B) 192.168.1.128
C) 192.168.1.129
D) 192.168.1.255

**Answer: B**

---

### Q8: In VLSM, which step should be done first?
A) Assign IP addresses
B) Create subnets
C) Sort requirements by number of hosts (descending)
D) Calculate broadcast addresses

**Answer: C**

---

### Q9: What does a /32 subnet mask represent?
A) A network
B) A broadcast address
C) A single host
D) An entire Class C network

**Answer: C**

---

### Q10: Which class of IP address is typically used for VLSM subnetting exercises?
A) Class A
B) Class B
C) Class C
D) Any of the above

**Answer: D**

---

## MEDIUM LEVEL

### Q11: You have 192.168.0.0/22 and need to create subnets for:
- Subnet A: 250 hosts
- Subnet B: 100 hosts
- Subnet C: 50 hosts

What should be the subnet mask for Subnet A?
A) /24
B) /25
C) /26
D) /23

**Answer: A** (/24 provides 254 hosts)

---

### Q12: Given 10.0.0.0/16, if you create a /24 subnet starting at 10.0.0.0, what is the next available network?
A) 10.0.1.0/24
B) 10.0.2.0/24
C) 10.0.0.256/24
D) 10.1.0.0/24

**Answer: A**

---

### Q13: You need to subnet 172.16.0.0/12 for different departments. What is the maximum number of /24 subnets you can create?
A) 256
B) 1024
C) 4096
D) 16

**Answer: C** (4096 = 2^12 / 2^8)

---

### Q14: In VLSM, the broadcast address of one subnet can be:
A) The network address of the next subnet
B) Any address in the next subnet
C) Always one less than the next network address
D) Shared with the next subnet

**Answer: C**

---

### Q15: What is the network address for host 192.168.10.201/27?
A) 192.168.10.192
B) 192.168.10.200
C) 192.168.10.128
D) 192.168.10.0

**Answer: A** (/27 = 255.255.255.224, networks at 0, 32, 64, 96, 128, 160, 192...)

---

### Q16: You have 203.0.113.0/24 and need three subnets with 100, 60, and 40 hosts respectively. What mask would you assign to the 60-host subnet?
A) /25
B) /26
C) /27
D) /28

**Answer: B** (/26 = 62 hosts)

---

### Q17: In the network 10.1.1.0/26, what is the broadcast address?
A) 10.1.1.63
B) 10.1.1.64
C) 10.1.1.127
D) 10.1.1.255

**Answer: A**

---

### Q18: VLSM differs from fixed-length subnetting in that:
A) VLSM uses only private addresses
B) VLSM allows different subnet sizes within the same network
C) VLSM is only for IPv6
D) VLSM eliminates the need for routing

**Answer: B**

---

### Q19: Calculate valid host range for 10.20.0.0/23:
A) 10.20.0.1 - 10.20.0.254
B) 10.20.0.1 - 10.20.1.254
C) 10.20.0.0 - 10.20.1.255
D) 10.20.1.0 - 10.20.1.255

**Answer: B**

---

### Q20: When subnetting 172.20.0.0/16 with VLSM, if the first subnet is /27, how many total networks of that size could theoretically exist?
A) 256
B) 512
C) 2048
D) 65536

**Answer: C** (2^16 / 2^5 = 2048)

---

## HARD LEVEL

### Q21: You must subnet 192.168.0.0/22 for the following requirements (in order of size):
- Department A: 200 hosts
- Department B: 100 hosts
- Department C: 50 hosts
- Department D: 20 hosts
- Department E: 10 hosts

What are the correct subnet masks? (Matching left to right)
A) /24, /25, /26, /27, /28
B) /23, /24, /25, /26, /27
C) /24, /24, /25, /26, /27
D) /25, /25, /26, /27, /28

**Answer: A**

---

### Q22: For 10.0.0.0/16 with VLSM allocation of /24, /24, /25, /25, /26, /26, /26, /26 - what is the network address of the second /26 subnet?
A) 10.0.2.128
B) 10.0.2.192
C) 10.0.3.0
D) 10.0.3.64

**Answer: B** (After two /24s and two /25s: 10.0.0.0/24, 10.0.1.0/24, 10.0.2.0/25, 10.0.2.128/25, 10.0.3.0/26, 10.0.3.64/26, 10.0.3.128/26...)

---

### Q23: Which of the following VLSM designs is MOST efficient for these requirements?
- 5 subnets of 50 hosts each
- 10 subnets of 10 hosts each
- 3 subnets of 30 hosts each

A) All /25
B) /25 for large, /28 for 10-host, /26 for 30-host
C) /26 for 50-host, /28 for 10-host, /27 for 30-host
D) Custom VLSM allocation based on requirements

**Answer: D**

---

### Q24: In VLSM, what is a "supernet" and when would you use it?
A) A backup network
B) Combining multiple networks with route aggregation
C) A network with subnets only
D) An encrypted network

**Answer: B**

---

### Q25: Given the following VLSM plan for 172.16.0.0/16:
- Network 1: 172.16.0.0/25 (126 hosts)
- Network 2: 172.16.0.128/26 (62 hosts)
- Network 3: 172.16.0.192/26 (62 hosts)
- Network 4: 172.16.1.0/27 (30 hosts)

What is the next available usable network block?
A) 172.16.1.32/27
B) 172.16.1.64/27
C) 172.16.2.0/24
D) 172.16.1.32/26

**Answer: A**

---

### Q26: A network admin assigned 10.0.0.0/24, 10.0.1.0/24, and 10.0.2.0/25 to three departments. Later, they need to summarize these routes. What is the most specific aggregate address?
A) 10.0.0.0/23
B) 10.0.0.0/22
C) 10.0.0.0/24
D) 10.0.0.0/25

**Answer: B** (10.0.0.0/22 covers 10.0.0.0 to 10.0.3.255)

---

### Q27: You're designing a network with VLSM where you have 192.168.0.0/21. Requirements are:
- Site A: 300 hosts
- Site B: 150 hosts
- Site C: 75 hosts
- Site D: 35 hosts
- Site E: 20 hosts

What is the correct assignment pattern?
A) /22, /23, /24, /25, /26
B) /23, /24, /25, /26, /27
C) /22, /24, /25, /26, /27
D) /23, /24, /24, /26, /27

**Answer: B**

---

### Q28: In a VLSM-enabled network, why is route aggregation important?
A) To increase bandwidth
B) To reduce routing table size and improve lookup efficiency
C) To prevent subnetting
D) To eliminate routing protocols

**Answer: B**

---

### Q29: You have 203.0.113.0/24 and must assign VLSM subnets. You created:
- 203.0.113.0/26
- 203.0.113.64/26
- 203.0.113.128/25

How many host addresses are wasted (Class D broadcast addresses not usable)?
A) 1
B) 2
C) 3
D) 4

**Answer: C** (One for each network's broadcast address)

---

### Q30: A company uses 10.0.0.0/8 with VLSM. They need the supernet that covers subnets 10.1.0.0 to 10.3.255.255. What is this supernet?
A) 10.0.0.0/14
B) 10.1.0.0/16
C) 10.0.0.0/16
D) 10.1.0.0/14

**Answer: A**

---

### Q31: Analyze this VLSM allocation error:
Network: 172.20.0.0/22
- Subnet 1: 172.20.0.0/24 (for 250 hosts) ✓
- Subnet 2: 172.20.1.0/25 (for 100 hosts) ✓
- Subnet 3: 172.20.1.128/26 (for 50 hosts) ✓

What is wrong?
A) No overlap, but inefficient
B) 172.20.1.0/25 overlaps with the parent network incorrectly
C) Actually correct - all are properly allocated
D) The subnet masks are wrong

**Answer: C** (This is actually correct allocation)

---

### Q32: For QoS and load balancing across 192.168.100.0/24, you assign VLSM subnets to different services:
- VoIP: /28 (14 hosts)
- Video: /26 (62 hosts)
- Data: /25 (126 hosts)

How many networks total can you create with these masks from the /24?
A) 3-4 combinations
B) 6-8 combinations
C) 12+ combinations
D) Unlimited - depends on arrangement

**Answer: D** (The parent /24 can accommodate multiple combinations of these subnets depending on allocation strategy)

---

### Q33: In an ISP environment using VLSM, a provider has 203.0.112.0/21 to allocate to customers. If they allocate:
- Customer A: 203.0.112.0/24
- Customer B: 203.0.113.0/25
- Customer C: 203.0.113.128/26

How much address space remains available?
A) 127 addresses
B) 255 addresses
C) 384 addresses
D) 512 addresses

**Answer: D** (Remaining: 203.0.114.0/23 + 203.0.116.0/22 = 512 addresses)

---

### Q34: When implementing VLSM with dynamic routing protocols, which aspect is CRITICAL?
A) All routers must support classless routing
B) Routing protocol must support CIDR notation
C) All routers must understand variable-length subnets
D) All of the above

**Answer: D**

---

### Q35: You're troubleshooting a VLSM network where 192.168.5.100/27 cannot communicate with 192.168.5.130/27. Why?
A) Different subnets despite close IP addresses
B) Broadcast domains are separate
C) Both reasons above
D) They should be able to communicate

**Answer: C** (100/27 = 192.168.5.96-127, 130/27 = 192.168.5.128-159 - different networks)

---

### Q36: For a multi-datacenter network using 10.0.0.0/8 with VLSM, what is the aggregate route for:
- DC1: 10.1.0.0/16
- DC2: 10.2.0.0/16
- DC3: 10.4.0.0/16
- DC4: 10.8.0.0/16
A) 10.0.0.0/8
B) 10.0.0.0/13
C) 10.0.0.0/9
D) Cannot be aggregated

**Answer: C**

---

### Q37: A network uses 172.16.0.0/16 with this VLSM scheme:
- 172.16.0.0/25 through 172.16.3.224/25 (64 subnets)
- 172.16.4.0/26 through 172.16.7.252/26 (256 subnets)

Why is this scheme problematic?
A) Too many subnets created
B) Overlapping addresses
C) It's actually efficient
D) Not enough addresses for /26 subnets

**Answer: B** (The ranges overlap - 172.16.4.0/26 falls within the /25 range)

---

### Q38: For convergence-sensitive networks, VLSM implementation should prioritize:
A) Maximum number of subnets
B) Hierarchical addressing and route summarization
C) Fixed-size subnets
D) Avoiding aggregation

**Answer: B**

---

### Q39: Calculate the number of usable hosts in this VLSM-designed network:
Parent: 10.100.0.0/22 (1022 usable)
Subnets: /24 (254), /25 (126), /25 (126)

Total usable after VLSM:
A) 506
B) 508
C) 1022
D) 512

**Answer: A** (254 + 126 + 126 = 506)

---

### Q40: In VLSM design for a ISP network, which routing protocol would you NOT recommend?
A) BGPv4
B) RIPv1
C) OSPF
D) IS-IS

**Answer: B** (RIPv1 doesn't support VLSM or CIDR)

---

## ANSWER KEY SUMMARY

| Difficulty | Easy (Q1-10) | Medium (Q11-20) | Hard (Q21-40) |
|-----------|-------------|----------------|--------------|
| Correct Answers | B,C,C,B,B,B,B,C,C,D | A,A,C,C,A,B,A,B,B,C | A,B,D,B,A,B,B,B,C,A |
| Key Topics | Basics, Protocols | Calculation, Allocation | Aggregation, Design, Troubleshooting |

---

## VLSM QUICK REFERENCE

### Subnet Mask Reference:
| CIDR | Dotted Decimal | Hosts | Networks per /8 |
|-----|----------------|-------|-----------------|
| /24 | 255.255.255.0 | 254 | 256 |
| /25 | 255.255.255.128 | 126 | 512 |
| /26 | 255.255.255.192 | 62 | 1024 |
| /27 | 255.255.255.224 | 30 | 2048 |
| /28 | 255.255.255.240 | 14 | 4096 |
| /29 | 255.255.255.248 | 6 | 8192 |
| /30 | 255.255.255.252 | 2 | 16384 |

### VLSM Steps:
1. Sort requirements descending by host count
2. Assign smallest possible mask for each requirement
3. Allocate subnets sequentially
4. Verify no overlaps
5. Implement route aggregation where possible

