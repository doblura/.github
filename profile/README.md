<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/doblura/.github/main/profile/logo-dark.png">
    <img src="https://raw.githubusercontent.com/doblura/.github/main/profile/logo-light.png" alt="Doblura" width="206">
  </picture>
</p>

<p align="center"><b>Rehearse your Odoo migration before it becomes irreversible.</b></p>

---

An Odoo `-u` alters the database schema and has no downgrade. No canary, no
blue/green, no rollback — the only way back is restoring a backup. And the
failures do not appear with demo data; they appear on the odd journal entry
somebody created in 2019.

So the only way to know whether a migration works is to run it against the real
data before running it against the real data. That is the whole idea, and the name:
**doblura**, from *doble* — the stunt double who takes the fall so the star does
not have to.

### Repositories

| | |
| --- | --- |
| [**doblura**](https://github.com/doblura/doblura) | the operator, the chart and the console · AGPL-3.0 |
| [**doblura.dev**](https://github.com/doblura/doblura.dev) | the site and the self-hosting documentation |

### Where the line is

Everything needed to rehearse a migration safely on your own cluster is open
source and stays that way: the rehearsal, the anonymized snapshots, every
guardrail, the environments, the five RBAC profiles, the console. The paid edition
is only what genuinely cannot exist on one cluster you already administer — many
clusters at once, a control plane somebody else operates, identity past group
mapping, retention across regions.

The test any future feature has to pass: *can a competent team do this on their own
cluster?* If yes, it is in the public repository, however sellable it looks.

Contributions are under the [DCO](https://github.com/doblura/doblura/blob/main/DCO)
— `git commit -s`, no CLA. Which also means the operator can never be relicensed,
by anyone. That is the point.
