# CCDP-0003 Container provides API for health status monitoring


- [Release Signoff Checklist](#release-signoff-checklist)
- [Summary](#summary)
- [Motivation](#motivation)
  - [Goals](#goals)
  - [Non-Goals](#non-goals)
- [Proposal](#proposal)
  - [User Stories (Optional)](#user-stories-optional)
    - [Story 1](#story-1)
    - [Story 2](#story-2)
  - [Notes/Constraints/Caveats (Optional)](#notesconstraintscaveats-optional)
  - [References](#references)
  - [Alternatives (Optional)](#drawbacksalternatives)
- [Test Plan](#test-plan)
- [Scoring](#scoring)
- [Implementation History](#implementation-history)

## **Release Signoff Checklist**

Items marked with (R) are required for the proposed best practice to be included in a release.

- [ ] (R) CCDP approvers have approved the CCDP status as `implementable`
- [ ] (R) CCDP summary, motivation and best practice details are appropriately documented
- [ ] (R) Test plan is in place, giving consideration to CNF Test Suite input
- [ ] (R) Scoring has been determined
- [ ] "Implementation History" section is up-to-date
- [ ] Supporting documentation—e.g., additional design documents, links to mailing list discussions/SIG meetings, relevant PRs/issues, release notes

## **Summary**

The higher level best practice is the concept of letting the application creator tell the operator/orchestrator, everything about the application. That includes general health status. 

A generic API should be exposed providing health status information

## **Motivation**

Providing health status allows the application to coordinate with platform and leverage its automated capabilities such as recovery and scaling.

To allow easier integration and interoperability there needs to be an agreement on a generic API that can be exposed, such as what can be used by K8s readiness/liveness checks. 

### **Goals**

### **Non-Goals**

## **Proposal**

### **User Stories (Optional)**
#### **Story 1**
#### **Story 2**

### **Notes/Constraints/Caveats (Optional)**

### **References**

"Always define liveness and readiness probes in the pod definitions." from RedHat's [14 Best Practices for Developing Applications on OpenShift](https://www.openshift.com/blog/14-best-practices-for-developing-applications-on-openshift)


### **Alternatives (Optional)**


## **Test Plan**

Start with validating CNF has readiness and liveness check entries.


## **Scoring**
- Mandatory (yes/no):
- Passing score (eg. +5):
- Failing score (eg. -1):

_Note: CCDPs may have different priorities and importance leading to different scores_


## **Implementation History**
- Proof of Concept: Test for a liveness entry and a readiness entry in the helm chart [#72](https://github.com/cncf/cnf-conformance/issues/72)
- Configuration test: is there a liveness entry in the Helm chart? [#56](https://github.com/cncf/cnf-conformance/issues/56)
- Configuration test: is there a readiness entry in the Helm chart? [#57](https://github.com/cncf/cnf-conformance/issues/57)
