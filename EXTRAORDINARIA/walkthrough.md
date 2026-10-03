 

# ChatBotPSP23 - Walkthrough

AWS:

- Start Lab

- Create Cloud9

  - New EC2
  - Ubuntu Server 18.04
  - SSH Connection

- Remember to open port on security rules.

- Open Cloud9

- Cloud9 Terminal

  - Configure git:

    - ```sh
      git config --global user.name "Your Name"
      ```

    - ```sh
      git config --global user.email "youremail@yourdomain.com"
      ```

  - Config to automatically push tags:

    - ```sh
      git config --global push.followTags true
      ```

  - Generate keypair

  - ```sh
    ssh-keygen -t rsa
    ```

  - show public key and copy to Github account settings:

  - ```sh
    cat ~/.ssh/id_rsa.pub
    ```

  - Start ssh-agent in the background

  - ```sh
    eval $(ssh-agent -s)
    ```

  - Add your private ssh key to ssh-agent:

  - ```sh
    ssh-add ~/.ssh/id_rsa
    ```

- Sometimes you will need:

  - ```sh
    ssh-keyscan -t rsa github.com >> ~/.ssh/known_hosts
    ```

- Cloud9 IDE:

  - Clone ssh repository
  - Add Server and Client Files
  - Test in local
  - Test from remote client
  - Commit 
  - Create Tag Phase1
  - Push

- Tags (Not recommended):

  - Push all annotated tags

  - ```sh
    git push origin --tags
    ```
