
# Observability

The observability of R&D resource allocations can be understood through units of work called **commits**. Commits are the footprint of the actual work, made at least once a day to origin/remote by each developer, and represent everything that has been produced.

One or more commits make up a **pull request**, which is a material change to the codebase and goes through various quality control and other procedures.

**Pull requests** make up completed **work orders**, which are the fulfilled specifications received from the product team. 

The **engineering cycle** is made up of work orders. The engineering cycle consists of the works described in the [resource allocation](org/resource-allocation) article. 

## Observation horizons

Several observation horizons are provided for observability of resource allocation in R&D. The horizons differ mainly in terms of time-from yearly to daily, and in the granularity that each horizon provides-from rough to highly granular.

The five observation horizons, from broadest to most specific:

* Roadmap
* Engineering cycle
* Word order
* Pull request
* Commit

### Roadmap

The **roadmap horizon** provides an annual view of resource allocation. The level of granularity is rough, for example, “solution implementation to support strategic objective.”

The product team maintains the product roadmap.

### Engineering cycle

The **engineering cycle horizon** provides a quarterly view of resource allocation. Its granularity is somewhat more refined than roadmap horizon i.e., engineer cycle items may be further broken down into work orders.

The engineering cycle horizon is visible on Stream. Moreover, canonical information about related work orders is available in the corresponding RFWs and RFCs.

### Work order

The time window of the **work order horizon** depends on the particular work order. But generally speaking, the horizon provides a month-to-month view of resource allocation. The level of granularity is somewhat more refined than engineering cycle horizon i.e. work order items may be further broken down into pull requests.

The work order horizon is visible on Stream. Moreover, canonical information about related work orders is available in the corresponding RFWs and RFCs.

### Pull request

The time window of the **pull request horizon** represents depends on the particular pull request. But generally speaking, the horizon provides a week-to-week view into resource allocation. The level of granularity is somewhat more refined than work order horizon, i.e., pull request items may be further broken down into commits.

The pull request horizon is visible on Stream. Moreover, canonical information about related work orders is available in the corresponding RFWs and RFCs.

### Commit

The **commit horizon** represents a daily time horizon. Developers commit code at least once per day on the work orders they are working on. The level of granularity is the highest attainable. Commit items may be further broken down into their actual contents, i.e., the material code contributions associated with the commit.

The commit horizon is visible on Stream. In addition, canonical information about related work orders is available in the corresponding RFWs and RFCs.
