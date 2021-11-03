<div align="center">

### My Home Assistant Configurations :house:

</div>

## :book:&nbsp; Overview

This repository contains my Home Assistant configuration files. I deploy Home Assistant using Kubernetes which is managed by Flux [here](https://github.com/budimanjojo/home-cluster). Changes in this repository will be pushed to my Home Assistant container using [this automation](./automation/update_config.yaml).

---

## :lock_with_ink_pen:&nbsp; Secret management

Secrets are environment variable that is deployed from my Flux managed Kubernetes cluster that you can look at [here](https://github.com/budimanjojo/home-cluster/blob/main/cluster/apps/homeassistant/secret.yaml).

[Secret file](./secrets.yaml) is encrypted using [SOPS](https://github.com/mozilla/sops) and will be decrypted before getting pushed into my Home Assistant container volume.

---

## :handshake:&nbsp; Thanks

Special thanks for [alex](https://github.com/alexwaibal) for the tips for pushing repository into HAss container.

---

## Todo List

- [ ] Improve README
- [ ] Include dashboard screenshots
