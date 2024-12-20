To set up Jenkins to use the Controller-Agent method (also known as Jenkins agent by the controller method), we need to ensure that the Jenkins master (controller) handles the creation and management of the agent connection rather than relying on the JNLP method.

This method is commonly used when the agent is launched automatically and managed from the Jenkins master using an SSH connection or the agent's docker container setup directly via the Jenkins controller.
Objective:

    Set up the Jenkins master to automatically start a slave agent via the Controller-Agent method.
    Use Docker Compose to define both the Jenkins master (controller) and slave (agent) containers.

Approach:

We will configure the slave agent to use Docker's controller-agent method, where Jenkins master manages the slave agent's lifecycle automatically.
Key Steps:

    Configure Jenkins Master to allow the Controller-Agent method.
    Set up the Jenkins slave (agent) container and ensure it communicates with the master using this method.
    Use Docker Compose to orchestrate both containers.


