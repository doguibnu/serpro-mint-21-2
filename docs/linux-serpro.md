## Instalar NeoID Linux Mint 21.2

**OBS: Alguns comandos realizados devem requerer permissão de super usuário (sudo), necessitando a senha de administrador do sistema.**

Verificando a versão do sistema:

![01-versao-mint-44](https://github.com/doguibnu/serpro-neoid-linux-mint-21-2/assets/38897311/562ef9c8-6ec1-4968-b41e-a2f9c1547fe2)

Abrir um **terminal** para executar o **update** e o **upgrade** do sistema com o comando:

```
sudo apt update -y && sudo apt upgrade -y
```

Ao finalizar o processo, executar um **reboot** do sistema, com o comando:

```
sudo reboot
```

Aguarde o sistema reiniciar!

No **Linux Mint (21.2)** é necessário baixar alguns pacotes manualmente para que se possoa instalar o aplicativo **NeoID** de forma correta e funcionamento desejado sem erros. Abra um **terminal** do sistema. Com o terminal aberto, utilizar o comando abaixo para fazer uma pasta chamada: **serpro**. Pasta feita, executar o comando para **entrar/mudar** para a pasta criada. Siga com os comandos abaixo:

```
mkdir serpro
cd serpro
```

A tela de terminal deve ser parecida como a figura abaixo:
![02-tela-terminal06](https://github.com/doguibnu/serpro-neoid-linux-mint-21-2/assets/38897311/b3baa6ed-8da3-4255-8656-59e46545fa41)
Dentro desta pasta criada, vamos iniciar o processo de instalação de alguns pacotes necessários. O primeiro pacote a ser baixado é: `libssl1.0.0_1.0.2g-1ubuntu4.20_amd64.deb`  Utilize o comando abaixo para download do pacote:

```
wget http://nz2.archive.ubuntu.com/ubuntu/pool/main/o/openssl/libssl1.0.0_1.0.2g-1ubuntu4.20_amd64.deb
```

Sua tela de terminal deve parecer com esta abaixo:

![03-pacote01-libssl04](https://github.com/doguibnu/serpro-neoid-linux-mint-21-2/assets/38897311/bd5e6d70-5035-489c-b336-5da40e228714)
Vamos instalar o pacote com o comando abaixo. **Atenção:** para este comando, será solicitado a senha de super usuário **(sudo)**:

```
sudo dpkg -i libssl1.0.0_1.0.2g-1ubuntu4.20_amd64.deb
```

Neste comando, sua tela de **terminal** deve parecer como abaixo. Digite a tecla **enter**:
![04-sudo-prim-pacote9](https://github.com/doguibnu/serpro-neoid-linux-mint-21-2/assets/38897311/d63d4e94-3836-4fb3-94a9-d683b1f3a84e)
O comando irá solicitar a **senha** de super usuário como mostra a figura abaixo. Digitar a senha de super usuário **(sudo)** e tecle **enter**.

![05-tela-sudo-prim-comando1](https://github.com/doguibnu/serpro-neoid-linux-mint-21-2/assets/38897311/7216dfb3-0ee3-4235-9da1-0f8f9f41b979)

O comando irá **instalar o pacote**. A tela deve parecer como a figura abaixo:
![06-instalar-primeiro-comando33](https://github.com/doguibnu/serpro-neoid-linux-mint-21-2/assets/38897311/61ddde35-932e-4c24-b3d1-7feb5b0ed101)

Ainda neste mesmo **terminal**, vamos executar o download do próximo pacote necessário que é: `libssl1.1_1.1.0g-2ubuntu4_amd64.deb` Utilizar o comando abaixo e digitar a tecla **enter:**

```
wget http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/libssl1.1_1.1.0g-2ubuntu4_amd64.deb 
```

A tela do comando será parecida com esta abaixo:

![07-segundo-pacote7](https://github.com/doguibnu/serpro-neoid-linux-mint-21-2/assets/38897311/bac76b49-4682-4842-855d-0af55420f1e3)

Quando o comando for executado, a tela deve parecer como esta abaixo:

![08-down-segundo-pacote](https://github.com/doguibnu/serpro-neoid-linux-mint-21-2/assets/38897311/a90897e3-d33b-4450-823f-fcf268e61e63)

Vamos instalar este segundo pacote baixado com o comando indicado. **Atenção:** o comando irá solicitar a senha de super usuário **(sudo)**, digite a tecla **enter** e digite a senha de super usuário.

```
sudo dpkg -i libssl1.1_1.1.0g-2ubuntu4_amd64.deb
```

A tela para executar o comando no **terminal** deverá parecer como esta abaixo:
![10-tela-instala-segundo-pacote-17](https://github.com/doguibnu/serpro-neoid-linux-mint-21-2/assets/38897311/db5e787e-6fd4-43f9-948f-2a22be9210f2)

Próximo passo, vamos baixar e instalar o pacote: **libnss3-tools** através do site da comunidade **Linux Mint.** Abra o navegador Firefox e acesse o endereço:

[Linux Mint - Community](https://community.linuxmint.com/software/view/libnss3-tools) . O navegador deve mostrar a tela como na figura abaixo. Clicar no botão **Install**:

![11-site-libnss0fire](https://github.com/doguibnu/serpro-neoid-linux-mint-21-2/assets/38897311/055df0d9-4698-4daa-921a-37bfccffcf0e)

Quando clicar, uma janela irá abrir questionando se permite que o site possa abrir a ligação do aplicativo **apt (instalar pacotes)** com o **AptURl**. Clique em: **Abrir/Permitir Ligação** como mostra a figura abaixo:

![12-clicar-abrir-link-52a](https://github.com/doguibnu/serpro-neoid-linux-mint-21-2/assets/38897311/c112d4e9-9058-453d-b7f7-52d21dc9780c)

Então, uma janela de instalação de programa irá questionar se deseja instalar o pacote desejado, como mostra a figura abaixo. **Clique** em **Instalar**:

![13-tela-de instalar-pacote0libnss3-50](https://github.com/doguibnu/serpro-neoid-linux-mint-21-2/assets/38897311/7b91b07a-7a61-4c53-8ad6-c5704e7a140a)

Inserir a senha de **super usuário** e clique em **Autenticar** para executar a instalação do pacote como mostra a figura abaixo. O pacote será instalado no sistema e a tela de instalação irá fechar.

![14-senha-para-instalar-pacote](https://github.com/doguibnu/serpro-neoid-linux-mint-21-2/assets/38897311/2b21d036-7cb9-45e5-801a-cee8aa703d46)

Os pacotes necessários foram instalados no sistema para o funcionamento correto do NeoID. Vamos baixar o instalador do NeoID da Serpro no site de download, acessando:  [NeoID - Seu certificado digital em nuvem - Drivers](https://neoid.estaleiro.serpro.gov.br/downloads/) selecione o sistema operacional **Linux** e clique em **baixar**. Veja a figura abaixo: 

![15-neo-id-baixiar-site-54aa](https://github.com/doguibnu/serpro-neoid-linux-mint-21-2/assets/38897311/dbfb82be-8ce6-415c-baab-77a0f590b565)

Quando o downlaod for concluído, **clique** no arquivo baixado para podermos fazer a instalação do mesmo, como mostra a figura abaixo:

![16-dowload-neo-id-44aa](https://github.com/doguibnu/serpro-neoid-linux-mint-21-2/assets/38897311/4c65627e-ca11-4cfc-b3d5-16e5bef3408b)

Aguarde o sistema mostrar a tela de instalação do program e então clique no botão: **Instalar Pacote**. Será requerido a senha de **super usuário (sudo)**.

![16-instalar-Neoid36](https://github.com/doguibnu/serpro-neoid-linux-mint-21-2/assets/38897311/d93483fa-fb41-4e79-a631-65b0a9234605)

Inserir a senha e clicar em **Autenticar**:

![17-senha-instalar-neoidg](https://github.com/doguibnu/serpro-neoid-linux-mint-21-2/assets/38897311/b22afc30-e09e-44f2-9442-983764a31c6c)

Alguns softwares adicionais serão requeridos para a instalação completa do aplicativo. Clique em **Continuar** e aguarde a finalização do processo. Veja a figura abaixo:

![18-pacotes-requeridos-neoid31](https://github.com/doguibnu/serpro-neoid-linux-mint-21-2/assets/38897311/d085cb82-7819-4a79-97e1-7785391298a7)

Após a instalação do programa, clique no menu do Linux Mint e encontre o programa **NeoID** como mostra a figura abaixo e **clique** para iniciar o mesmo:

![21-menu-neoid-mint](https://github.com/doguibnu/serpro-neoid-linux-mint-21-2/assets/38897311/abd9f967-fb35-4cc3-9142-fc7b61c2b56e)

Para aprender a usar o **NeoID**, utilize o manual oficial disponibilizado no site da [Serpro ](https://neoid.estaleiro.serpro.gov.br/downloads/Manual-NeoID.pdf)


**TUTORIAL REALIZADO ATRAVÉS DO DEPARTAMENTO de TI**
