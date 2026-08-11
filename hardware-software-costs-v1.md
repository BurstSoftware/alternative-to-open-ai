# how much does it cost to maintain the hardware and the software

A lot. And the important thing is that “maintenance” is only part of the cost. For an organization operating at OpenAI's scale, there are really three buckets:

Capital costs — buying/building GPUs, servers, data centers, networking, power systems.
Operating costs — electricity, cooling, repairs, cloud rentals, replacement hardware, networking.
Software + people — engineers, researchers, model training, security, databases, monitoring, etc.

OpenAI doesn't publicly disclose a clean line-by-line annual maintenance bill, so exact numbers aren't available. But its infrastructure commitments give us a sense of the scale.

Hardware

The hardware itself is enormous.

OpenAI announced a $38 billion AWS commitment providing hundreds of thousands of NVIDIA GPUs and the ability to scale to tens of millions of CPUs.

It is also expanding its own Stargate infrastructure. OpenAI says it had surpassed 10 GW of AI infrastructure commitments by April 2026.

And reported infrastructure spending commitments have become extraordinary: TechCrunch reported in July 2026 that OpenAI's planned infrastructure spending through 2030 had reached roughly $750 billion. That's a future infrastructure spending commitment, not an annual maintenance bill.

What does it cost to keep a GPU cluster running?

Imagine you have a hypothetical $1 billion AI data center.

You have to continuously pay for:

Cost	What you're paying for
Electricity	GPUs + CPUs + networking
Cooling	Moving all that heat out
Networking	Fiber, switches, transceivers
Hardware replacement	Failed/obsolete GPUs, memory, SSDs, etc.
Data center	Building, rent, security, facilities
Cloud/infrastructure	If capacity is rented
Software	Engineering, licenses, infrastructure systems
People	Engineers, researchers, operations, security
Backup/redundancy	Spare capacity and disaster recovery

The electricity alone can be enormous.

For example, a 1-GW facility operating continuously consumes:

1 GW × 8,760 hours ≈ 8.76 billion kWh/year

At an illustrative electricity price of $0.07/kWh, that's about:

$613 million/year in electricity.

And that's just electricity—not GPUs, buildings, cooling equipment, employees, networking, etc.

But there's an important catch

OpenAI doesn't necessarily own all the hardware it's using.

This is crucial.

Some infrastructure is effectively:

OpenAI → pays cloud/infrastructure provider → provider owns/operates data center and hardware.

Other infrastructure involves OpenAI's partners building capacity specifically for its workloads.

That's why saying “OpenAI's hardware maintenance bill is $X” would be misleading.

Microsoft, for example, has reportedly spent more than $100 billion on its broader OpenAI partnership, including infrastructure and data centers, according to testimony reported by The Information.

OpenAI also says Microsoft remains its primary cloud partner, while OpenAI now has flexibility to use other cloud providers.

Software is actually a different kind of expense

Software doesn't wear out like a GPU.

You don't have to replace a copy of the inference software every three years.

Instead, the costs are primarily:

people + computing + development + operations.

For example, OpenAI needs teams working on:

model architecture
inference optimization
distributed computing
GPU kernels
databases
networking
security
reliability
APIs
ChatGPT
mobile/web applications
monitoring
internal developer tools
safety systems
evaluation
billing
authentication

And software itself requires hardware to run.

So you can have a beautifully optimized inference system, but if millions of users are asking questions simultaneously, you're still paying for the GPUs performing the computation.

The biggest recurring expense may actually be inference

This is the fascinating part.

Every time you ask ChatGPT something, the model has to perform computation to generate the response.

If you ask:

"Write me a 10-page report."

you're consuming substantially more compute than:

"What's 2+2?"

And if millions of people do that continuously, the compute bill becomes enormous.

There have been reports based on leaked/documentary financial information that OpenAI's Azure inference spending alone reached billions of dollars. Those figures aren't official OpenAI financial statements, so I'd treat them as estimates/reporting rather than definitive numbers.

The economics therefore look something like:

                 CUSTOMER
                    │
                 $20/mo
                    │
                    ▼
              ┌───────────┐
              │  OpenAI   │
              └─────┬─────┘
                    │
          ┌─────────┼─────────┐
          ▼         ▼         ▼
       Compute   Employees   Other
          │
     ┌────┴────┐
     ▼         ▼
   GPUs      Power
     │
     ▼
  Cooling
     │
     ▼
  Networking

And compute is consumed every single time the customer uses the product.

Why AI companies need so much money

There's a subtle difference between normal software and AI.

For a normal SaaS company:

Build software once → distribute another copy for almost zero marginal cost.

For AI:

Build model → then pay for computation every time someone uses it.

That's why scaling ChatGPT from 10 million users to 100 million users isn't simply a matter of adding database servers.

You potentially need vastly more AI compute capacity.

And that's why OpenAI's infrastructure strategy is so aggressive: OpenAI explicitly describes compute as the critical input for training models, serving them reliably, improving performance and lowering costs over time.

A useful way to think about it

If you wanted to build a competing AI company, your expenses would roughly become:

Year 0–2:

💰 Build/buy enormous compute
💰 Train models
💰 Hire researchers/engineers

After launch:

💰 GPUs/cloud
💰 Electricity
💰 Cooling
💰 Hardware depreciation
💰 Software engineering
💰 Employees
💰 Security/reliability
💰 Inference for every customer

And then you have to charge customers enough that:

Revenue > inference + infrastructure + employees + everything else

That's one of the central economic challenges of frontier AI.

If you'd like, I can next 
build a realistic hypothetical $1-billion AI data center and break down exactly where the $1 billion goes—GPUs, servers, networking, building, electricity, cooling, and annual operating cost.
