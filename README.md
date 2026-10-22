<p align="center">
  <img src="assets/header.svg" alt="beladjioo — platform engineer jacked into bare-metal Kubernetes" width="100%">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/status-online-00f0ff?style=for-the-badge&labelColor=0a0a12" alt="status: online">
  <img src="https://img.shields.io/badge/cloud-none-ff2a6d?style=for-the-badge&labelColor=0a0a12" alt="cloud: none">
  <img src="https://img.shields.io/badge/lock--in-zero-fcee0a?style=for-the-badge&labelColor=0a0a12" alt="lock-in: zero">
  <img src="https://img.shields.io/badge/drift-0-b967ff?style=for-the-badge&labelColor=0a0a12" alt="drift: 0">
</p>

## `0x00` BOOT

```console
$ whoami
netrunner // senior devops & platform infrastructure

$ cat /etc/manifesto
> i build the infrastructure cities run on.
> bare metal. kubernetes. gitops. open source end to end.
> no hyperscaler. no proprietary lock-in. no manual changes.
> if it isn't in git, it doesn't exist.
```

## `0x01` MEGACITY GRID

```text
╔══[ SMART CITY // LIVE ]══════════════════════════════════╗
║                                                          ║
║  SECTOR    Montpellier Méditerranée Métropole            ║
║  CITIZENS  500,000+                                      ║
║  SENSORS   100,000+ IoT nodes                            ║
║  FEEDS     air · waste · water · energy · mobility       ║
║  CLUSTERS  4 × Kubernetes, reconciled from Git           ║
║  INFRA     100% owned · zero hyperscaler                 ║
║                                                          ║
╚════════════════════════════════════[ SYNCED · HEALTHY ]══╝
```

## `0x02` THE PIPE

```mermaid
%%{init: {'theme': 'base', 'themeVariables': {'fontFamily': 'monospace'}}}%%
flowchart LR
    A(["git push"]) ==> B["CI ▸ tests · build · scan · SBOM"]
    B ==> C[("registry ▸ immutable · signed")]
    C ==> D{{"Argo CD ▸ auto-sync"}}
    D ==> E["bare-metal k8s ▸ owned · sovereign · observable"]
    classDef cyan fill:#0a0a12,stroke:#00f0ff,stroke-width:2px,color:#00f0ff
    classDef mag fill:#0a0a12,stroke:#ff2a6d,stroke-width:2px,color:#ff2a6d
    classDef yel fill:#0a0a12,stroke:#fcee0a,stroke-width:2px,color:#fcee0a
    classDef pur fill:#0a0a12,stroke:#b967ff,stroke-width:2px,color:#b967ff
    class A,E cyan
    class B mag
    class C yel
    class D pur
    linkStyle default stroke:#ff2a6d,stroke-width:2px
```

## `0x03` LOADOUT

<p>
  <img src="https://img.shields.io/badge/kubernetes-0a0a12?style=for-the-badge&logo=kubernetes&logoColor=00f0ff" alt="Kubernetes">
  <img src="https://img.shields.io/badge/argo_cd-0a0a12?style=for-the-badge&logo=argo&logoColor=ff2a6d" alt="Argo CD">
  <img src="https://img.shields.io/badge/cilium_%C2%B7_ebpf-0a0a12?style=for-the-badge&logo=cilium&logoColor=fcee0a" alt="Cilium eBPF">
  <img src="https://img.shields.io/badge/rook--ceph-0a0a12?style=for-the-badge&logo=ceph&logoColor=b967ff" alt="Rook-Ceph">
  <img src="https://img.shields.io/badge/opentofu-0a0a12?style=for-the-badge&logo=opentofu&logoColor=fcee0a" alt="OpenTofu">
  <img src="https://img.shields.io/badge/grafana-0a0a12?style=for-the-badge&logo=grafana&logoColor=ff2a6d" alt="Grafana">
  <img src="https://img.shields.io/badge/python-0a0a12?style=for-the-badge&logo=python&logoColor=00f0ff" alt="Python">
  <img src="https://img.shields.io/badge/rust-0a0a12?style=for-the-badge&logo=rust&logoColor=ff2a6d" alt="Rust">
  <img src="https://img.shields.io/badge/linux-0a0a12?style=for-the-badge&logo=linux&logoColor=fcee0a" alt="Linux">
</p>

```yaml
loadout:
  platform:      [kubernetes, rke2, rancher, metallb, rook-ceph, cilium/ebpf, envoy-gateway, helm]
  gitops_iac:    [argo-cd, gitlab-ci, opentofu, terraform, ansible]
  iot_rf:        [lorawan at scale, rf planning, vlan segmentation, fleet provisioning, ota]
  observability: [mimir, loki, grafana, alloy, zabbix]
  languages:     [python/django, rust, bash]
  r_and_d:       [computer vision/yolo, gpu scheduling, kubeflow]
```

## `0x04` HOME RIG

```yaml
rig:  # where the grid gets rehearsed
  cluster:  k3s on arm64
  gpu:      nvidia jetson, cuda
  delivery: ci → ghcr, sha-pinned → argo cd auto-sync
  secrets:  sealed, never in git
  rule:     nobody runs kubectl apply by hand
```

## `0x05` OPEN SOURCE DROPS

| node | signal |
|---|---|
| [**OpenHertz / Spectra**](https://github.com/beladjioo/Spectra) | learn radio with a real SDR — all-Rust DSP, live demod in the browser, ADS-B, LoRa, ham-radio exam prep · [openhertz.org](https://openhertz.org) |
| [**chirpstack-v4-kubernetes**](https://github.com/beladjioo/chirpstack-v4-kubernetes) | ChirpStack v4 LoRaWAN network server on Kubernetes |
| [**FineTuneForge**](https://github.com/beladjioo/FineTuneForge) | fine-tune a small open model (1B–7B) on your own data with LoRA, ship it to Hugging Face |
| [**robotique**](https://github.com/beladjioo/robotique) | robotics monorepo — manipulators, navigation, EKF, drones, swarms, RL, ROS 2 |

## `0x06` CERTS

```text
[ CKA ]  Certified Kubernetes Administrator  ::  in progress · 2026 · CNCF
```

## `0x07` UPLINK

<p>
  <a href="https://belhadj.dev"><img src="https://img.shields.io/badge/%E2%96%B8_uplink-web-00f0ff?style=for-the-badge&labelColor=0a0a12" alt="web"></a>
  <a href="mailto:contact@belhadj.dev"><img src="https://img.shields.io/badge/%E2%96%B8_signal-mail-ff2a6d?style=for-the-badge&labelColor=0a0a12" alt="mail"></a>
</p>

<p align="center"><sub>░▒▓ end of transmission ▓▒░</sub></p>
