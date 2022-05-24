## Jupyter Boilerplate :star:

### Project structure

```
.
├── data                         # Data sources (.csv, .txt...)
├── notebooks                    # Jupyter Notebook files
├── queries                      # Files to keep queries, if needed
├── scripts                      # Scripts (to configure the container, but may be used to other purposes as well)
├── tests                        # Automated tests (alternatively `spec` or `tests`)
├── utils                        # Tools and utilities
└── README.md
```

### Getting started

- Starting the container:

`$ make up`

- Stopping the container:

`$ make down`

- Building the image

`$ make build` 

- Accessing the container shell

`$ make shell` 

### Adding new libs

- Add the lib and the version to the `requirements.txt` file;
- Make sure the container is down with `$ docker-compose down`;
- Build the image with the new lib with `$ docker-compose build`;
- Start the container with `$ docker-compose up`;
- You can now use the lib in your notebook with `import <lib>`.
