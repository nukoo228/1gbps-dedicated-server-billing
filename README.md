# Dedicated Server Hosting 1Gbps: Is the Port Enough, Metered or Unmetered, and What Else Lands on the Bill? (Full Plan Table)

A 1 Gbps port caps how fast data leaves your server in any given second. It says nothing about how much data you are allowed to push across a month, and the monthly volume is the number that produces overage invoices. Ava Hosting lists four dedicated servers, all with a 1 Gbps port, from USD 95.32/mo, and the product page does not publish a monthly traffic allowance for any of them. Below are the verified plans with current prices, how metered and unmetered actually differ on an invoice, the add-ons that raise the real monthly cost, and which of the four boxes fits a streaming, gaming, or e-commerce workload.

> **Quick pick:** the 2x Intel Xeon E5-2620 v3 at **USD 134.57/mo** is the sensible default. It is the cheapest Ava plan that pairs DDR4 memory with SSD storage, both expandable, and 12 cores / 24 threads covers a busy web or application stack. The USD 111.02 dual E5-2680 v2 gives you more cores and 256 GB of RAM for less money, but runs on DDR3 and 600 GB SAS drives.
> 👉 [Check current Ava dedicated server stock and configuration options](https://my.ava.hosting/aff.php?aff=15562)

## Ava Hosting 1Gbps dedicated servers: full lineup

| Plan | CPU | RAM | Storage | Port | Price / order |
| --- | --- | --- | --- | --- | --- |
| AMD Ryzen 5 4650G | 6 cores / 12 threads | from 16 GB DDR4 | from 256 GB NVMe, up to 4 extra disks | 1 Gbps | from **USD 95.32/mo** —  [Order](https://my.ava.hosting/aff.php?aff=15562) |
| 2x Intel Xeon E5-2680 v2 | 20 cores / 40 threads | 256 GB DDR3 ECC | 8 × 600 GB SAS HDD | 1 Gbps | from **USD 111.02/mo** —  [Order](https://my.ava.hosting/aff.php?aff=15562) |
| 2x Intel Xeon E5-2620 v3 | 12 cores / 24 threads | from 32 GB DDR4 | from 1 TB SSD | 1 Gbps | from **USD 134.57/mo** —  [Order](https://my.ava.hosting/aff.php?aff=15562) |
| 2x Intel Xeon E5-2699 v3 | 36 cores / 72 threads | from 32 GB DDR4 | from 1 TB SSD | 1 Gbps | from **USD 167.09/mo** —  [Order](https://my.ava.hosting/aff.php?aff=15562) |

Every plan includes 1 IPv4 address, free DDoS protection, 24/7 support, and optional add-ons. RAID controller and remote management appear on the three Xeon listings; the Ryzen listing does not mention them, so confirm both if you need hardware RAID or IPMI-style access.

Three things about that table are easy to misread.

The prices are floors. "RAM from 16 GB", "Disks from 256 GB NVMe", and "up to 4 additional disks" mean the checkout total rises as you configure. The USD 95.32 figure buys the minimum configuration, not a typical one.

Currency changes between product lines. The dedicated server page quotes USD; the VPS pages on the same store quote EUR (from €2.00/mo for 1 vCPU / 1 GB / 15 GB NVMe). Check the currency selector before you stack Ava against a quote in another currency.

More cores does not mean more money here. The 20-core dual E5-2680 v2 costs USD 23.55 less per month than the 12-core dual E5-2620 v3. The gap is platform age: DDR3 memory and 600 GB SAS disks on the cheaper box versus DDR4 and SSD on the dearer one.

## What the 1 Gbps port buys, and what it does not

1 Gbps is 125 MB per second. Held at that rate for 30 days, the port moves roughly 324 TB. That is the theoretical ceiling, and almost nobody reaches it.

Providers routinely sell the same 1 Gbps port with a monthly volume cap attached, which tells you the two figures are accounted separately:

| Provider | Port and traffic pairing | Notes |
| --- | --- | --- |
| noushost | 1 Gbps with 50 TB/mo on every plan in that line, from $45.80/mo (Xeon E3-1230v6, 16 GB, 250 GB SSD) | Runs a separate 1 Gbps unmetered line |
| HOSTKEY | 1–10 Gbps port, 50 TB guaranteed on the listed configuration | Inbound free under fair use, outbound rated by the traffic plan |
| Amaze Servers | 1 Gbps guaranteed port with 30 TB/mo | Also sells a 10 Mbps unmetered configuration |
| ServerPacket | 1 Gbps unmetered, DDoS protection, one-hour setup | Server management +$39/mo |

A 50 TB monthly cap is about 15% of what a 1 Gbps port could move if it ran flat out; 30 TB is about 9%. If your forecast sits between 5 and 20 TB per month, a 1 Gbps port with a 30–50 TB allowance leaves real headroom. Cross into four figures of terabytes and the port itself becomes the bottleneck, at which point 10 Gbps is the conversation, not a bigger traffic bundle.

The other thing the port number does not tell you is contention. A dedicated port means a neighbouring tenant's traffic spike does not eat into your throughput, which is the practical difference between this and a shared uplink when your peak hour arrives.

One warning that applies to any provider's product list: the marketing name of a line is not a guarantee for every row inside it. Amaze Servers sells a 10 Mbps unmetered plan alongside its 1 Gbps guaranteed plans. Check the port field on the specific configuration you are buying. All four Ava listings state 1 Gbps individually, which is the right way round.

## Metered vs unmetered: what actually changes on the invoice

noushost splits its catalogue into two lines, "1Gbps Metered" and "1Gbps Unmetered". The hardware is comparable; the billing model is the product. On a metered plan you buy a monthly volume and pay for what you exceed. On an unmetered plan the volume stops being a line item.

"Unmetered" is not a synonym for "unlimited", and the difference shows up in the fine print. HOSTKEY's own traffic policy states that servers ship with a 1–10 Gbps port, incoming traffic is free under fair usage, and the outgoing traffic limit and rate depend on the traffic plan you select. So an unmetered headline can sit on top of per-plan outbound accounting. HOSTKEY says directly that unlimited bandwidth does not exist in server hosting, that the data rate always has a ceiling, and that CPU, RAM, and storage cap throughput regardless of what the port can theoretically do.

ServerPacket's rule of thumb is worth borrowing: unmetered pays off if you are already absorbing monthly overage charges, or if you expect to move more than 1,000 TB in a month. Below that, a metered plan with a generous allowance is usually cheaper per TB.

Ava does not use either label. The dedicated page states "Port Speed: 1 Gbps" and stops there. A third-party review page lists monthly traffic of 2 TB and 5 TB against two Ava dedicated plans whose names and prices do not match the official lineup, so that figure is not something to size capacity on. Ask sales, in writing, for four things: the monthly traffic allowance, the overage rate per TB, whether inbound traffic counts, and whether the allowance resets on the billing date or the calendar month.

👉 [See how each Ava plan is configured on the order page](https://my.ava.hosting/aff.php?aff=15562)

## Costs that sit outside the sticker price

The sticker is a starting point. Ava prices memory and disk as options on three of the four plans, and lists "optional add-ons" on all four without quoting them on the product page.

Other providers' published add-on rates give you a sense of the scale. noushost charges $11.99/mo to step up to 8 GB DDR4, $20.99 for 16 GB, $40.99 for 32 GB, $59.99 for 48 GB, and $79.99 for 64 GB. Windows Server licences run $20.00/mo; CloudLinux is $18.00/mo. ServerPacket charges $39/mo for managed service on top of an unmanaged server.

Do the arithmetic before you choose a plan. Moving from 16 GB to 64 GB of RAM costs more per month than the gap between Ava's cheapest and most expensive dedicated plans. A Windows licence plus a control panel can add $38/mo or more, which is 40% of the entry plan's price. Price the configuration you actually need and compare that number, not the "from" figure.

There is also a jurisdiction premium worth naming. Ava's entry box at USD 95.32/mo is roughly double noushost's $45.80/mo for a comparable 16 GB machine. You are not buying cheaper hardware; you are buying a Moldovan data centre and the legal position that comes with it. If jurisdiction is irrelevant to your project, that premium buys you nothing.

👉 [Price out the Ryzen 5 4650G configuration](https://my.ava.hosting/aff.php?aff=15562)

## Which of the four boxes fits your workload

**AMD Ryzen 5 4650G, USD 95.32/mo.** Newer architecture with strong single-thread performance and 6 cores / 12 threads. Game servers, single-thread-bound PHP or Laravel applications, small databases, and anything that cares more about clock speed than core count. The 16 GB base RAM is the tightest starting point in the lineup, so budget for an upgrade if you run a database and a web stack on the same box.

**2x Intel Xeon E5-2680 v2, USD 111.02/mo.** 20 cores / 40 threads and a fixed 256 GB of DDR3, plus 8 × 600 GB SAS drives for 4.8 TB raw. This is the cheapest way to buy memory density, which suits container fleets, build caches, in-memory datasets, and backup targets. The trade-off is a decade-old platform on spinning disks: fine for capacity and parallelism, poor for random I/O.

**2x Intel Xeon E5-2620 v3, USD 134.57/mo.** 12 cores / 24 threads on DDR4 with SSD storage, both configurable. The general-purpose pick for a web application, API, or database that needs predictable disk latency more than raw core count.

**2x Intel Xeon E5-2699 v3, USD 167.09/mo.** 36 cores / 72 threads. Virtualization hosts, CI runners, transcoding, and batch processing. Only worth the extra USD 32.52 over the E5-2620 v3 if you can keep that many threads busy; a single WordPress site will not notice the difference.

The order page runs a live stock counter per plan. At the time of writing the Ryzen listing showed zero units available and the dual E5-2680 v2 showed one. Check the counter before you schedule a migration window, because a sold-out plan means waiting rather than provisioning.

## The network and jurisdiction behind the port

Ava is headquartered in Chisinau, Moldova, and markets itself as an offshore, DMCA-tolerant provider. The facility is a hardened underground data centre with 24/7 physical security, roughly 50 Gbit/s of network capacity, about 1.6 MW of power with generator backup, and very large DDoS mitigation capacity. Billing accepts cryptocurrency alongside conventional methods. The stack runs NVMe storage with LiteSpeed on the shared side.

A third-party review published in 2026 measured a 573 ms time to first byte from a US-East testing location against a stated 600 ms industry average, and reported 99.99% uptime over 30 days. Treat those as one reviewer's numbers rather than a benchmark. User comments on the same page are mixed: several complain about slow ticket responses and inconsistent load times, and one describes the control panel as clunky. A 99.9% uptime SLA is what the provider advertises.

Geography matters more than usual here. Ava runs a single region. European visitors get low latency; US West Coast and Asian visitors get noticeably more. If your audience is mostly North American, a provider with a US presence will beat this on round-trip time regardless of port speed.

Offshore hosting decides which jurisdiction's content and privacy rules apply to the server. It does not change your obligation to follow the law in the country where you operate or where your customers are. Choose it for privacy and jurisdiction, and host lawfully.

## FAQ

**Is unmetered really unlimited?**
No. HOSTKEY states plainly that unlimited bandwidth does not exist in hosting, and that every server has a finite data rate. An unmetered plan removes the monthly volume meter; the port speed, CPU, RAM, and disk still cap what you can actually push.

**How much traffic can a 1 Gbps port move in a month?**
About 324 TB if it runs at full rate for 30 days. Real traffic never looks like that: averages sit far below peak, so plan on the monthly allowance rather than the port number. A 30–50 TB allowance covers most sites and applications comfortably.

**Should I skip 1 Gbps and go straight to 10 Gbps?**
Only if you expect sustained high concurrency or four-figure monthly terabytes. ServerPacket's guidance points at 10, 20, or 40 Gbps for projects above roughly 1,000 TB per month or with heavy concurrent transfer needs. Below 30 TB, the port is not your constraint.

**How long does Ava take to provision a server?**
The product page does not state a provisioning time, and the stock counters suggest some configurations ship from available inventory while others may not. Ask before you commit to a cutover date. For reference, ServerPacket advertises one-hour setup, so sub-day provisioning is normal in this market.

**Is management included?**
Ava lists 24/7 support and optional add-ons on every plan without separating self-managed support from hands-on administration. ServerPacket charges $39/mo for the managed layer, which is a reasonable benchmark for what that service costs elsewhere. Confirm what is covered before you assume the operating system, panel, and security patching are handled.

## Before you order

Match the plan to the bottleneck rather than the price list. Single-threaded application or game server: Ryzen 5 4650G. Memory-hungry container host on a budget: dual E5-2680 v2. General web, API, or database: dual E5-2620 v3. Heavy virtualization or batch compute: dual E5-2699 v3.

Then confirm three things in writing before paying: the monthly traffic allowance and the overage rate per TB, whether inbound traffic counts against it, and whether DDoS protection and the IPv4 address are included at no extra cost on the configuration you selected. Add the cost of any RAM, disk, Windows licence, or control panel upgrade to the monthly figure before you compare it with anything else.

👉 [Compare the four Ava Hosting 1Gbps dedicated servers](https://my.ava.hosting/aff.php?aff=15562)
