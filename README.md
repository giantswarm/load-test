[![CircleCI](https://circleci.com/gh/giantswarm/load-test.svg?style=svg)](https://circleci.com/gh/giantswarm/load-test)

# load-test

A collection of resources for load testing Kubernetes clusters.

## Locust

- [locust](https://locust.io/) is a load testing tool written in Python.
- Create 2 tenant clusters for the test workload and locust.
- Install the locust chart.

```
helm install -n locust charts/locust --set baseDomain=[base domain for locust cluster] --set target.address=[target workload]
```
