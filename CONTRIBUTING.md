# Contribution Guidelines

We appreciate your interest in contributing to **_the sudo academy_**! This document outlines the guidelines and best practices for contributing to this project.


## Code of Conduct

By participating in this project, you are expected to uphold our [Code of Conduct](CODE_OF_CONDUCT.md).


## Reporting Issues

If you find a bug or have a suggestion for improvements, please create an issue on the GitHub repository.
Be sure to provide enough information for us to understand and reproduce the issue


## Local Development Setup

### Docker for serving the website
 
1. Install [Docker](https://www.docker.com/products/docker-desktop) on your system.
2. Clone the repository: `git clone https://github.com/thesudoacademy/thesudo.academy.git`
3. Navigate to the project directory: `cd thesudo.academy`
4. Build the Docker image: `docker build -t thesudo-academy .`
5. Run the Docker container: `docker run --rm -it -p 8000:8000 -v ${PWD}:/docs thesudo-academy`

The site should now be accessible at http://localhost:8000 and making changes to the documentation files will be automatically reflected in the site. 

#### Build the website using Docker

1. Build the Docker image: `docker build -t thesudo-academy .`
2. Run the Docker container to build the website: `docker run --rm -it -v ${PWD}:/docs thesudo-academy build`

The built website will be available in the `site` directory within your project folder.

### Using Docker Compose

1. Install [Docker Compose](https://docs.docker.com/compose/install/) on your system.
2. Clone the repository: `git clone https://github.com/thesudoacademy/thesudo.academy.git`
3. Navigate to the project directory: `cd thesudo.academy`
4. Run the Docker Compose for local development: `docker-compose up`

The site should now be accessible at http://localhost:8000, and making changes to the documentation files will be automatically reflected in the site.

#### Docker Compose for building the website

1. Run the Docker Compose to build the website: `docker-compose run --rm mkdocs build`

The built website will be available in the `site` directory within your project folder.

## Submitting a Pull Request
Before submitting a pull request, make sure you have:

1. Forked the repository.
2. Created a new branch for your changes.
3. Made your changes in the new branch.
4. Tested your changes locally.
5. Pushed your changes to your forked repository.
6. Created a pull request with a clear and concise description of your changes.

We will review your pull request and provide feedback. If everything looks good, we'll merge your changes.

Thank you for your contributions!


## License

By contributing, you agree that your contributions will be licensed under the MIT License. See [LICENSE](LICENSE) for more information.