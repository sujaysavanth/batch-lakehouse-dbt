    # Batch Lakehouse + dbt

    ![status](https://img.shields.io/badge/status-WIP-blue)

    Airflow-orchestrated batch ELT over public GitHub-events data (GH Archive): raw -> staging -> marts with incremental dbt models, tests, and generated docs.

    **Stack:** Airflow, dbt, BigQuery, Python

    ## Architecture

    ```
    GH Archive -> [extract] -> raw (BigQuery)
Airflow DAG schedules incremental runs
dbt: raw -> staging -> marts (+ tests + docs)
    ```

    ## Getting started

    ```bash
    # see setup steps below
    ```

    ## Roadmap

    - [ ] Extract GH Archive to raw
- [ ] Airflow schedule
- [ ] Incremental dbt models
- [ ] Tests + generated docs
- [ ] Watermark for late partitions

    ## Notes

    Built on public data — fully reproducible. Honest scope: this README reflects
    what is planned vs. built. Sections marked (WIP) are in progress.

    ---
    Sujay Govindappa Rajashekar · [github.com/sujaysavanth](https://github.com/sujaysavanth)
