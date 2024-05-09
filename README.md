# Cocktaily

#### Welcome to the Cocktail Recipes Website project, an engaging and educational initiative developed for the Development Club at Reichman University! This project aims to provide students with a practical, hands-on experience in web development and database management.


## Main Project Repository

This repository serves as the central hub for the Cocktailify, which is structured into two main components: the Server and the Client. Each component is maintained in its own repository and included here as a submodule.

## Repository Structure

- `server`: This submodule links to the Server repository which handles all backend operations.

- `client`: This submodule links to the Client repository which manages the frontend interface.

## Cloning the Repository

To clone this repository along with its submodules, you should use the following command:

```sh
git clone --recurse-submodules https://github.com/yourusername/MainRepo.git
```
If you have already cloned the main repository without the submodules, you can initialize and update the submodules with:

```sh
git submodule update --init --recursive
```


### 4. Pulling Latest Updates
This section explains how to update the repository and its submodules to ensure all parts are current.

## Pulling Latest Updates

To fetch the latest updates for the main repository and all submodules, follow these steps:

1. Pull the latest changes for the main repository:
    ```sh
   git pull
    ```
2. Update all submodules to the latest commits on their respective branches:
    ```sh
   git submodule update --remote --recursive
    ```

