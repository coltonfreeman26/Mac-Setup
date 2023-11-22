# Mac Setup
## This project is meant to help with setting up an intel Mac book for DevOps type work.
### This is currently a WIP

**I work with Containers/Docker images a lot so this will mainly be aimed towards that but not strictly.**

### Setting up Brew
**Brew is Macs package manager. It makes downloading various tools quick and easy. Brew is open source and anyone can technically contribute a new package to their repository but they are vetted for validity before being accepted. So be aware of thepackage you are installing**
* First you will need to install Homebrew which can be ound here https://brew.sh/
* Once that is complete you now have the power of Brew. `brew install python@3.x`, `brew install docker` etc.
* You can view all the different casks and formulae here https://formulae.brew.sh/
* I would advise updating brew weekly (at least) `brew update` `brew upgrade`. I have a cron job set up that kicks this off every Monday morning before work.

### Setting up your IDE.
**I personally like Visual Studio Code the most but there are multiple options out there https://www.keycdn.com/blog/best-ide#which-is-the-best-ide-on-the-market . You can find the download link for VS Code here https://code.visualstudio.com/download**
* Once you have installed VS Code I would suggest also downloading some extras to help make using it easier.
* Oh My ZSH is a tool that enriches you terminal and is very configurable. https://ohmyz.sh/
* cmd+shft+p will bring up the prompt for you to search for `Toggle Auto Save` and `Install "code" command in PATH`. Both useful.
* Extensions are very useful for just about any type of work you are doing within VS    Code. Some of the ones I use are...
- Ansible by Red Hat
- Docker by Microsoft
- DotENV by mikestead
- Gitlab Workflow by Gitlab
- HashiCorp Terraform by HashiCorp
- json by zainchen
- Python by Microsoft
- YAML by Red Hat
* These are just a few I use. There are a lot out there for various needs like: spell   check, linting, SSH etc. I would advise only using extensions that have a lot of    downloads and a high rating.

### Tools I use to make my life easier
**Docker**
* Docker is a widely popular containerization tool. The two most popular options out there (Aside from Docker which is not free) are Rancher and Colima-(for Mac). I use Colima https://github.com/abiosoft/colima
* Colima uses Qemu as its virtualization tool which does eat up a lot of resources but this tool works out of the box.
* It also comes with k3s (kubernetes is disabled by default)
* To install and get colima running you just need to run `brew install colima` > `colima start` however I suggest using `colima start --kubernetes --cpu 16 --memory 16 --disk 100`

**Slack**
* Slack is a free opensource chat app that is widely used in the IT realm.
* To download slack go to https://slack.com/downloads/mac

**Programming languages.**
* Having multiple languages on your box at setup can save you some grief down the road when building or troubleshooting.
* A simple `brew install <language>` should do the trick. Pay attention to the download logs though as some installations will require you to either symlink them or update your PATH.

**Virtual Box**
* 

**CaC and IaC**
* Ansible, Terraform, Terragrunt and Packer
* 

**osxkeychain**
* 


### This project is meant to help individuals who have just joined the IT world or individuals who have not had to set up a computer in forever. Please feel free to contribute if something is missing or incorrect.