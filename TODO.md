# TODO

This file lists the things we'd like to get done.  Some of it is stuff we're working on and some of it is stuff anyone in the community could help with.

## Minor Fixes
* Spelling, grammar, review
* Containers Work in Progress and Known Issues pages
  * Add exact error messages for more searchable resolution to issues.

## Articles to edit/revise
* Hyper-V on Windows [remote host management article](./virtualization/hyperv_on_windows/user_guide/remote_host_management.md)

## Articles to add

## Web App Performance Review Playbook (Taste Match style projects)
* Add a repeatable profiling baseline in the repo:
  * Run bundle analysis on each release candidate.
  * Track Core Web Vitals (LCP, INP, CLS) before and after optimization.
* Reduce first-load JavaScript:
  * Lazy-load route-level pages and heavy optional features.
  * Keep manual chunking in Vite and validate chunk boundaries after each new dependency.
* Audit frontend dependencies quarterly:
  * Remove unused UI/animation/chart libraries.
  * Deduplicate overlapping packages and keep a single package manager lockfile strategy.
* Optimize data fetching:
  * Configure React Query defaults (`staleTime`, `gcTime`, retry rules) per endpoint class.
  * Prevent duplicated queries via stable query keys and shared hooks.
  * Fetch only required fields and paginate large lists.
* Reduce render work:
  * Measure component re-render hotspots with React Profiler.
  * Memoize expensive derived data and virtualize large lists.
  * Gate non-critical animations on reduced-motion preference and device constraints.
* Add performance gates to CI:
  * Fail PRs when bundle-size budgets are exceeded.
  * Include a lightweight Lighthouse or Web Vitals regression check in preview builds.
* README for all Container samples and tools
* README for all Hyper-V samples and tools
