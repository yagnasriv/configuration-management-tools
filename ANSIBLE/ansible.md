## Configuration Management Tools
# ANSIBLE
___________________________________________________________________________________________________

- Ansible is an open-source automation tool that is widely used in DevOps practices for configuration management, application deployment, task automation, and orchestration.
- It simplifies complex infrastructure and application management tasks by providing a simple, human-readable language to describe automation workflows.
- Ansible is agentless, meaning it doesn't require any software to be installed on the managed nodes, making it easy to use and deploy.

- Ansible is installed on the control node and the contrl node manages the managed node / nodes. 
    - Control Node :
        - Ansible is installed on the Control node and from which all tasks and playbooks are executed. It is the system that you use to connect to and control other machines.
    - Managed Nodes :
        - Managed nodes are the remote servers or devices that are managed by Ansible. These are the systems on which Ansible performs tasks, runs playbooks, and manages configurations.
        - When you run an Ansible playbook or ad-hoc command, the control node connects to the managed nodes over SSH (by default) and executes the specified tasks. The managed nodes don't require any special software or agents; Ansible relies on standard SSH connections and Python to execute its tasks.

Here's a brief overview of the typical roles:

Control Node:

Ansible is installed on the control node.
Playbooks and tasks are defined and executed from the control node.
SSH keys are often used to enable passwordless access to the managed nodes.
Managed Nodes:

No specific Ansible software or agent is required on managed nodes.
Python (version 2 or 3) must be available on the managed nodes as Ansible uses it to execute modules.
While the terminology might differ (for example, you may hear "worker nodes" in other automation or orchestration tools), in the context of Ansible, the control node and managed nodes are the primary entities. Ansible uses a push-based model where the control node pushes configurations and tasks to the managed nodes, making it agentless and straightforward to set up.


Key features and components of Ansible include:

- Playbooks
    - Ansible automation is defined in YAML files called playbooks. 
    - Playbooks are human-readable and describe a series of tasks that need to be executed on remote nodes.

- Inventory
    - The inventory is a list of managed nodes (servers) that Ansible can connect to and perform tasks on. It can be static or dynamic and is defined in INI or YAML format.

- Modules
- Roles
- Templates