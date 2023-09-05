# jenkins

<style>
mark {
  background-color: #fc4d14;
  color: white;
}
</style>

<p align="center">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=jenkins"/>
  </a>
</p>

<table>
  <tr>
    <td width=40%>
Ambientes de criação de ambientes de pipeline com jenkins. Em distribuições Debian e baseadas em Debian como <mark>Ubuntu</mark> você pode instalar o Jenkins através apt.
    </td>
    <td>
O principal servidor de automação de código aberto, Jenkins fornece centenas de plug-ins para apoiar a construção, implantação e automação qualquer projeto. 
    </td>
  </tr>
</table>


### Requisitos mínimos de hardware:
- 256 MB de RAM
- 1 GB de espaço em disco (embora 10 GB seja o mínimo recomendado se estiver executando Jenkins como um contêiner Docker)

### Configuração de hardware recomendada para uma equipe pequena:
- 4GB+ de RAM
- 50 GB+ de espaço em disco

## Lançamento de suporte de longo prazo
Uma versão LTS (suporte de longo prazo) é escolhida a cada 12 semanas no fluxo de versões regulares como a versão estável para esse período. Pode ser instalado a partir do debian-stable apt repository.
```bash
curl -fsSL https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key | sudo tee \
  /usr/share/keyrings/jenkins-keyring.asc > /dev/null
echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
  https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
sudo apt-get update
sudo apt-get install jenkins
```