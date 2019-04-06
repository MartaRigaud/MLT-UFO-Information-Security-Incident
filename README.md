# MLT-UFO-Information-Security-Incident
Information Security Incident domain


Considering a computational environment, a number of devices, such as computers, network equipment, software, data, among others are 
utilized for various purposes. Therefore, the operation of these information assets involves numerous events. In this context, an event 
is a sequence of directed actions with specific purposes as a consequence of  a change in the state of an information asset. Whenever 
the actions have the intention of resulting in something that is not allowed to happen, an attack is set up.


The occurrence of an attack involves a participation of an attacker. An attacker employs a tool malicious to explore an information asset vulnerability and performs an action to obtain an unauthorized result [29]. Often, a succession of attacks occur by the same attacker to cause damage. These attacks are part of an incident. In this way, an incident is a group of attacks that can be distinguished from others considering the attackers, attacks and damages involved. An incident can be understood as a simple attack or a set of attacks. Figure 1 shows an Incident model using the UFO taxonomy.
	

As shown in Figure 1, an "Incident" is an instance of "Complex Event" because it consists of one or more "Attack" ("Atomic Event") that
were committed by the same Attacker to reach a certain "Damage" ("Situation").


As an Event,  "Attack" depends on the participation of objects. "Person" , "Information Asset" and "Tool" are objects participants
of an “Attack”. A "Person", playing the role of "Attacker", "Raise" a sort of "Tool", playing the role of "Malicious", to execute an 
"Attack". When the "Attack" happens, it looks for some "Information Asset" in  "Vulnerable" pre-state. Then, the action of the "Attack" 
produces an unauthorized result. So,  the "Information Asset" before the attack is in the "Vulnerable" situation and then goes to 
"Unauthorized Result" situation. The set of unauthorized results of attacks in an incident leads to a "Damage" situation.	


Figure 2 illustrates part of a model for "Information Asset" employing UFO-MLT. "Information Asset" specializes "Individual" and is 
instance of "Category." So, "Information Asset" is classified as first-order type. As a "Category", "Information Asset" generalizes 
properties of different types of assets. These types are classified by a second-order type "Information Asset Kind" that specialize 
"Kind" and partition "Information Asset", i.e., each instance of “Information Asset” is instance of one and only one instance of 
“Information Asset Type", applying as classification criterion the inheritance of its principle of identity, having as instances the 
kinds "Process", "Account", "Data", "Component", "Computer", "Network" and "Internetwork."


Similarly, the "Tool" utilized by "Attacker" can be represented. The "Tool" is instance of "Category" partitioned by second-order 
type "Tool Kind" that specializes "Kind". In this context, "Physical Attack", "Information Exchange", "User Command", "Script or 
Program" and "ToolKit" are instances of kinds illustrated in Figure 2 exemplify the types of tools.


The situations that make possible attack occurrence and the ones which follow the attack can be detailed. Furthermore, a series of 
unauthorized situations caused by attacks can lead to various types of damage. Figure 3 illustrates the types of situations that lead 
an "Information asset": (i) to become vulnerable; (ii) to generate an unauthorized result; and (iii) to be damaged. "Vulnerable", 
"Unauthorized Result" and "Damage" specialize "Individual" and are instances of "Situation", being classified as first-order type 
entities. The second-order type "Vulnerable Type" specializes "Situation" and may thus categorizes an instance of "Vulnerable" 
defining as classification criteria the distinct stages of life of an "Information Asset": implementation time, specification time 
and use time. Types such as "Implementation Vulnerable", "Specification Vulnerable" and "Configuration Vulnerable" represent examples 
of instances of "Vulnerable Type." "Unauthorize Result Type" specializes "Situation" and categorizes "Unauthorized Result" defining as 
classification criteria the consequences of a well-succeeded attack: "Increased access", "Disclosure of information", "Corruption of 
information", "Denial of service" and "Theft of resources." Finally, "Damage Type" is a second-order type that specializes "Situation" 
and categorizes instances of "Situation" using damage qualities as classification criteria.


Attackers are categorized according to the objectives employed in an incident. As shown in Figure 4, it was defined as a second-order 
type "Person Role" that categorizes "Person" according to role that a person may play during an "Attack" having as instances "Attacker".
More specific specializations of "Person Role" include "Attacker Role" whose instances specialize "Attacker". Types such as "Corporate 
Raider", "Hacker", "Spy" and "Professional Criminal" which are examples of instances of "Attacker Role".	


Attacks, according to [29], can be categorized into "Stealing passwords", "Social Engineering", "Bugs and Backdoors", "Authentication 
Failures", "Protocol Failures", "Information Leakage" and "Denial of Service" (DoS). Being "Attack" an instance of the base type 
"Atomic Event", it is also a first-order type. "Attack Type" are specialized instances of "Atomic Event" and  categorizes "Attack". 
These examples of second-order types specializing "Attack" are illustrated in Figure 5.


Attack types can be specialized in types to be represented in more detail by increasing the expressiveness of the model. For example, 
a Denial of Service (DoS) attack makes a system unavailable to its legitimate users. It can be specialized in the Distributed Denial of 
Service (DDoS) attack when unavailability is caused from different sources. These sources send packet streams, consuming some key 
resources and rendering it unavailable to legitimate users [23].


Thus, the DDoS attack has several sorting criteria. The mechanism used to attack was utilized by [23] to establish eight DDoS attack 
classification criteria. Figure 10 shows the representation of three of these classes using MLT.


Attacks are classified according to the attack method (for example, "DoS") giving rise to types of attacks. Therefore, "Attack Type" 
is type of "2ndOT" that categorizes "Attack". In this context, "DoS" is an instance of "Attack Type". The DoS attack can be classified 
according to a criterion, i.e., an "Attack Type" can specialize in a third order type of "Attack DoS Type" and categorizes "DoS". 
"DDoS" is instance of "Attack DoS Type" which is specialized for "Attack DDoS Type". Types "4thOT" such as "Attack DDoS degree of 
automation type", "Attack DDoS exploited weakness type" and "Attack DDoS  possibility of characterization type" are examples 
specialization of "Attack DDoS Type".


Descending in the classification hierarchy of the DDoS attack, it becomes possible to make explicit the rules applied to classify 
an attack by the possibility of characterization. A DDoS attack is characterized when it is possible to identify its occurrence by 
inspecting the packet headers. Consequently, the attack that can not be identified by inspection of the packet headers is 
non-characterizable. In addition, the characterizable DDoS attack may be filterable or non-filterable. The DDoS filterable attack uses 
malformed packets or packets that are not required for the normal operation of the information asset [23]. Figure 7 details this 
classification structure.


Thus, attacks DDoS require multiple levels of classification. Figure 7 depicts the application of MLT for DDoS attacks. All 
instances of "Attack DoS Type" are proper specializations of "DoS". It is represented by the categorization relation between a higher 
order type "Attack DoS Type" and a base type "DoS" because all instances of "DoS" specialize "Attack DoS Type" according to specific 
classification criteria (in this case, attack method). So, "DDoS" is a specialization of "DoS" and an instance of "Attack DoS Type".


Similarly, "Attack DDoS Type", with its instances "UDP Flooding", "Smurf", "Sockstress", "Slow HTTP" and "HTTP Flooding", specializes 
"Attack DoS Type" and categorizes "DDoS". Moreover, each "DDoS" is an instance of an instance of one of the "Attack DoS Type". 
Therefore, each instance of "Attack DDoS Type" categorizes "DDoS". In addition, instances of "DDoS" ("Attack DDoS Type" specializations)
form a chain of subordination, i.e., instances of "Attack DDoS Filtration", are specializations instances of "Attack DDoS 
Characterization". Thus, instances of "DDoS" may specialize: (i) instances of "Attack DDoS Filtrable" ("UDP Flooding" and "Smurf" 
in the example); (ii) instances of "Attack DDoS Non-filterable" ("Sockstress", "Slow HTTP" and "HTTP Flooding" in the example).
