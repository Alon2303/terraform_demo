# terraform_demo

## Prerequisites

- For the latest versions, update homebrew:
  ```zsh
    brew update
  ```

- Use the links below to install Terraform , AWS cli & Docker Desktop
  
- Install Links:  
  - [Terraform Cli](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli)
  - [AWS Cli](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html)
  - [Docker Desktop](https://docs.docker.com/docker-for-mac/install/)

- Clone the demo repo:
  ```zsh
    git clone https://github.com/Alon2303/terraform_demo.git
  ```

## Docker Example

- Change directory to docker_example
  ```zsh
    cd docker_example
  ```
- Init terraform project
  ```zsh
    terraform init
  ```

- Apply the instructions
  ```zsh
    docker apply
  ```

- If everything went well, you should be able to  
  receive a response from the server at localhost:8000

- To destroy the container run
  ```zsh
    terraform destroy
  ```

## AWS Example

- After installing AWS cli and to be able to work and expand on this demo, You'll need:
  - An AWS account(Requires a CC)
  - create accsess key and secret
  - in your local machine you'll need to export them like so:
    ```zsh
      export AWS_ACCESS_KEY_ID=<YOUR_ACCESS_KEY>
      export AWS_SECRET_ACCESS_KEY=<YOUR_SECRET_ACCESS_KEY>
    ```
  - Once you've set everything up, change directory to the aws_example
  - initialize the project:
    ```zsh
      terraform init
    ```
  - Now you can apply your changes with
    ```zsh
      terraform apply
    ```
  - With AWS it's V E R Y  important to track your resources
  - The same as the docker example you , to destroy the ec2 instance you can run:
    ```zsh
      terraform destroy
    ```


