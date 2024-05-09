# Cocktailify

![GitHub last commit](https://img.shields.io/github/last-commit/Omri-Lvy/Cocktailify)
![GitHub issues](https://img.shields.io/github/issues/Omri-Lvy/Cocktailify)
![GitHub forks](https://img.shields.io/github/forks/Omri-Lvy/Cocktailify)
![GitHub stars](https://img.shields.io/github/stars/Omri-Lvy/Cocktailify)
![GitHub license](https://img.shields.io/github/license/Omri-Lvy/Cocktailify)
![Python version](https://img.shields.io/badge/python-3.x-blue.svg)
![React version](https://img.shields.io/badge/react-18.2.0-blue.svg)

Welcome to **Cocktailify**, an exciting project developed for the Development Club at Reichman University. Our goal is to provide students with hands-on experience in web development and database management.

This project serves as an exemplary model, illustrating the end goal of what students can achieve with the skills they acquire in the club. It demonstrates a practical application of web development and database management techniques, showcasing a fully functional web-based application.

![Status](https://img.shields.io/badge/status-in_development-orange.svg)

## Table of Contents

- [Project Introduction](#cocktailify)
- [Table of Contents](#table-of-contents)
- [Quick Start](#quick-start)
  - [Prerequisites](#prerequisites)
  - [Cloning the Repository](#cloning-the-repository)
  - [Running the Application](#running-the-application)
- [Updating Your Local Repository](#updating-your-local-repository)
- [License](#license)
- [Acknowledgements](#acknowledgements)


## Quick Start

### Prerequisites

Before you begin, ensure you have the following installed:
- Git
- Python (with pip)
- Node.js
- A web browser

### Cloning the Repository

Clone this repository and all its submodules using:

```bash
    git clone --recurse-submodules https://github.com/yourusername/MainRepo.git
```

If you have already cloned the repository without submodules, initialize and update them with:

```bash
    git submodule update --init --recursive
```

### Running the Application

**Server (Flask):**
1. To start the Flask server, navigate to the server directory and set up a virtual environment:

```bash
    cd server
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    pip install -r requirements.txt
```

2. Create a `.env` file inside the `app` folder with the following configurations:

```bash
    echo "MONGO_URI=your_mongo_uri_here" >> .env
    echo "PROD_ORIGIN=your_production_origin_url_here" >> .env  # Optional
    echo "DEV_ORIGIN=your_development_origin_url_here" >> .env  # Optional
```

3. Run the server using:

```bash
    flask run
```

**Client (React):**
1. To launch the React client, in another terminal window, navigate to the client directory and install dependencies:

```bash
    cd client
    npm install
    npm start
```

2. (optional) Create a `.env` file in the client directory with your configurations configurations:

```bash
    echo "REACT_APP_BACKEND_ADDRESS_PROD=your_production_backend_url_here" > .env
    echo "REACT_APP_BACKEND_ADDRESS_DEV=your_development_backend_url_here" >> .env
```

3. Start the client:

```bash
    npm run start
```

By default the client can be accessed at `http://localhost:3000` in your web browser, and the server will be running on `http://localhost:5000`.

## Updating Your Local Repository

To ensure your local repository stays current with the main project repository, follow these steps:

### Fetching the Latest Changes

1. **Fetch the Latest Changes from the Main Repository**
   First, you'll need to fetch the latest changes from the main repository. This does not merge the changes into your local branch but allows you to see what they are.

```bash
    git fetch origin
```

### Merging Updates

2. **Merge the Updates into Your Current Branch**
   Once you have fetched the updates, you can merge them into your current branch to keep your local repository up-to-date.

```bash
    git merge origin/main  # Replace 'main' with the appropriate branch name if different
```

### Updating Submodules

3. **Update Submodules**
   If the project uses submodules, as Cocktailify does, you'll also need to update them to get the latest changes.

```bash
    git submodule update --remote --recursive
```

### Handling Merge Conflicts

4. **Resolve Any Merge Conflicts**
   If there are conflicts between your changes and the updates, you'll need to resolve them. This process may require manual editing of the conflicted files.

```bash
    # Follow git's instructions to resolve conflicts
```

By regularly updating your local repository, you can avoid large merge conflicts and stay aligned with the project's progress.

## License

Cocktailify is open source and freely available to everyone. It is provided under the MIT License, which allows users to modify, distribute, and use the software for both private and commercial purposes.

### License Summary

- **Permission is granted** to use, copy, modify, and distribute the software.
- **No warranty** is provided with the software. Use it at your own risk.

For full details, see the [LICENSE](LICENSE) file included in the repository.

## Acknowledgements
I extend my heartfelt thanks to everyone who has contributed to the Cocktailify project.

I also acknowledge the use of open-source libraries and tools that made this project possible. Thank you to the broader open-source community for supporting initiatives like mine.




