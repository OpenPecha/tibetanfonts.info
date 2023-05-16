
# Resource allocation

## 1.1. Definitions

Each engineering stage describes the current phase of a product specification. There are three stages:

* Request for work (RFW)
* Request for comments (RFC)
* Work order (WO)

**Request for work** is a detailed product specification that the product department submits following a standard template. The shorthand is RFW.

**Request for comments** is a detailed engineering specification that the R&D department submits following a standard template, based on the underlying RFW. The shorthand is RFC.

**Work order** is the final stage before an engineering specification described in the underlying RFC becomes allocated in the next engineering cycle. The shorthand is WO.

**Work ID** identifies connections between various stages in the resource allocation process. The shorthand is WID.

**Engineering cycle** is a three-month period in which allocated WOs are fulfilled.

**Stream** is an internal resource allocation observability dashboard. 

## 1.2. Overview

The R&D department's resource allocation falls into four categories: 

* Work orders
* Issue resolution
* Maintenance and process automation
* Experiments

### 1.2.1 Work orders

In any given time window, the majority of available R&D resources are allocated based on product specifications making their way from an RFW to an RFC and reaching the WO stage. One hundred percent of material changes to OpenPecha solutions result from a given product specification reaching the WO stage. There are no other means to cause material changes to OpenPecha solutions. As outlined elsewhere, the R&D department depends on the product department for WOs.

### 1.2.2. Issue resolution

When issues arise and they warrant prompt unplanned action, these will be handled accordingly. Support channels are provided to notify the R&D Department of issues. There are two kinds of issues: 

* Regular issues
* Fires

#### 1.2.2.1. Regular issues

Regular issues are handled periodically through the standard resource allocation process described in this section. 

#### 1.2.2.2. Fires

Fires require immediate attention. There are three ratings for fires based on the severity of the issue: 

* 🔥🔥🔥 - Most severe: there's a critical or an imminent threat to the business
* 🔥🔥 - Moderate severity: there's a medium probability of an adverse effect on the business 
* 🔥 - Minor severity: there's a low probability of an adverse effect on business, but *fast action must be taken*

Examples:

- An interruption in business-critical services: 🔥🔥🔥
- A data integrity issue results: 🔥🔥
- An interruption in data collection results: 🔥🔥🔥
- An interruption in data integrity monitoring results: 🔥🔥🔥
- A data leak or other critical security issue results: 🔥🔥🔥
- An interruption limiting login access to OpenPecha solutions: 🔥🔥

Status updates for fires are available for fires through [https://status.openpecha.com](https://status.acme.com)

### 1.2.3. Maintenance and process automation

R&D resources are regularly allocated to various maintenance activities, as well as process automation-related activities. Process automation allocations mainly focus on improving system visibility and stability, reducing overall operational risks and costs, as well as removing dependency on humans. 

Maintenance and process automation priorities are expressed in individual production repositories and the Housekeeping repository in an issue titled “Non-Request Priorities,” each repository having its own issue with this title.

### 1.2.4. Experiments

R&D department resources are occasionally allocated to experimenting with new technologies and methods, such as delivery mechanisms, data stores, and other approaches that support the scope of R&D responsibilities.

## 1.3. Engineering cycle

The engineering cycle follows “tik-tok-tik-tok…” model, where each “tik” involves a major fulfillment of something new, and each “tok” focuses on improving what has been previously fulfilled. Each cycle lasts three months, following the quarterly calendar. For example, if Q1/2023 is “tok” and focuses on improving previous fulfillments, Q2/2023 will be “tik” focused on fulfilling a new, or otherwise major thing. 

## 1.4. Process outline

### 1.4.1. Request process

1. An RFW is submitted on GitHub (by the product department)
2. The RFW is evaluated and various communications may take place
3. An RFC is created with a corresponding WID
4. The RFC is evaluated and various communications take place (by the product department)

> **Note**: Any changes that result in the evaluation process and various related communications are recorded in the request only if it changes the specification. The purpose of RFWs and RFCs are to be a self-contained record of specification and its evolution, not a record of various related communications. 

### 1.4.2. Work order process

5. Work is mutually agreed on (by Product & R&D)
6. There is a seven-day cooling period, during which nothing happens
7. The specification becomes a WO that is sealed to prevent any alteration
8. The WO becomes visible with stage labeling in Stream

> **Note**: Changes beyond the 5th step should be used sparingly. For most requests, they should never happen. They are there as a fail-safe to avoid serious negative consequences resulting from negligence in the earlier steps of the process. 

### 1.5. Timing

Estimating how long a given WO takes to fulfill is difficult, and ample time should be reserved for all engineering work. This is especially true for requests that have a large scope or include new kinds of work. 

> **Note**: The total throughput of the R&D department can be accelerated by investing in more resources (people) for future WOs, but not outstanding ones. Total throughput can't be accelerated by making more RFWs. This is important to understand.

RFWs for the next engineering cycle must be submitted at least 45 days before the start of the cycle. For example, any RFWs that arrive before the 15th of November 2023, will be processed as fulfillment candidates for the Q1/2024 engineering cycle.

## 1.6. Quality assessment

The efficiency of resource allocation in the R&D department can be objectively evaluated through quality assessment. This is mainly done through the evaluation of two aspects:

* Specification fulfillment rate (%)
* Defect rate (#)

### 1.6.1. Specification fulfillment rate

This can be understood as the overlap between the agreed-up specification and the completed work. 

### 1.6.2. Defect rate

This can be understood in two ways: the number of fulfilled WOs with defects and the total number of defects per WO. 
