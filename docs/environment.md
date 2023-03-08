# Environment structure

The scenario can be applied in several ways. The most interesting ones are, deploying a server for the web and another one for the Elastic stack from virtual machines, the same deployment but having the machines run the services via containers and finally, deploying the services directly via containers on the host machine.

## Criteria
We will follow these criteria in order to choose the best option:\
1. Realistic environmet
2. Easily reproducible
3. Easily maintained and updated


## Summary

>We are assuming that *alternative 1* is "deploying a server for the web and another one for the Elastic stack (VM)", *alternative 2* is "deploying both machines but run the services via containers" and *alternative 3* is "deploying the services directly via containers on the host machine".

The chosen option is: **Alternative 2**

| Alternative | Realistic | Easily reproducible | Easily maintained and updated |
|-------------|-----------|---------------------|-------------------------------|
| 1 | :white_check_mark: | :x: | :x: |
| 2 | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| 3 | :x: | :white_check_mark: | :white_check_mark: |


## Alternatives analysis
>We are assuming that *alternative 1* is "deploying a server for the web and another one for the Elastic stack (VM)", *alternative 2* is "deploying both machines but run the services via containers" and *alternative 3* is "deploying the services directly via containers on the host machine".

### Alternative 1
This alternative is realistic because several solutions found over the internet are deployed this way. The servers are running in different machines (vm) and will run natively on them.
This alternative won't be easy to reproduce due to the fact that running the services natively on the servers will make the scenario dependent on the OS and the packages it has.
This alternative won't be easy to maitain and update because it will require the maintenance of all the machine and updates of the whole system.

### Alternative 2
This alternative is realistic because several solutions found over the internet are deployed this way. The servers are running in different containers inside virtual machines.
This alternative will be easy to reproduce because the main focus will be a functional and up-to-day OS which can run some kind of containerization.
This alternative will be easy to maintain and update because the OS and the services can be maintained separately.

### Alternative 3
This alternative is not realistic since deploying all services on the host machine is not how real solutions are implemented.
This alternative will be easy to reproduce because the main focus will be a functional and up-to-day OS which can run some kind of containerization.
This alternative will be easy to maintain and update because the OS and the services can be maintained separately.
