@title[Automation]

## Automation<br> @Actelion
How to migrate thousands of ip with little ressources and time.
@fa[fa-heart text-white]

@snap[south docslink span-50]
[Damien Hauser](http://www.dhconsulting.ch)
@snapend

+++?image=template/img/bg/orange.jpg&position=right&size=50% 100%
@title[Topics]

@snap[west split-screen-heading text-orange span-50]
Topics to be covered today
@snapend

@snap[east text-white span-45]
@ol[split-screen-list](false)
- Project
- Infrastructure
- GXP
- Solution
- Result
- Lessons learned
- Demo
@olend
@snapend

+++

### Project

- Automate the migration to the new ip plan (Windows and Linux)
- Take care of any dependancy (F5, Infoblox, Firewall, etc...)
- Short deadline and small team
- Keep the systems validated :-)


+++?image=template/img/bg/pink.jpg&position=left&size=50% 100%
@title[Infrastructure]

@snap[east split-screen-heading text-pink span-50]
Infrastructure
@snapend

@snap[west text-white span-65]
@ul[split-screen-list](false)
- Virtualization: Vmware
- DNS: Infoblox
- Load Balancers: F5
- Firewall: Checkpoint
@ulend
@snapend

@snap[south-west template-note text-white]
Most of the infrastructure is supported out of the box
@snapend

+++
@title[GXP: Qualifications]

@snap[east split-screen-heading text-green span-25]
GXP
@snapend

@snap[west text-white span-75]
Workshop with the quality team and qualify the whole automation system
@snapend

@snap[south-east template-note text-white]
Note: don't forget the mighty GXP
@snapend

+++
@title[Solution]

@snap[east text-white span-65]
@ul[split-screen-list](false)
- Database with the inventory
- Web application for the team doing the migration
- Ansible to automate the change
- Awx/Tower to provide a rest api 
- Pdf report for the quality team
@ulend
@snapend

@snap[west split-screen-img]
![SOLUTION](template/img/keep-calm-we-have-the-solution-11.png)
@snapend

@snap[south-west template-note text-gray]
@size[2em](Cost: open source software)
@snapend


+++?image=template/img/bg/black.jpg&position=left&size=50% 100%
@title[Result]

@snap[west split-screen-byline text-white]
We sucessfully migrated the VMs...
@snapend

@snap[midpoint split-screen-img]
![DEVELOPER](template/img/sucess.jpg)
@snapend

@snap[east split-screen-byline text-white]
With a team of 8 in 3 months.
@snapend


+++?image=template/img/bg/blue.jpg

## Lesson learned

1. Quality of the inventory is very important
2. Don't assume specific config on every systems (even if it should be the case): Disabling UAC on Windows was a PITA !
3. When a system doens't have an api the Ansible shell module is your friend 
4. There is never enough communication and documentation

+++

## Demo

#### Ansible roles and playbook
#### Ipmigrator
#### Awx/Tower
