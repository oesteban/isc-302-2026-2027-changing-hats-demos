# 302 · Changing hats demos · 2026-2027

The sixteen demos built for the *changing hats* presentations of HES-SO
Valais-Wallis module *302 Data Computation* (data pipelines block, weeks 1 to 3):
you draw a topic, you build a demo, you teach it.

Each directory is a git submodule pointing at the repository its presenter
published, pinned at the commit that was current on 29 September 2026. How to
run a demo is in that demo's own README.

## Get the demos

```bash
git clone --recurse-submodules https://github.com/oesteban/isc-302-2026-2027-changing-hats-demos.git
```

If you already cloned without `--recurse-submodules`:

```bash
git submodule update --init                          # all sixteen
git submodule update --init 12-parquet-internals     # just one
```

To pick up commits a presenter pushed after the pin:

```bash
git submodule update --remote 12-parquet-internals
```

## The demos

| # | Topic | Directory |
|---|---|---|
| 01 | Containers vs. VMs | [`01-containers-vs-vms`](https://github.com/Algath/Container-vs-VMs) |
| 02 | Building containers (with Docker) | [`02-building-containers-docker`](https://github.com/ffavre13/building-containers-demo) |
| 03 | Automating image building with CI/CD | [`03-ci-cd-image-builds`](https://github.com/Dav0105/docker-ci-cd) |
| 04 | From Docker Compose to Kubernetes | [`04-compose-to-kubernetes`](https://github.com/val-mon/k8s-demo) |
| 05 | K8s, MicroK8s, K3s, minikube: container orchestration | [`05-k8s-k3s-microk8s-minikube`](https://github.com/FlorianHESWALLIS/k8s-distros-demo) |
| 06 | Data streams with Kafka | [`06-kafka-data-streams`](https://github.com/g-ae/kafka-presentation-demo) |
| 07 | Packaging Kubernetes apps with Helm | [`07-helm-packaging`](https://github.com/Vchobu/302-demo) |
| 08 | Container security: what isolation does not give you | [`08-container-security`](https://github.com/AlexisKueny/container-security-class) |
| 09 | Caching and typed interfaces in Flyte | [`09-flyte-caching-typed-interfaces`](https://github.com/Sebastian0211-vs/Flyte_Caching) |
| 10 | Retries and idempotence: what happens after a task fails | [`10-retries-idempotence`](https://github.com/rdtjulien/302-Retries-and-idempotence) |
| 11 | Slurm and Kubernetes, two ways to schedule work | [`11-slurm-vs-kubernetes`](https://github.com/Zoatik/Slurm-and-Kubernetes) |
| 12 | Inside a Parquet file | [`12-parquet-internals`](https://github.com/NatXiao/Demo-Parquet-presentation) |
| 13 | Partitioning and the small-files problem | [`13-partitioning-small-files`](https://github.com/Neb5384/partitioning) |
| 14 | Table formats and the lakehouse | [`14-table-formats-lakehouse`](https://github.com/Dyumes/TableFormatsAndTheLakehouse) |
| 15 | Object stores versus file systems | [`15-object-stores-vs-filesystems`](https://github.com/Discretos2022/Filesystem-vs-object-store) |
| 16 | DataFrames with pandas, Polars and Arrow | [`16-pandas-polars-arrow`](https://github.com/grey-park/pandas-Polars-Arrow) |

## When a demo does not run on your machine

The demos were built on their presenters' laptops, so a path, a version or an
architecture may need adapting. Open an issue or a pull request on the
presenter's repository (the links above), not here: this repository only
records which commit of each demo is current.
