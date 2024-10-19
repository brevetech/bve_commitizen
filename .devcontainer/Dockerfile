# Use an Ubuntu-based image
FROM mcr.microsoft.com/vscode/devcontainers/python:3-bullseye

# Install pyenv
RUN curl https://pyenv.run | bash

# Update bashrc to load pyenv
RUN echo 'export PATH="$HOME/.pyenv/bin:$PATH"' >> ~/.bashrc \
    && echo 'eval "$(pyenv init --path)"' >> ~/.bashrc \
    && echo 'eval "$(pyenv init -)"' >> ~/.bashrc \
    && echo 'eval "$(pyenv virtualenv-init -)"' >> ~/.bashrc

RUN pip install poetry

CMD [ "sleep", "infinity" ]
