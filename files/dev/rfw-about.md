
# What is an RFW?

* RFW stands for **request for work**. 
* An RFW is a detailed product specification that the product department submits to developers following a standard template. 
* It is filled by all the stakeholders in a meeting. 
* It focuses on *what* developers should make and *why*.

## Minimum amount of work for an RFW

If you expect a task to take more than four hours to complete, it needs an RFW. Bundle smaller tasks into a single thematically consistent RFW. Thematic consistency refers to how the specifications can be fulfilled by an engineer by working on one part of the system. Generally, specifications for different parts of the system get their own RFWs.

## Two types of RFWS

There are two acceptable types of RFWs: 

- **Type-A**: re-arranges or extends something already built
- **Type-B**: creates something new

Mixing the two types of RFWs is prohibited, and RFWs that mix the two types will be rejected. RFWs of different types are also not allowed to depend on each other, as that would be like an RFW that mixes the two types.

A simple way to think about both types of RFWs is that they have to be self-sustained. Before an RFW is moved to an RFC, it must stand on its own without another request being fulfilled.

A type-B RFW can't introduce two new things that are conceptually new but different. Such an RFW should be separated into two RFWs, where the first one doesn't have any dependencies—functional, conceptual, or otherwise–on the second one.

RFWs must focus on either the frontend or backend—not on both. When a new product specification requires major changes to both the frontend and backend, separate RFWs should be made for the frontend and backend. In that case, the frontend-focused RFW shouldn't be submitted until after the RFCs for the underlying non-frontend RFWs have been processed.
