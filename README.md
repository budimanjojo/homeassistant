<div align="center">

### My Home Assistant Configurations :house:

</div>

## :book:&nbsp; Overview

This repository contains my Home Assistant configuration files. I deploy Home Assistant using Kubernetes which is managed by Flux [here](https://github.com/budimanjojo/home-cluster). Changes in this repository will be pushed into the Kubernetes PVC (planning to use some kind of git hook in the future).

---

## :lock_with_ink_pen:&nbsp; Secret management

[Secret file](./secrets.yaml) is encrypted using [SOPS](https://github.com/mozilla/sops) and will be decrypted before getting pushed into my Home Assistant container volume.

## Todo List

- [ ] Improve README
- [ ] Add git hook to auto push changes
- [ ] Include dashboard screenshots
