---
marp: true
---

<!-- 
theme: gaia 
class: invert
-->

# dbt Testing the Easy Way

A discussion on dbt test generation

---

# Introduction
- Kevin McQuate - Data Engineer
- Specialize in Python, Spark, Terraform
  
---

# Data Quality __Matters__

- [The Annual State of Data Quality Survey](https://resources.montecarlodata.com/c/data-quality-survey-1?x=fP0c5d&__hstc=100283906.4d5bbc655bb2d063b3073552b52afbe0.1707330646540.1707330646540.1707330646540.1&__hssc=100283906.1.1707330646540&__hsfp=3295665591&_gl=1*2cdxsf*_ga*NTQ1NDUzNjY4LjE3MDczMzA2NDY.*_ga_SZGJ8KW5Z8*MTcwNzMzMDY0NS4xLjAuMTcwNzMzMDY0NS42MC4wLjA.&_ga=2.232933662.1223611414.1707330646-545453668.1707330646#page=1)
  - Commissioned by Monte Carlo
  - "166% increase in the average time to resolution" since last year
  - "Unity Technologies cited a $110M decrease in their yearly revenue"

- Automated tests
  - Reduce manual QA work
  - Validate migrations

---
# Data *Observability*
- Products:
  - ![width:200px ](https://www.montecarlodata.com/wp-content/uploads/2023/06/mc-logo.svg)

  - ![width:200px ](https://imgix.datadoghq.com/img/dd_logos/png_logos/horizontal/dd_logo_h_white.png)

- Proactive vs. Reactive
  - Fail-fast principle

---
# Why are we not writing tests?
- Time
- Effort
- Culture
- Assumption of Consistency
  - Robustness principle - "be conservative in what you send, be liberal in what you accept"
  - At scale, failure rates increase


---
# dbt-testgen
- dbt package
- https://github.com/kgmcquate/dbt-testgen
- Generates YAML for tests based on dbt model statistics
- Available on dbt Hub or and GitHub
    - https://github.com/kgmcquate/dbt-testgen
    - https://hub.getdbt.com/kgmcquate/testgen/latest/

---
# Demo

---
# Development
- Jinja vs. Python
  - dbt Cloud
- Integration Testing
  - 6 different DBs


---
# Future Features
- More tests
- CLI interface
- Interactive Web interface
- Suggestions, GitHub issues, and PRs welcomed