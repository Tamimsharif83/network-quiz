# Static IP Configuration MCQ Quiz

---

## EASY LEVEL

### Q1: What is a Static IP address?
A) An IP address that changes every time you connect
B) An IP address that is manually assigned and doesn't change
C) An IP address assigned by DHCP
D) An IP address only used for servers

**Answer: B**

---

### Q2: In Cisco CLI, which command is used to configure a static IP on an interface?
A) `ip address 192.168.1.1`
B) `ip address 192.168.1.1 255.255.255.0`
C) `address 192.168.1.1 255.255.255.0`
D) `static ip 192.168.1.1`

**Answer: B**

---

### Q3: What does the subnet mask 255.255.255.0 represent?
A) /8
B) /16
C) /24
D) /32

**Answer: C**

---

### Q4: Which command enables an interface in Cisco?
A) `interface up`
B) `no shutdown`
C) `enable`
D) `interface enable`

**Answer: B**

---

### Q5: How do you configure a loopback interface with IP 10.0.0.1?
A) Enter interface loopack0, then configure IP
B) Enter interface loopback0, then configure IP
C) Use `loopback 10.0.0.1`
D) Both B and part of this answer

**Answer: B**

---

### Q6: What does the command `ip address DHCP` do?
A) Assigns a static IP
B) Enables the interface
C) Configures the interface to use DHCP
D) Disables DHCP

**Answer: C**

---

### Q7: To view all configured IP addresses on a router, which command is used?
A) `show ip address`
B) `show interface ip`
C) `show ip interface brief`
D) `show addresses`

**Answer: C**

---

### Q8: What is the default gateway in network 192.168.1.0/24?
A) 192.168.1.0
B) 192.168.1.1
C) 192.168.1.254
D) 192.168.1.255

**Answer: B** (typically, though can be any usable address)

---

### Q9: Which command removes an IP address from an interface?
A) `no ip address`
B) `remove ip address`
C) `delete ip address`
D) `ip address none`

**Answer: A**

---

### Q10: A /32 subnet mask represents:
A) An entire network
B) A single host
C) A broadcast domain
D) A network with 254 hosts

**Answer: B**

---

### Q11: In Cisco routers, interface IP configuration is done in:
A) Global configuration mode
B) Interface configuration mode
C) Privileged EXEC mode
D) User EXEC mode

**Answer: B**

---

### Q12: What command configures a description for an interface?
A) `description "LAN Interface"`
B) `name "LAN Interface"`
C) `label "LAN Interface"`
D) `comment "LAN Interface"`

**Answer: A**

---

### Q13: To ping the local interface, you would use:
A) `ping localhost`
B) `ping 127.0.0.1`
C) `ping 0.0.0.0`
D) Both A and B

**Answer: D**

---

### Q14: What is the broadcast address for 192.168.1.0/24?
A) 192.168.1.0
B) 192.168.1.1
C) 192.168.1.254
D) 192.168.1.255

**Answer: D**

---

### Q15: Which command shows interface MAC address?
A) `show interface ethernet 0`
B) `show mac address`
C) `show interface hardware`
D) `show mac`

**Answer: A**

---

### Q16: To configure multiple IP addresses on one interface (secondary IP):
A) Configure multiple `ip address` commands
B) Use `ip address secondary`
C) Use `ip address X.X.X.X Y.Y.Y.Y secondary`
D) Not possible on one interface

**Answer: C**

---

### Q17: What is the purpose of a subnet mask?
A) To hide the network
B) To identify which part is network and which is host
C) To encrypt data
D) To speed up routing

**Answer: B**

---

### Q18: A static IP configuration survives a reboot?
A) Yes, if configured in running config
B) No, it's lost after reboot
C) Yes, if saved in startup config
D) Only sometimes

**Answer: C**

---

### Q19: Which command saves configuration to NVRAM?
A) `save config`
B) `write memory`
C) `copy running-config startup-config`
D) Both B and C are correct

**Answer: D**

---

### Q20: What is the host address in 10.0.0.0/8?
A) 10.0.0.0
B) 10.255.255.255
C) Any address from 10.0.0.1 to 10.255.255.254
D) All of the above

**Answer: C**

---

## MEDIUM LEVEL

### Q21: You need to configure three IP addresses on FastEthernet0/0. What sequence of commands would you use?
A) Three separate `ip address` commands
B) First `ip address X.X.X.X Y.Y.Y.Y`, then two `ip address X.X.X.X Y.Y.Y.Y secondary`
C) Use `ip alias` command
D) Not possible on one physical interface

**Answer: B**

---

### Q22: Configure IP 172.16.0.1/28 on Gig0/0. What is the usable host range?
A) 172.16.0.0 - 172.16.0.15
B) 172.16.0.1 - 172.16.0.14
C) 172.16.0.1 - 172.16.0.15
D) 172.16.0.2 - 172.16.0.14

**Answer: B**

---

### Q23: Which command displays detailed interface statistics?
A) `show interface`
B) `show ip interface detail`
C) `show interface status`
D) `show interface statistics`

**Answer: B**

---

### Q24: To configure a static IP 10.10.10.5/30 on Serial0/0, what is the broadcast address?
A) 10.10.10.4
B) 10.10.10.5
C) 10.10.10.6
D) 10.10.10.7

**Answer: D**

---

### Q25: What command verifies IP configuration on an interface?
A) `ping interface`
B) `verify ip`
C) `show running-config interface fastethernet 0/0`
D) All of the above

**Answer: C**

---

### Q26: You configured IP 192.168.1.1/24 but can't reach 192.168.1.100. What should you check?
A) Interface is up/up
B) No shutdown command is issued
C) Routing is configured towards target network
D) All of the above

**Answer: D**

---

### Q27: In the command `ip address 10.0.0.1 255.255.0.0 secondary`, what does "secondary" mean?
A) It's the backup IP
B) It's an additional IP on the interface
C) It's less important than primary IP
D) It's for secondary interfaces only

**Answer: B**

---

### Q28: Configure IP on loopback interface for router ID. Which subnet is typically used?
A) /24
B) /25
C) /30
D) /32

**Answer: D**

---

### Q29: What does `show ip interface brief` display?
A) Detailed configuration of each interface
B) Only IP addresses
C) Interface status, IP address, and protocol status (up/down)
D) Only physical layer information

**Answer: C**

---

### Q30: How to disable IPv6 on an interface while keeping IPv4?
A) `no ipv6 enable`
B) `no ipv6 address`
C) `ipv6 disable`
D) `no ip version 6`

**Answer: B**

---

### Q31: What command resets interface statistics?
A) `clear interface counters`
B) `reset counters`
C) `clear statistics`
D) Not possible

**Answer: A**

---

### Q32: You need to check if interface is physically up. Which command?
A) `show interface status`
B) `show interface brief`
C) `show ip interface`
D) `show interface description`

**Answer: A**

---

### Q33: To assign description "To Server" to Fa0/1, what command?
A) `description "To Server"`
B) Enter Fa0/1 context first, then `description "To Server"`
C) `interface Fa0/1 description "To Server"`
D) Not possible in CLI

**Answer: B**

---

### Q34: A /31 subnet mask has how many usable addresses?
A) 0
B) 1
C) 2
D) 3

**Answer: C**

---

### Q35: To see memory usage and interface details, which command?
A) `show memory`
B) `show process`
C) `show interface`
D) `show version`

**Answer: C**

---

### Q36: Configure IPv4 address 172.20.1.1 and IPv6 2001:db8::1 on same interface - is it possible?
A) No, only one can exist
B) Yes, both can coexist
C) Only on loopback
D) Only on serial interfaces

**Answer: B**

---

### Q37: What happens when you type `no shutdown` on a shutdown interface?
A) Interface remains down
B) Interface goes up immediately
C) Interface goes to a pending state
D) Configuration is rejected

**Answer: B**

---

### Q38: To verify connectivity between two static IP interfaces, use:
A) `tracert`
B) `ping`
C) `test connectivity`
D) `show route`

**Answer: B**

---

### Q39: In static IP configuration, what is MOST critical?
A) Using /24 only
B) Configuring no shutdown
C) Choosing high IP addresses
D) Using public IPs only

**Answer: B**

---

### Q40: Multiple static IPs on one interface cause:
A) Interface errors
B) Routing loop
C) No issues - legitimate use case
D) Bandwidth problems

**Answer: C**

---

## HARD LEVEL

### Q41: Configure interface Gig0/0 with primary IP 10.0.0.1/24 and secondary IP 192.168.1.1/24. What are the complete commands?
A) `interface Gig0/0` → `ip address 10.0.0.1 255.255.255.0` → `ip address 192.168.1.1 255.255.255.0`
B) `interface Gig0/0` → `ip address 10.0.0.1 255.255.255.0` → `ip address 192.168.1.1 255.255.255.0 secondary`
C) Both A and B produce valid results
D) Neither - secondary must use /30

**Answer: B**

---

### Q42: You have 172.16.0.0/22. You want to assign subinterface IP to Gig0/0.1 as 172.16.1.1/25. Is this valid?
A) Yes, it's within the range
B) No, it overlaps with primary interface
C) Yes, but you must delete primary IP first
D) No, subinterfaces can't use smaller subnets

**Answer: A**

---

### Q43: Configure static IP on a subinterface: what's the difference compared to physical interface?
A) Use `ip address-family` instead of `ip address`
B) Must create VLAN first, then assign IP
C) Same commands, but must create subinterface first
D) Requires special licensing

**Answer: C**

---

### Q44: What does `passive-interface` do in routing context with static IPs?
A) Makes interface ignore static routes
B) Prevents sending routing updates on interface
C) Disables interface for backup only
D) Reduces IP address range

**Answer: B**

---

### Q45: You need failover between two static IPs. What's the best approach?
A) Configure VRRP/HSRP with static IPs
B) Manually switch at reboot
C) Configure in DNS
D) Not possible with static IPs

**Answer: A**

---

### Q46: In a point-to-point link 10.1.1.0/30, you assign 10.1.1.1 to Router A. What's best for Router B?
A) 10.1.1.2
B) 10.1.1.3
C) 10.1.1.0
D) Any of the above

**Answer: A**

---

### Q47: To track interface with IP 10.0.0.1/24 using object tracking, what's the command?
A) `track 1 interface Gig0/0 ip routing`
B) `track 1 ip routing Gig0/0`
C) `ip tracking object 1`
D) Not possible with static IP

**Answer: A**

---

### Q48: Static IP on management interface (vty) - what command enters interface config?
A) `interface vty 0 4`
B) Can't configure IP on vty
C) Use `line vty 0 4` then `ip address`
D) Special command: `mgmt ip address`

**Answer: B**

---

### Q49: Unnumbered interface uses another interface's IP. Command?
A) `ip address copy from Gig0/0`
B) `ip unnumbered Gig0/0`
C) `ip address reference Gig0/0`
D) Not available in modern IOS

**Answer: B**

---

### Q50: What's the impact on routing when you remove static IP from interface?
A) No impact - routes remain
B) Routes pointing to that interface become invalid
C) Automatic failover to backup route
D) Interface goes to standby mode

**Answer: B**

---

### Q51: Configure IP 10.0.0.0/24 with host bits set (impossible in real networks). What happens?
A) IOS auto-corrects to 10.0.0.0
B) IOS rejects the configuration
C) IOS creates it but warns
D) IOS crashes

**Answer: B**

---

### Q52: Static IP configuration in OSPF network - what's the role of loopback IP?
A) Only for emergency backup
B) Serves as router ID if highest IP
C) Completely separate from OSPF
D) Must match OSPF area wildcard

**Answer: B**

---

### Q53: You need sub-interfaces on Fa0/0: .1 with 10.1.1.1/25, .2 with 10.1.1.129/25. Valid?
A) Yes, no issues
B) No - they'd need trunking between them
C) Yes - they're on same physical link
D) Only if MPLS is enabled

**Answer: A**

---

### Q54: EtherChannel with static IPs: Can you load-balance across multiple links?
A) No - static IPs only work on single link
B) Yes - EtherChannel keeps same IP
C) Only for DHCP clients
D) Requires special routing command

**Answer: B**

---

### Q55: Configure static IP on tunnel interface 10.0.0.1/24. What command first?
A) `interface tunnel 0`
B) `tunnel interface 0`
C) `create tunnel 0`
D) `tunnel 0`

**Answer: A**

---

### Q56: What's the implication of static IP with /32 subnet?
A) It can reach only itself
B) It's a host address, not used in real deployment
C) Typically used for loopback or P2P links
D) Automatically becomes DHCP

**Answer: C**

---

### Q57: In spanning tree, static IP on bridge groups - does it affect STP?
A) No - STP works at Layer 2
B) Yes - must coordinate with RSTP
C) Only if VLAN ID matches
D) Requires manual STP tuning

**Answer: A**

---

### Q58: Static IP in Cisco SD-WAN (Viptela): Same commands as traditional IOS?
A) Yes - identical commands
B) Mostly same, but with SD-WAN context
C) Different syntax entirely
D) Not supported

**Answer: B**

---

### Q59: Configuring static IP with ACL filter on interface - order of configuration?
A) First IP, then ACL
B) First ACL, then IP
C) Order doesn't matter
D) Must use special command `ip address acl`

**Answer: A**

---

### Q60: What's the best practice for static IP addressing in large networks?
A) Use /8 for everything
B) Use /32 for everything
C) Implement subnetting strategy, document allocation
D) Random assignment to avoid patterns

**Answer: C**

---

### Q61: Static IP on PPPoE interface - possible?
A) No - PPPoE requires DHCP
B) Yes - static IP inside PPPoE session
C) Yes - as PPPoE parameter directly
D) Only in older IOS versions

**Answer: B**

---

### Q62: Configure redundancy for static IP using VRRP virtual IP 10.0.0.10/24:
A) Cannot use static IP with VRRP
B) Configure physical static IPs, then VRRP virtual IP on top
C) Only use virtual IP, remove physical
D) Requires BGP integration

**Answer: B**

---

### Q63: Static IP in multi-context security appliance - is scope global or local?
A) Always global
B) Always local to context
C) Depends on configuration mode entered from
D) Can be either - configurable

**Answer: C**

---

### Q64: What's the maximum useful prefix length for static P2P link IP?
A) /24
B) /25
C) /30
D) /32

**Answer: C**

---

### Q65: Static IP with route-map filtering - which command applies it?
A) `ip address X.X.X.X route-map NAME`
B) Use access-list, then route-map separate
C) `apply ip address to route-map`
D) Not possible on interface IP

**Answer: B**

---

### Q66: Configure IP 192.0.2.1/24 on interface for testing. After testing, remove it. What's the full removal command?
A) `delete ip address`
B) `no ip address`
C) `ip address none`
D) `ip address 0.0.0.0`

**Answer: B**

---

### Q67: In NSF (Non-Stop Forwarding), do static IPs on backup cards failover instantly?
A) No - requires manual reconfig
B) Yes - NSF handles it automatically
C) Only if synchronized first
D) Only for HSRP-configured IPs

**Answer: B**

---

### Q68: Static IP in VRF context - must it differ from global context?
A) Yes - always must differ
B) No - can use same subnets in different VRFs
C) Only if routes are different
D) Requires special command to isolate

**Answer: B**

---

### Q69: What happens when two interfaces on same router have overlapping static IPs?
A) Automatic failover occurs
B) IOS prevents the configuration
C) Both are active - routing table uses longest match or order
D) Secondary one becomes inactive

**Answer: B**

---

### Q70: Static IP on demand circuit (DDR) - does it remain assigned when link is down?
A) No - removed when PPP closes
B) Yes - remains in config
C) Yes - but packet-switched only
D) Depends on routing protocol

**Answer: B**

---

## COMMAND REFERENCE

Common Static IP Commands:
```
interface GigabitEthernet0/0
 ip address 192.168.1.1 255.255.255.0
 ip address 192.168.2.1 255.255.255.0 secondary
 no shutdown
 description "Primary LAN"
exit

interface Loopback0
 ip address 10.0.0.1 255.255.255.255
exit

! View configurations
show ip interface brief
show ip interface detail
show running-config interface GigabitEthernet0/0

! Remove IP
no ip address

! IPv4 & IPv6 coexist
interface Gig0/0
 ip address 10.0.0.1 255.255.255.0
 ipv6 address 2001:db8::1/64
exit

! Subinterface
interface GigabitEthernet0/0.1
 encapsulation dot1q 10
 ip address 192.168.10.1 255.255.255.0
exit

! Save config
copy running-config startup-config
write memory
```

---

## KEY CONCEPTS

1. **Static vs DHCP**: Static is manually configured, DHCP is automatic
2. **Subnet Mask**: Determines network and host portions of IP
3. **Primary vs Secondary IP**: Primary is main, secondary is additional on same interface
4. **Loopback Interface**: Always up, used for router ID, management
5. **no shutdown**: Essential to bring interface up
6. **Configuration Persistence**: Must save to startup-config for persistence after reboot
7. **Interface Types**: Fast Ethernet, Gigabit, Serial, Tunnel, Loopback (all support static IP)
8. **Pointto-Point**: Typically /30 or /31 for efficiency
9. **Multi-IP Scenarios**: Secondary IPs useful for migration, redundancy
10. **Error Checking**: Must verify no overlaps and proper routing exists

