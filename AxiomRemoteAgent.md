# Magnet Axiom Cyber - Remote Agent

## Disclaimer
This writeup is product using Magnet Axiom Version 6. This guide is my personal reference. Do your own test for feasibility of your deployment.
All Access must be legal or authorized.

## Setting up Remote Agent
1. In AXIOM Process, start a new case and fill up the details
<img width="500" alt="image" src="https://github.com/cisnerof/img/blob/main/AxiomRemote001.png">

2. Proceed to 'Evidence Sources', click on 'Remote computer'.
<img width="500" alt="image" src="https://github.com/cisnerof/img/blob/main/AxiomRemote002.png">

3. In the Manage agents and endpoints screen, click 'Create new agent'.
<img width="500" alt="image" src="https://github.com/cisnerof/img/blob/main/AxiomRemote003.png">

4. In the 'General agent settings section', provide a unique Agent ID in the 'Agent ID' field to identify the agent within AXIOM Process. If you don’t enter an Agent ID, AXIOM Process will automatically create a unique ID for you.
5. From the Operating system drop-down list, select which operating system you want to create the agent for.
6. In the Agent masking details section, in the File name field, provide the name of the agent as you want it to appear on the endpoint.
7. To configure additional masking details for the agent, click Show more details. Provide any other information to determine how you want the agent to appear on the endpoint.
<img width="500" alt="image" src="https://github.com/cisnerof/img/blob/main/AxiomRemote004.png">

8. If you want the agent to survive a shut down of the endpoint, select Keep the agent on the endpoint after a shut down.
<img width="500" alt="image" src="https://github.com/cisnerof/img/blob/main/AxiomRemote005.png">

9. In the Connectivity details section, provide information about the host computer that will deploy the agent. Typically, this is the IP of the machine for the Axiom Process
<img width="500" alt="image" src="https://github.com/cisnerof/img/blob/main/AxiomRemote006.png">

10. Click 'Create agent'. Agent are stored in c:\.
<img width="500" alt="image" src="https://github.com/cisnerof/img/blob/main/AxiomRemote006.png">

11. To remotely deployed an agent, click on 'Deploy Agent'
<img width="500" alt="image" src="https://github.com/cisnerof/img/blob/main/AxiomRemote007.png">

12. In the 'Deploy Agent' section, Enter:
    - IP address of the target
    - Username and password
    - Location for the agent to be stored. Path of the location must exist on the remote target.
<img width="500" alt="image" src="https://github.com/cisnerof/img/blob/main/AxiomRemote008.png">

13. If the agent is successfully deployed and launched, can proceed to 'Connect To Agent'
<img width="500" alt="image" src="https://github.com/cisnerof/img/blob/main/AxiomRemote009.png">

14. In the 'Connect To Endpoints' section, you can see the agents connected to Axiom Cyber. Click on 'Connect To Endpoint' at the desired target to connect to target machine.
<img width="500" alt="image" src="https://github.com/cisnerof/img/blob/main/AxiomRemote010.png">

15. Once successful, you can proceed to select the data to be exported.

### Windows
16. If the OS of the remote machine is Windows, there are 3 options:
    - Targeted Locations
    - Files and Drives
    - Memory
<img width="500" alt="image" src="https://github.com/cisnerof/img/blob/main/AxiomRemote011.png">

17. In the 'Memory' option, you can choose to acquire the full memory dump or the individual process(es)
<img width="500" alt="image" src="https://github.com/cisnerof/img/blob/main/AxiomRemote012.png">

18. In the 'Targeted Locations', there is a set of pre-defined artifacts. You can also add on to the predefined set.
<img width="500" alt="image" src="https://github.com/cisnerof/img/blob/main/AxiomRemote014.png">

19. In the 'Files and Drives' option, you can choose to collect specified folders and files, or acquire the drive.
<img width="500" alt="image" src="https://github.com/cisnerof/img/blob/main/AxiomRemote015a.png">

20. Full drive acquisition
<img width="500" alt="image" src="https://github.com/cisnerof/img/blob/main/AxiomRemote016a.png">

21. The selected artifacts will queue to be collected from the target machine
<img width="500" alt="image" src="https://github.com/cisnerof/img/blob/main/AxiomRemote017a.png">

### Linux
22. If the OS of the remote machine is Linux, there are 2 options:
    - Targeted Locations
    - Files and Drives
<img width="500" alt="image" src="https://github.com/cisnerof/img/blob/main/axiomremotelinux001.png">

23. In the 'Targeted Locations', there is a set of pre-defined artifacts. You can also add on to the predefined set.
<img width="500" alt="image" src="https://github.com/cisnerof/img/blob/main/axiomremotelinux002.png">

24. In the 'Files and Drives' option, you can choose to collect specified folders and files. You can select '/' to collect all the files and folders.
<img width="500" alt="image" src="https://github.com/cisnerof/img/blob/main/axiomremotelinux003.png">

### MacOS
22. If the OS of the remote machine is Mac, there are 2 options:
    - Targeted Locations
    - Files and Drives
<img width="500" alt="image" src="https://github.com/cisnerof/img/blob/main/axiomremotemac001.png">

23. In the 'Targeted Locations', there is a set of pre-defined artifacts. You can also add on to the predefined set.
<img width="500" alt="image" src="https://github.com/cisnerof/img/blob/main/axiomremotemac002.png">

24. In the 'Files and Drives' option, you can choose to collect specified folders and files. You can select '/' to collect all the files and folders.
<img width="500" alt="image" src="https://github.com/cisnerof/img/blob/main/axiomremotemac003.png">

## References
Configuring An Agent 
- https://www.magnetforensics.com/docs/axiom-cyber/html/Content/en-us/acquire-remote/configuring-agent.htm

Remotely (& Covertly) Acquire Mac with Magnet AXIOM Cyber 
- https://www.youtube.com/watch?v=uHvyjOEMrhE
