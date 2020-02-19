# squash-setups-kubernetes
[Squash instanciations with kubernetes]

Squash with h2 DB:

  - squash-h2.yml
  
---  
  
Squash with postgres:

  - squash-pg.yml

---

Squash with postgres using deployment and not pods:
(it will re-instance once they stopped or being stopped)

  - deploy-squash.yml
  
  squash service is in another file to be able to root users during maintenance
  to change squash "state", apply one of the two following files:
  
  - squash-on.yml
  - squash-off.yml
  
  vm used during maintenance and data folder with html file displayed instead of squash:
  
  - maintenance.yml
  - data/index.html
  
  secret file to store credentials:
  
  - secrets.yml
