# Instalando Jenkins
## Guias deste repositório
- <a href="https://github.com/joao-prs/jenkins">Voltar para o inicio.</a>
- <a href="https://github.com/joao-prs/jenkins/blob/main/GUI.installation.md">Guia de uso.</a>

## Instalação de Java
Jenkins requer Java para funcionar, mas certas distribuições não incluem isso por padrão e algumas versões Java são incompatíveis com Jenkins.
```bash
sudo apt update
sudo apt install openjdk-17-jre
java -version
openjdk version "17.0.7" 2023-04-18
OpenJDK Runtime Environment (build 17.0.7+7-Debian-1deb11u1)
OpenJDK 64-Bit Server VM (build 17.0.7+7-Debian-1deb11u1, mixed mode, sharing)
```

## Lançamento de suporte de longo prazo
Uma versão LTS (suporte de longo prazo) é escolhida a cada 12 semanas no fluxo de versões regulares como a versão estável para esse período. Pode ser instalado a partir do debian-stable apt repository.
```bash
curl -fsSL https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key | sudo tee \
  /usr/share/keyrings/jenkins-keyring.asc > /dev/null
echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
  https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
sudo apt update
sudo apt install jenkins
```

> informações tiradas do site oficial do jenkins, para mais informações, visite o <a href="https://www.jenkins.io/">site</a>.