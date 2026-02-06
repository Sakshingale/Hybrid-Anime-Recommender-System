FROM jenkins/jenkins:lts

USER root

# Install Docker CLI (stable & compatible)
RUN apt-get update && \
    apt-get install -y \
        ca-certificates \
        curl \
        gnupg && \
    mkdir -p /etc/apt/keyrings && \
    curl -fsSL https://download.docker.com/linux/debian/gpg | \
        gpg --dearmor -o /etc/apt/keyrings/docker.gpg && \
    echo \
        "deb [arch=amd64 signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/debian bookworm stable" \
        > /etc/apt/sources.list.d/docker.list && \
    apt-get update && \
    apt-get install -y docker-cli && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*

# Allow Jenkins to use Docker
RUN groupadd -f docker && \
    usermod -aG docker jenkins

USER jenkins
