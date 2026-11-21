# OpenColo colocation: what's inside the 71,000 sq ft Santa Clara site, who it fits, and what month-to-month really means (power, network and service breakdown)

OpenColo runs one data center: 3223 Kenneth Street in Santa Clara, 71,000 square feet, 9 MW of live capacity with another 4.5 MW under construction, true 2N power, and its own BGP network on AS18779. It also publishes no prices. Every colocation, bare metal and cloud engagement starts with a quote, and every contract runs month to month.

Whether that's good news depends on what you're shopping for. If you want to compare dollars per rack on a web page and check out, this provider can't help you and you'll spend a week finding out. If you need a custom cage in Silicon Valley, racks drawing 30 kW or more, and an exit that doesn't require a lawyer, the spec sheet is worth your time.

> **Quick take**
> - **Best fit:** teams that need custom racks or cages in Santa Clara, high-density power, and a commitment they can end without penalty.
> - **Verified specs:** 2N power with four lithium-ion UPS units, dual 2,750 kW generators, 100% power uptime SLA, 99.999% network SLA, SOC 2 Type II.
> - **The catch:** pricing is quote-only. Your first call is a scoping call, not a checkout.
>
> 👉 [See OpenColo's current colocation specs and open a quote request](https://bit.ly/akkocloud)

## What OpenColo actually sells

Three product lines sit under one roof and one bill: retail colocation, bare metal hosting, and cloud. That combination is rarer than the marketing suggests. Most Santa Clara providers sell you space and hand you to a separate cloud or managed-services partner the moment you need anything above the rack.

| Service | What you get | Power and space options | Billing | Get pricing |
| --- | --- | --- | --- | --- |
| **Rack / cabinet colocation** | Your hardware in a single rack or cabinet, your network, your rules | Busway drops at 30A single-phase, 30A three-phase or 60A three-phase; cross-connects at 1G / 10G / 100G / 400G | Month-to-month, quoted per deployment | [Ask for a rack quote](https://bit.ly/akkocloud) |
| **Custom cage / private suite** | Buildout to your own spec inside the 71,000 sq ft floor, biometric and mantrap access, dedicated onsite storage | Custom power footprint, racks configured for 30 kW+ | Month-to-month, quoted | [Scope a private cage](https://bit.ly/akkocloud) |
| **Bare metal dedicated servers** | Single-tenant hardware sold through the hosting arm the company has run since 2003 under the EGIHosting name | Standard configurations, racked and powered onsite | Month-to-month, quoted | [Check bare metal availability](https://bit.ly/akkocloud) |
| **Cloud (American Cloud)** | Virtual compute run by the same team, sitting next to your physical footprint | On-ramps to AWS, GCP and Azure through PacketFabric, Megaport, Zayo, Comcast and SFMIX | Month-to-month, quoted | [Ask how the cloud tier is priced](https://bit.ly/akkocloud) |
| **Remote hands and onsite support** | In-house technicians for routine tasks; basic remote hands at no charge | 24/7 staff, never outsourced | Included with colocation | [Confirm what remote hands covers](https://bit.ly/akkocloud) |

Every line above is quoted rather than listed. That's not a website oversight: colocation economics depend on committed kilowatts, density, cage footprint and cross-connect count, and a provider publishing a single rack number is usually selling you a 5 kW slice at a density you'll outgrow in a year.

## The specs that actually drive your monthly bill

**Power is the line item that decides everything.** OpenColo takes dual utility feeds from Silicon Valley Power, the municipal utility serving Santa Clara. The company's argument, repeated by CEO Sally Simkiss in a 2022 facility profile, is that SVP delivers the most reliable and least expensive power in California, and that being on SVP rather than PG&E territory is a structural cost advantage rather than a marketing point. Treat that as the operator's claim, but the underlying setup is verifiable: dual feeds, four UPS units on lithium-ion batteries in a true 2N configuration, two 2,750 kW / 3,437 kVA generators, and 7,990 gallons of onsite fuel. The published power SLA is 100%.

**Busway distribution is the detail most buyers miss.** Power reaches racks through busway taps rather than fixed breaker panels, in 30A single-phase, 30A three-phase and 60A three-phase configurations. The practical consequence, as OpenColo's engineering side described it, is that upgrades don't come with long waits or setup charges for new electrical work. If you expect to go from 8 kW to 20 kW per rack in eighteen months, that matters more than the rack rate you negotiate today.

**Cooling is N+1 indirect evaporative**, with four Vertiv IDEC units and hard-walled hot-aisle containment. N+1 means any single unit can be pulled for maintenance without risking a thermal event, which is the minimum bar for a facility running production workloads but not universal at boutique scale.

**Capacity headroom:** 9 MW live, 4.5 MW expansion in progress. A facility with that much room left doesn't need to shuffle you between halls when you add cabinets.

| Facility | Verified detail |
| --- | --- |
| Space | 71,000 sq ft, single operator, racks / cabinets / custom cages |
| Power | Dual SVP feeds, 2N (4x lithium-ion UPS), dual 2,750 kW generators, 7,990 gal fuel, 100% power SLA |
| Capacity | 9 MW live, 4.5 MW expansion underway |
| Cooling | N+1 indirect evaporative, 4x Vertiv IDEC, hard-walled hot-aisle containment |
| Compliance | SOC 2 Type II with annual third-party audit; ISO standards adherence |
| Security | Biometric multi-factor access, mantraps, perimeter fencing, 24/7 in-house guards, CCTV, VESDA with dual-interlock pre-action dry pipe |
| Resilience | Seismic-rated, sited above the 100-year floodplain, raised access flooring |
| Monitoring | DCIM and BMS running 24/7, active from day one of your deployment |

## Two numbers on the directory sites that don't match the operator's sheet

This is where a five-minute check saves a bad shortlist.

**Redundancy.** At least one large colocation directory still lists OpenColo's power as "N+1." The operator's own spec sheet and ColoMap both describe true 2N: four UPS units, dual generators, dual utility feeds. If your SLA negotiation hinges on 2N, ask for the single-line diagram rather than quoting a directory back at the sales team.

**Carrier count.** ColoMap counts 25 carriers on-net. OpenColo advertises more than 50 peered networks. These measure different things. On-net carriers are the ones that will physically hand you a cross-connect in the meet-me room: BandwidthIG, Zayo, Lumen, SVP, AT&T and Comcast are listed, with Boldyn arriving. The 50-plus figure describes networks reachable over OpenColo's own blended BGP. Ask which providers are on-net in the MMR, and which you'd reach only through transit.

## Network: what carrier-neutral means here

OpenColo runs its own multi-homed network on AS18779 with 1G, 10G, 100G and 400G links and a published 99.999% uptime figure. Transit and peering include Arelion, Cogent (AS174), Comcast (AS7922), Zayo (AS6461), Hurricane Electric (AS6939), NetActuate (AS36236) and the SFMIX Bay Area exchange. Cloud fabric runs over Megaport with MegaIX and PacketFabric.

You have three options, and the third is the one worth asking about: bring your own carrier and cross-connect, ride the blended AS18779 service, or do both and use BGP to fail over between them. Dual-homed meet-me rooms with diverse dark fiber from Zayo, BandwidthIG, SVP, Comcast and Lumen back that up, and dark fiber reaches Equinix and CoreSite for the latency-sensitive work.

The building sits roughly ten minutes from San Jose Mineta airport, and the surrounding blocks are dense with other operators. ColoMap lists facilities at 1100 Space Park Drive, 1201 Comstock, 1500 Space Park Drive and 1525 Comstock within a third of a mile. If your architecture depends on a second site that doesn't share your risks, keep it further away than that.

## What month-to-month is worth in real money

No published rate card means no published early-termination schedule either, and OpenColo says contracts are month-to-month as a matter of policy, not as a promotional term. For a startup or a team whose headcount forecast changes twice a year, that removes the single largest hidden cost in a three-year colo deal: the buyout.

It also changes how you should negotiate. With no term to trade, your leverage sits in committed kilowatts and cross-connect volume. Ask what the rate looks like at 10 kW, 30 kW and 60 kW per rack, and whether the quoted number holds if you reduce committed power after six months.

👉 [Get the current month-to-month terms and power pricing from OpenColo](https://bit.ly/akkocloud)

## What to put in the quote request

A vague "how much for a rack" email gets you a vague number. Send these six items and you'll get something you can compare against a competing quote:

1. **Committed kW per rack and total**, plus your expected 12-month growth.
2. **Rack count and cage footprint**, and whether you need a private suite or shared cage space.
3. **Cross-connects**: how many, at what speed, to which carriers, and whether you want the AS18779 blend as a backup path.
4. **Density ceiling** for the specific hall they'd place you in, not the facility average.
5. **Remote hands scope**: what counts as "basic" and free, and what's billed hourly.
6. **Access model**: who gets badges, how biometric enrollment works for contractors, and escort rules after hours.

Two more questions worth asking on the tour: which PDU and busway configuration the quoted rack actually lands on, and what the process and lead time is for adding a second feed.

## Who it fits, and who should keep looking

The workload mix OpenColo describes matches its physical plant:

- **Hybrid cloud with a private footprint.** Your racks in a cage, bursts to AWS, GCP or Azure through direct on-ramps, one team accountable for both halves.
- **High-density AI and GPU clusters.** 9 MW of capacity and power configurations built for 30 kW-plus racks, with 4.5 MW more coming.
- **Latency-sensitive Bay Area applications.** Ten minutes from SJC, dark fiber to the major interconnection campuses nearby.
- **Disaster recovery that isn't in the same building as your primary.** Seismic-rated, above the floodplain, single-operator.
- **Compliance-first deployments.** SOC 2 Type II, biometric access, dedicated cages for fintech, healthcare and government work. Note that HIPAA and PCI-DSS readiness appear in third-party directory profiles rather than the operator's own compliance page, so get the specific controls in writing if either framework is mandatory for you.

Keep looking elsewhere if you want a self-serve order flow, a published price per U, or a global footprint with locations in five markets. OpenColo is one building in Santa Clara, run by a company that started in 2003 as a Counter-Strike server host called EGIHosting, says it has never taken venture money, and whose CEO described it in 2022 as one of the last independent data centers left in the Valley. That independence is why the flexibility exists and also why you won't get a slick procurement portal.

## Moving in

Most deployments go live within weeks of signing. The building has a loading dock with a hydraulic lift built for receiving heavy equipment, cross-connects and carrier circuits can be provisioned before your hardware arrives, and DCIM monitoring is active from day one. Technicians assist with racking, cabling and power-on during a migration, which is the stage where a move from another facility usually slips.

The onsite experience is more practical than most: offices and conference rooms you can lease steps from your racks, customer work areas and a lounge, free parking and facility-wide WiFi, and sales and billing staff who answer a phone rather than routing you into a ticket queue.

👉 [Start an OpenColo migration conversation and check lead times](https://bit.ly/akkocloud)

## FAQ

**Does OpenColo publish colocation prices?**
No. Rack, cage, bare metal and cloud pricing all run through a quote, and contracts are month-to-month.

**Is there a minimum term?**
The company states month-to-month terms across its offerings, with no multi-year lock-in. Confirm the exact wording in the agreement you're sent.

**Can I bring my own carrier?**
Yes. The facility is carrier-neutral with on-net access to BandwidthIG, Zayo, Lumen, SVP, AT&T and Comcast, plus a dual-homed meet-me room. You can also use the AS18779 blend, or both.

**What redundancy should I expect?**
True 2N power: four lithium-ion UPS units, dual utility feeds, dual 2,750 kW generators with 7,990 gallons of onsite fuel, and a 100% power uptime SLA. Cooling is N+1.

**Can it handle GPU-density racks?**
The facility advertises support for racks needing 30 kW or more, with 9 MW installed and 4.5 MW of expansion underway.

**How far is it from the airport?**
About ten minutes from San Jose Mineta (SJC).

## The decision

Match your situation to the rule that fits:

- **You need one or two racks, standard power, and a published price.** OpenColo isn't structured for that; a self-serve retail provider will be faster and cheaper to evaluate.
- **You need a custom cage at 20 kW-plus per rack with a short commitment.** Get a quote here and put the six items above in front of them. Month-to-month terms are the reason to take the call.
- **You're migrating off a multi-year contract you regret.** The absence of a term commitment is the whole argument, and the loading dock and pre-provisioned cross-connects make the move less disruptive than most.
- **You need a DR site that doesn't share your primary's risk.** One building, single operator, seismic-rated, above the floodplain, and close enough for hands-on failover drills.

Before you sign anything, confirm two things in writing: the 2N power topology for the specific rack position you're being sold, and which carriers are physically on-net in the meet-me room versus reachable only through transit. Those two answers separate a good fit from an expensive surprise.

👉 [Request OpenColo's current colocation quote and facility tour](https://bit.ly/akkocloud)
