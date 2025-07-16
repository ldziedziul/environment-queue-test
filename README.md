# environment-queue-test

This repository demonstrates that using the same `environment` key in GitHub Actions enforces **FIFO serial execution across multiple workflows**, effectively forming a queue.

Trigger multiple `workflow_dispatch` runs manually. Each will wait for the previous run to finish before starting.
