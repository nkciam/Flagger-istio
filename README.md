# Flagger-istio

[![e2e](https://github.com/seifrajhi/Flagger-istio/workflows/e2e/badge.svg)](https://github.com/seifrajhi/Flagger-istio/actions)
[![e2analyzee](https://github.com/seifrajhi/Flagger-istio/workflows/analyze/badge.svg)](https://github.com/seifrajhi/Flagger-istio/actions)
[![license](https://img.shields.io/github/license/seifrajhi/Flagger-istio.svg)](https://github.com/seifrajhi/Flagger-istio/blob/main/LICENSE)

This is a guide where you will get hands-on experience with GitOps and
Progressive Delivery using Kubernetes and Istio.

## Introduction

### What is GitOps?

GitOps is a way to do Continuous Delivery, it works by using Git as a source of truth
for declarative infrastructure and workloads.
For Kubernetes this means using `git push` instead of `kubectl apply/delete` or `helm install/upgrade`.

In this workshop you'll be using GitHub to host the config repository and [Flux](https://fluxcd.io)
as the GitOps delivery solution.

### What is Progressive Delivery?

Progressive delivery is an umbrella term for advanced deployment patterns like canaries, feature flags and A/B testing.
Progressive delivery techniques are used to reduce the risk of introducing a new software version in production
by giving app developers and SRE teams a fine-grained control over the blast radius.

In this workshop you'll be using [Flagger](https://flagger.app), Istio and Prometheus to automate
Canary Releases and A/B Testing for your applications.

![Progressive Delivery GitOps Pipeline](/docs/images/flux-flagger-gitops.png)
