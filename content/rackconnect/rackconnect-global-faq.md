---
permalink: rackconnect-global-faq/
audit_date:
title: RackConnect Global FAQ
type: article
created_date: '2015-10-16'
created_by: Sameer Satyam
last_modified_date: '2018-05-11'
last_modified_by: Shannon Enix
product: RackConnect
product_url: rackconnect
---

#### What is RackConnect Global?

RackConnect Global is a connectivity service that makes it
possible for you to deploy a hybrid cloud infrastructure connecting Rackspace to infrastructure hosted on your premises, at a colocation provider, or in AWS or Microsoft Azure clouds 
with the best network performance possible. For more details, see
<http://www.rackspace.com/cloud/hybrid/rackconnect/global>.

#### Who is the audience for RackConnect Global and what pain points does it solve?

RackConnect Global is intended for enterprise users that want to connect their
infrastructure at Rackspace with their infrastructure outside of
Rackspace without going over the Internet. Traditionally you would
choose a site-to-site VPN solution or work with a network provider to
drop a leased line into Rackspace data centers. The first solution
results in unpredictable latency and throughput, and the latter involves
working with a third-party provider, which can be costly.
RackConnect Global enables you to deploy your hybrid cloud in a network with low
latency, predictable throughput, and predictable redundancy at a
reasonable cost to you, all managed by Rackspace **Fanatical Support**&reg;.

#### What are the primary use cases?

If you want to use Rackspace infrastructure for backup and disaster recovery
scenarios (for example, database replication), if you are seeking to
avoid the Internet networking path to reduce the latency, and if you want
to make throughput predictable, RackConnect Global helps you achieve this goal.

RackConnect Global also works for customers who want to deploy some components of their infrastructure at Rackspace (for example a database in Rackspace) and other components (web or front end) in other clouds (like Microsoft Azure, Amazon Web Services, Google Public Cloud, and Alibaba Cloud). RackConnect Global makes the connectivity between components
faster and more reliable than connectivity over the Internet.

Lastly, RackConnect Global works for those who have latency-sensitive services (like VoIP or video) on Rackspace and might want dedicated access to Rackspace for good performance.

#### Is this product being launched for dedicated hosting or cloud customers? What networks can be connected?

RackConnect Global is primarily for Rackspace dedicated hosting users at
launch. Dedicated hosting users who want to establish a virtual circuit
to connect the dedicated private (ExNet) address space at Rackspace to a
private address space on their side of the connection (for purposes like
disaster recovery or business continuity, for example, database replication)
are the target customer set. However, Rackspace cloud or dedicated
hosting customers who want to access public prefixes via RackConnect Global can also do
so via dedicated cross-connect only. Note that customers cannot use
RackConnect Global to connect to private prefixes on the Rackspace Public
cloud (for example, cloud networks).

#### In what regions is the service available?

RackConnect Global is available in Rackspace data centers across the U.S., Europe, and Australia with connectivity to enabled Equinix and Megaport locations across North America, Europe, Australia, and New Zealand. You can also use RackConnect Global to connect Rackspace regions across the U.S. and Europe along the Rackspace backbone, which avoids the Internet. View the detailed connectivity map and table here: <http://www.rackspace.com/cloud/hybrid/rackconnect/global>.

#### What are the connectivity options for users to establish a connection via RackConnect Global?

Users can connect via the following means:

- Dedicated cross-connect, if they are colocated at supported Equinix facilities or Megaport locations in North America, Europe, Australia, and New Zealand. 

- As a buyer on the Equinix or Megaport cloud exchange

- As a Microsoft Azure customer using ExpressRoute (this is a Microsoft Equivalent of RackConnect Global)

#### Can I connect to public cloud isolated networks (cloud networks) over RackConnect v3?

No, we do not support any sort of connectivity to Rackspace public cloud resources via RackConnect v2.0 or v3.0 at this time.

#### What speeds are supported?

Connectivity speeds of 100 Mbps, 200 Mbps, 500 Mbps, 1 Gbps, 2 Gbps, 5 Gbps, and 10 Gbps are supported. Higher speeds will be handled on a case-by-case basis. Note
that these are the speeds supported by Rackspace and can be
supported only if the other end of the virtual circuit is capable of
supporting these speeds.

#### Is a dedicated aggregation (customer edge) device needed to use this service?

Customers have the option between using a shared 10G aggregation switch or a dedicated 10G aggregation (customer edge) switch. 

#### Are dedicated TORs needed to use this service?

Yes, dedicated TORs are needed. We cannot connect shared TORs to dedicated
aggregation devices because that would create a problem with zone management,
billing, automation, and monitoring, and complicate troubleshooting. We currently recommend one of the following devices:
•	Cisco Catalyst 4948E
•	Cisco Nexus 9372TX
•	Arista 70570S-64
•	Arista 750TX-64

#### Is the traffic secure?

The traffic rides all the way through the Rackspace
Backbone (the network that interconnects Rackspace regions and provides
connectivity outside of Rackspace) without hitting the Internet path and
is inherently secure. It is purely an
MPLS VPN connection. The service does not provide encryption of any sort. 

#### Does the service have an SLA?

Rackspace guarantees that the termination end point for the RackConnect Global Service virtual circuit will be able to accept connections 99.9% of the time in any calendar month, provided that there are two or more virtual circuit termination end points at the Rackspace data center location. You can read the agreement at (https://www.rackspace.com/information/legal/rackconnect-global-regionlink).

#### What is the high-level procedure by which an RackConnect Global connection can be ordered and provisioned for the customer?

The complete procedure can be found at [RackConnect Global user workflow](/how-to/rackconnect-global-user-workflow).
