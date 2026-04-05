# QoS & Classification (ECL/MQC) MCQ Quiz

---

## EASY LEVEL

### Q1: What is QoS (Quality of Service)?
A) Mechanism to prioritize network traffic
B) Ensures minimum bandwidth/latency guarantee
C) Classifies and marks traffic
D) All of above

**Answer: D**

---

### Q2: MQC (Modular QoS CLI) components:
A) Class-map, Policy-map, Service-policy
B) Defines traffic classification
C) Both concepts
D) No such structure

**Answer: C**

---

### Q3: Traffic classification - main purpose:
A) Identify different traffic types
B) Apply policies per class
C) Both purposes
D) Just for logging

**Answer: C**

---

### Q4: Create class-map:
A) `class-map match-any CLASS_NAME`
B) `match protocol http`
C) Both steps
D) `create class-map CLASS_NAME`

**Answer: C**

---

### Q5: Policy-map applies:
A) Actions to class-maps
B) Bandwidth/priority per class
C) Both elements
D) Independent of class-map

**Answer: C**

---

### Q6: Service-policy applies:
A) Policy-map to interface
B) Direction (in/out)
C) Both required
D) `apply policy-map`

**Answer: C**

---

### Q7: DSCP (Differentiated Services Code Point):
A) 6-bit field in IP header
B) Marking for QoS handling
C) Both characteristics
D) Port-based only

**Answer: C**

---

### Q8: CoS (Class of Service) - where is it?
A) Ethernet frame (3 bits)
B) 802.1p priority
C) Both same thing
D) IP header

**Answer: C**

---

### Q9: Traffic policing - what does it do?
A) Limits traffic to configured rate
B) Drops/marks excess traffic
C) Both aspects
D) Increases bandwidth

**Answer: C**

---

### Q10: Traffic shaping - differs from policing:
A) Buffers instead of dropping
B) Smooths traffic rate
C) Both characteristics
D) Same as policing

**Answer: C**

---

### Q11: Queue management (FIFO):
A) First-in-first-out
B) Default queue behavior
C) Both true
D) Always uses priority

**Answer: C**

---

### Q12: Priority queue (PQ):
A) Critical traffic first
B) Other traffic delayed
C) Both behaviors
D) Equal treatment

**Answer: C**

---

### Q13: Fair Queuing (FQ):
A) Equal bandwidth share
B) Per-flow fairness
C) Both benefits
D) Unfair distribution

**Answer: C**

---

### Q14: Congestion tail drop:
A) Drops packets when queue full
B) Causes TCP timeouts/retransmits
C) Both consequences
D) Optimal behavior

**Answer: C**

---

### Q15: RED (Random Early Detection):
A) Drops packets proactively before congestion
B) Signals routers to reduce rate
C) Both mechanisms
D) Wait for full queue

**Answer: C**

---

### Q16: Mark traffic with DSCP:
A) `set dscp EF` (Expedited Forwarding)
B) In policy-map class action
C) Both true
D) `mark dscp EF`

**Answer: C**

---

### Q17: Common DSCP values:
A) EF (Expedited = 46)
B) AF (Assured = 10-38)
C) Both standard
D) No standard values

**Answer: C**

---

### Q18: View applied QoS policy:
A) `show policy-map interface`
B) Shows statistics per class
C) Both show info
D) `show qos interface`

**Answer: C**

---

### Q19: Traffic shaping bucket:
A) Token bucket algorithm
B) Rate limiting mechanism
C) Both concepts
D) Not used anymore

**Answer: C**

---

### Q20: Bandwidth reservation - different from policing?
A) Guarantees minimum bandwidth
B) Policing maximum bandwidth
C) Both different purposes
D) Same concept

**Answer: C**

---

## MEDIUM LEVEL

### Q21: Configure VoIP traffic (voice):
A) Classify DSCP EF / CoS 5
B) Priority queue or dedicated bandwidth
C) Both mechanisms
D) No special handling

**Answer: C**

---

### Q22: Implement QoS on WAN link (1 Mbps):
A) VoIP gets 128 kbps guaranteed
B) Data gets remaining 872 kbps
C) Both bandwidth allocations
D) No allocation needed

**Answer: C**

---

### Q23: Create class-map for HTTP traffic:
A) `match protocol http`
B) `class-map match-any WEB`
C) Both parts
D) HTTP automatically detected

**Answer: C**

---

### Q24: Apply policy-map to interface:
A) `service-policy output POLICY_NAME`
B) On egress (outbound) direction
C) Both true
D) `apply-policy POLICY_NAME`

**Answer: C**

---

### Q25: Rate limiting with police:
A) `police 512000 bps`
B) In policy-map class, specifies max rate
C) Both true
D) Shaping uses police

**Answer: C**

---

### Q26: Action on exceeding police rate:
A) `exceed-action drop` / `conform-action transmit`
B) Different actions possible
C) Both aspects
D) Always drop

**Answer: C**

---

### Q27: Hierarchical QoS (traffic classes):
A) Parent/child policy-maps
B) Nested bandwidth allocation
C) Both concepts
D) Flat QoS only

**Answer: C**

---

### Q28: Queue threshold - when does drop occur?
A) Min-threshold triggers marking
B) Max-threshold drops packets
C) Both thresholds
D) No thresholds

**Answer: C**

---

### Q29: Low latency queuing (LLQ):
A) Priority + Fair Queuing
B) Real-time traffic first
C) Both characteristics
D) Just priority queue

**Answer: C**

---

### Q30: WRED (Weighted RED):
A) Marks/drops based on DSCP
B) Higher DSCP = lower drop probability
C) Both behaviors
D) Random drops only

**Answer: C**

---

### Q31: Match criteria in class-map:
A) Protocol, port, DSCP, source, destination
B) Complex matching possible
C) Both true
D) IP address only

**Answer: C**

---

### Q32: Class-map with "match-all" vs "match-any":
A) All criteria must match vs any single
B) Different matching logic
C) Both options available
D) Same result

**Answer: C**

---

### Q33: Mark traffic then match:
A) First policy marks/classifies
B) Second policy uses marked value
C) Both stages
D) One policy only

**Answer: C**

---

### Q34: Jitter in VoIP:
A) Delay variation
B) QoS reduces via priority queuing
C) Both characteristics
D) Static delay

**Answer: C**

---

### Q35: Admission control - what is it?
A) Limits calls when bandwidth insufficient
B) Rejects new flows if threshold reached
C) Both functions
D) No control possible

**Answer: C**

---

### Q36: Bandwidth configured as percentage:
A) `bandwidth percent 25`
B) Of interface capacity
C) Both true
D) Absolute kbps only

**Answer: C**

---

### Q37: QoS in non-dropping scenarios:
A) Still useful for prioritization
B) Prevents congestion proactively
C) Both benefits
D) Only useful when full

**Answer: C**

---

### Q38: Default class in policy:
A) Class with no explicit match
B) Catches unclassified traffic
C) Both true
D) No default class

**Answer: C**

---

### Q39: Aggregate traffic shaping:
A) Shape total across multiple classes
B) Parent policy hierarchy
C) Both concepts
D) No aggregation

**Answer: C**

---

### Q40: Clear QoS counters for fresh stats:
A) `clear policy-map counters`
B) At interface level
C) Both applicable
D) `clear qos counters`

**Answer: A**

---

## HARD LEVEL

### Q41: Design QoS for multi-service network:
A) Voice VoIP priority
B) Video high guaranteed bandwidth
C) Both service types
D) Single class only

**Answer: C**

---

### Q42: Implement DiffServ (Differentiated Services):
A) Service provider edge coloring
B) Core performs per-hop behavior
C) Both roles
D) Per-flow in core

**Answer: C**

---

### Q43: Configure child policy-map in parent:
A) Nested bandwidth allocation
B) Traffic steering to child
C) Both hierarchical
D) Flat structure only

**Answer: C**

---

### Q44: MPLS EXP bits interaction with DSCP:
A) Mapped during MPLS encapsulation
B) Preserved across network
C) Both mechanisms
D) Independent systems

**Answer: C**

---

### Q45: Design QoS for mission-critical application:
A) Dedicated class with min bandwidth
B) Low jitter (priortiy queue)
C) Both protections
D) No special handling

**Answer: C**

---

### Q46: QoS convergence (EIGRP routing + QoS):
A) Fast convergence with QoS-marked paths
B) Routing protocol independent of QoS
C) Both accurate
D) QoS breaks convergence

**Answer: C**

---

### Q47: Implement QoS on branch router (WAN):
A) Shape outbound to ISP rate
B) Prioritize VoIP within branch capacity
C) Both policies
D) No QoS on branch

**Answer: C**

---

### Q48: QoS with NAT interaction:
A) Marks preserved through NAT
B) Classification before/after NAT
C) Both considerations
D) No interaction

**Answer: C**

---

### Q49: Design QoS for video conference:
A) Reserved bandwidth (15-25% for video)
B) DSCP EF or AF43
C) Both solutions
D) Best-effort only

**Answer: C**

---

### Q50: Micro-burst handling via QoS:
A) Token bucket absorbs small bursts
B) Prevents packet drop for short peaks
C) Both benefits
D) Can't handle micro-bursts

**Answer: C**

---

### Q51: Implement QoS with redundancy failover:
A) QoS must track active link
B) Backup policy automat switches
C) Both aspects
D) Single QoS across links

**Answer: C**

---

### Q52: QoS for multi-tenancy (VRF):
A) Per-VRF QoS policies
B) Policies isolated per tenant
C) Both characteristics
D) Shared QoS across VRFs

**Answer: C**

---

### Q53: Design QoS for SD-WAN:
A) Central policy provisioning
B) Per-tunnel bandwidth allocation
C) Both characteristics
D) On-premises QoS only

**Answer: C**

---

### Q54: Traffic engineering via QoS (load balancing):
A) Lower cost paths get traffic
B) QoS steers via classification
C) Both mechanisms
D) Routing unrelated to QoS

**Answer: C**

---

### Q55: AQM (Active Queue Management):
A) WRED variant
B) Proactive congestion avoidance
C) Both aspects
D) Passive management only

**Answer: C**

---

### Q56: Configure QoS with ACL:
A) ACL identifies traffic
B) Policy-map applies QoS per class
C) Both integration
D) QoS independent of ACL

**Answer: C**

---

### Q57: QoS in cloud connectivity:
A) Public cloud ingress/egress marked
B) Border policies apply
C) Both concepts
D) No cloud QoS needed

**Answer: C**

---

### Q58: Implement QoS for real-time gaming:
A) Ultra-low latency required (LLQ)
B) Fixed bandwidth insufficient
C) Both must apply
D) Best-effort acceptable

**Answer: C**

---

### Q59: QoS with IPv6:
A) DSCP still 6 bits in Traffic Class
B) Equivalent functionality to IPv4
C) Both true
D) Different in IPv6

**Answer: C**

---

### Q60: Design QoS for disaster recovery:
A) Critical apps prioritized
B) Non-critical throughput minimum guaranteed
C) Both allocation tiers
D) No special DR QoS

**Answer: C**

---

### Q61: Queue drop simulation (testing):
A) Set max-queue size below normal
B) Observe application behavior
C) Both testing aspects
D) No recommended testing

**Answer: C**

---

### Q62: Implement QoS for SLA compliance:
A) Jitter < 50ms commitment
B) Loss < 0.5%
C) Both SLA targets
D) No SLA guarantees

**Answer: C**

---

### Q63: PIR (Peak Information Rate) vs CIR:
A) CIR = committed rate
B) PIR = burst rate
C) Both concepts
D) No distinct rates

**Answer: C**

---

### Q64: Design QoS for campus network:
A) Access layer classifies (ACL+policy)
B) Distribution/core prioritizes
C) Both layers involved
D) Access layer only

**Answer: C**

---

### Q65: Implement QoS with link aggregation:
A) QoS per link bundle
B) Equal distribution by default
C) Both characteristics
D) Single QoS inappropriate

**Answer: C**

---

### Q66: Buffer management in QoS:
A) Queue size limits
B) Drop/mark threshold tuning
C) Both buffer controls
D) No buffer management

**Answer: C**

---

### Q67: Design QoS monitoring/alerting:
A) SNMP statistics polling
B) Threshold-based alerts configured
C) Both monitoring methods
D) No monitoring available

**Answer: C**

---

### Q68: QoS for machine learning / big data:
A) Bulk transfer low priority
B) Interactive query higher priority
C) Both traffic types
D) Same priority for all

**Answer: C**

---

### Q69: Implement QoS with SRv6 (Segment Routing):
A) Path selection includes QoS
B) Traffic steered to optimal path
C) Both mechanisms
D) No interaction with routing

**Answer: C**

---

### Q70: Design multi-level QoS policy hierarchy:
A) Global, regional, site-specific tiers
B) Parents delegate to children
C) Both hierarchy levels
D) Single flat policy only

**Answer: C**

---

## COMMAND REFERENCE

```
! Create class-map
class-map match-any VOICE
 match ip dscp ef
 match protocol voip
exit

! Create policy-map
policy-map QoS_Policy
 class VOICE
  priority 256  ! Strict priority, 256 kbps
 class VIDEO
  bandwidth 512  ! Guarantee 512 kbps
  random-detect  ! WRED
 class DEFAULT
  buffer-policy drop-tail
exit

! Apply service policy
interface Serial0/0
 service-policy output QoS_Policy
exit

! View applied QoS
show policy-map interface Serial0/0

! Mark traffic with DSCP
policy-map MARK_DSCP
 class WEB
  set dscp af31
 class VOICE
  set dscp ef
exit

! Traffic shaping (bandwidth limiting)
policy-map SHAPE_POLICY
 class ALL
  shape average 1000000 8000  ! 1 Mbps with 8KB burst
exit

! Police traffic (not shaped, drops excess)
policy-map POLICE_POLICY
 class ALL
  police 512000 negotiate
exit

! Queue configuration
policy-map QUEUE_PRIORITY
 class VOICE
  priority 128  ! Strict priority queue
 class VIDEO
  bandwidth percent 50  ! 50% of available
 class DEFAULT
  fair-queue
exit

! Match based on port
class-map HTTPS
 match protocol https
 match tcp port eq 443
exit

! Show statistics
show policy-map
show policy-map interface interface-name
show class-map

! Clear QoS counters
clear policy-map counters

! Configure hierarchical QoS
policy-map MAIN_POLICY
 class VOICE
  service-policy VOICE_SUB_POLICY
exit

! View detailed interface queue info
show interfaces Serial0/0
show interfaces Serial0/0 queue
```

---

## KEY CONCEPTS

1. **Classification**: Identifies traffic types using ACL, protocol, port, DSCP
2. **Marking**: Applies DSCP/CoS labels for QoS handling downstream
3. **Queuing**: FIFO, Priority, Fair-Queue, WFQ manage traffic order
4. **Congestion Mgmt**: RED/WRED proactively drops; tail-drop at limit
5. **Policing**: Rate limiting with hard limit (drops excess)
6. **Shaping**: Rate limiting with buffering (delays excess)
7. **Priority Queue (PQ)**: Critical traffic first (can starve other traffic)
8. **Fair Queuing (FIQ)**: Equal bandwidth per connection
9. **WFIQ (Weighted Fair)**: Weight-based on traffic class
10. **DSCP**: 6-bit marking field (0-63, 0=none, 46=EF, 8-38=AF)
11. **CoS**: 3-bit Layer 2 marking (802.1p)
12. **Token Bucket**: Traffic policing/shaping algorithm
13. **LLQ (Low Latency Queuing)**: Priority + Fair Queuing
14. **MPLS EXP**: Equivalent to DSCP in MPLS headers
15. **SLA**: Service Level Agreement defining QoS expectations

