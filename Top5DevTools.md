# Top 5 DevOps Tools to Increase Agility

DevOps has been broadly defined as a movement that aims to remove the barriers between the development and operations teams within an organization. Agile practices have helped to increase speed and agility within the development teams but the old methodology of throwing the code over the wall to an operations department to manage the deployment of the code to the production systems still persists. 

>> The primary goal of the adoption of the DevOps practice is to improve both the communication between disparate operations and development groups and the process by which they work.

	
Several tools are being used across the industry to put this idea into practice. We will cover what I feel is the top set of those tools from the various areas of the DevOps pipeline.

In no particular order.

## Docker 

“It worked on my machine…” Every operations or development manager has heard this at some point in their career. A developer commits their code and promptly breaks an important environment because their local machine isn’t configured to be identical to a larger production or integration environment. 

Containerization has exploded onto the scene and Docker is at the nexus of the change to isolate code and systems into easily transferable modules. Docker is used in the DevOps suite of tools in a couple of methods. The quickest win is to first use Docker to provide the developers with easily useable containers that can mimic the various systems within the stack. If a developer is working on a new RESTful service, they can checkout the container that is setup to run Node.js or Spring Boot and write the code for the new service with the confidence that the container will be identical to the service environment on the servers.

With the success of using Docker in the development workflow, the next logical step is to use Docker in the build stage of the CI/CD pipeline. Docker can help to isolate the build environments requirements across different portions of the larger application. By containerizing this step, it is easy to use one generic pipeline to build components as different spanning from Ruby and Node.js to Java and Golang.

## Git & JFrog Artifactory 

Source control and artifact management acts as the funnel for the DevOps pipeline. The structure of an organization can dictate how they run these tools, be it hosted or served locally. Git’s decentralized source code management and high performance merging features have helped it to become the most popular tool in version control systems. Atlassian BitBucket and Github both provide a good set of tooling around Git and are easy to use and to integrate with other systems. Source code control is vital to the pipeline, but the control and distribution of artifacts into the build and deployment chain is important as well.


![](https://raw.githubusercontent.com/darrellpratt/writings/master/1*eBxJEMDzJ04LfVBSJxlokA.png)
> Branching in Git


Artifactory is one-stop shop for any binary artifact hosted within a single repository which now supports Maven, Docker, Bower, Ruby Gems, CocoaPods, RPM, Yum and npm. As the codebase of an application grows and includes a broader set of technologies, the ability to control this complexity from a single point and integrate with a broad set of continuous integration tools cannot be stressed enough. Ensuring that the build scripts are using the correct dependencies, both external and internal, and serving a local set of Docker containers, reduces the friction in the build chain and will make the lives of the technology team much better.

## Jenkins 
There are several CI servers to choose from on the market. The hosted set of tools such as Travis CI, Codeship, Wercker and Circle CI are all very well suited to drive an integration pipeline and each caters slightly better to an organization that is more cloud focused (source control and hosting) with the deep integrations with GitHub and cloud providers like AWS, Heroku, Google and Azure. The older and less flashy system is Jenkins.

![](https://raw.githubusercontent.com/darrellpratt/writings/master/1*V0BBy66wRTr9d3_7D3B0JQ.png)
> Pipeline example




Jenkins has continued to nurture a large community that is constantly adding in new integrations and capabilities to the product. The Jenkins Pipeline feature provides a text based DSL for creating complex workflows that can move code from repository to the glass with any number of testing stages and intermediate environment deployments. The pipeline DSL can be created from code and this enables a good scaffolding setup for new projects to be integrated into the larger stack’s workflow.

## Hashicorp Terraform 
At this point we have a system that can build and manage applications through the software development lifecycle. The code is hosted in Git, orchestrated through testing and compilation with Jenkins, running in reliable containers and we are storing and proxying dependencies in Artifactory. The deployment of the application is where the operations and development groups come together in DevOps. Terraform is an excellent tool to manage the infrastructure required for running the applications as code itself. There are several vendors in this space — Chef, Puppet and Ansible to name just a few. Terraform sits at a higher level than many of these tools by acting as more of a provisioning system than a configuration management system. It has plugins to incorporate many of the configuration tools, so any investment that an organization has made in one of those systems can be maintained.


![](https://raw.githubusercontent.com/darrellpratt/writings/master/1*1K9cn6YGHsOFeZpClmwhNQ.png)
> Load balancer and instance config


Where Terraform excels, is its ability to easily provision arbitrarily complex multi-tiered systems, both locally or cloud hosted. The syntax is simple and declarative and because it is text it can be versioned along side the code and other assets of an application. This delivers on “Infrastructure as Code”.

## Slack 
A chat application was probably not what you were expecting in a DevOps article, but Slack has been a transformative application for many technology organizations. Slack provides an excellent platform for fostering communication between teams (text, voice and video) and integrating various systems. 

>> The DevOps movement stresses the removal of barriers between the teams and individuals who work together to build and deploy applications.

Web hooks provide simple integration points for simple things such as build notifications, environment statuses and deployment audits. There is a growing number of custom integrations for some of the tools we have covered in this article and the bot space is rapidly expanding into AI backed members of the team that answer questions about builds and code to deploy code or troubleshoot issues in production. It’s not a surprise that this space has gained its own name, ChatOps. Articles covering the top 10 ChatOps strategies will surely follow.


## Summary 
In this article we covered several of the tools that integrate into the DevOps culture and how those tools are used and are transforming all areas of the technology organization. While not an exhaustive list, the areas that were covered will give you an idea of the scope of the space and how these various systems can be integrated together.