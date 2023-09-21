
# Implementando um site estático com o S3 e CloudFront

Este projeto foi desenvolvido como TCC do curso AWS Fundamentos da Escola da Nuvem. O desafio foi o desenvolvimento de um website estático e a estruturação de uma arquitetura utilizando AWS para disponibilizar este site, atendendo a demanda de 11 milhões de requisições (get, select) por mês.

## Estrutura do Site

Toda a estrutura do site está disponível [aqui](./site). O site estático possui uma interface amigável e aplicando os conceitos de user interface, para apresentação dos currículos de todos os integrantes do grupo de desenvolvedores. Estão disponíveis os arquivos [index.html](./site/index.html), [style.css](./site/style.css) e [mains.js](./site/main.js).




<div style="display: flex; justify-content: center;">
    <img src="img\Webpage.png" height="400" />
</div>

## Planejamento da Arquitetura AWS

O planejamento da arquitetura AWS é uma etapa crucial para o sucesso do projeto. Ele envolve a definição dos serviços e recursos da AWS que serão utilizados, bem como a estruturação e configuração desses serviços para atender aos requisitos do projeto.

Durante o planejamento, é importante considerar os seguintes aspectos:

1. **Escalabilidade**: Garantir que a arquitetura seja capaz de lidar com o aumento da demanda de tráfego e processamento, sem comprometer o desempenho do site estático.

2. **Disponibilidade**: Assegurar que o site esteja sempre disponível para os usuários finais, mesmo em caso de falhas em algum dos serviços utilizados.

3. **Segurança**: Implementar medidas de segurança adequadas para proteger o site contra ameaças cibernéticas, como ataques DDoS e injeção de código malicioso.

4. **Otimização de recursos e custos**: Utilizar os recursos da AWS de forma eficiente, evitando desperdícios e reduzindo os custos operacionais.

5. **Monitoramento e gerenciamento**: Estabelecer mecanismos de monitoramento e gerenciamento dos serviços utilizados, a fim de identificar possíveis problemas e garantir a estabilidade do site.

A arquitetura AWS desempenha um papel fundamental no sucesso do projeto, pois permite a disponibilização do site estático de forma eficiente, segura e escalável. Portanto, é essencial dedicar tempo e esforço ao planejamento adequado da arquitetura.

## Serviços utilizados na AWS:


<div style="display: flex; align-items: center;">
    <img src="img\Arch_Amazon-Simple-Storage-Service_64.png" height="40" />
    <div style="margin-left: 10px;">
        <strong>S3 (Simple Storage Service)</strong>: É um serviço de armazenamento de objetos que oferece escalabilidade, disponibilidade de dados, segurança e performance. Ele é utilizado para armazenar os arquivos do site estático.
    </div>
</div>
<br>
<div style="display: flex; align-items: center;">
    <img src="img\Arch_Amazon-CloudFront_64.png" height="40" />
    <div style="margin-left: 10px;">
        <strong>CloudFront</strong>: É uma rede de entrega de conteúdo (CDN) que distribui o conteúdo do site estático globalmente, melhorando a velocidade de acesso ao site para os usuários finais.
    </div>
</div>
<br>
<div style="display: flex; align-items: center;">
    <img src="img\Arch_Amazon-Route-53_64.png" height="40" />
    <div style="margin-left: 10px;">
        <strong>Route 53</strong>: É um serviço de sistema de nomes de domínio (DNS) altamente disponível e escalável. Ele é utilizado para rotear o tráfego da internet para o site estático.
    </div>
</div>
<br>
<div style="display: flex; align-items: center;">
    <img src="img\Arch_AWS-Certificate-Manager_64.png" height="40" />
    <div style="margin-left: 10px;">
        <strong>Certificate Manager</strong>: É um serviço que provisiona e gerencia certificados SSL/TLS para uso com serviços da AWS e recursos internos conectados. Ele garante a segurança das comunicações entre o site estático e os usuários finais.
    </div>
</div>
<br>
<div style="display: flex; align-items: center;">
    <img src="img\Arch_AWS-Shield_64.png" height="40" />
    <div style="margin-left: 10px;">
        <strong>AWS Shield</strong>: É um serviço que fornece proteção contra ataques de negação de serviço distribuídos (DDoS) para recursos da AWS. Ele ajuda a manter o site estático seguro e disponível mesmo durante ataques DDoS.
    </div>
</div>
<br>
<div style="display: flex; align-items: center;">
    <img src="img\Arch_AWS-WAF_64.png" height="40" />
    <div style="margin-left: 10px;">
        <strong>AWS WAF</strong>: É um firewall de aplicação web que monitora e controla o acesso ao site estático, protegendo-o contra ataques comuns à segurança da web, como injeção SQL ou cross-site scripting (XSS).
    </div>
</div>
<br>

# Arquitetura AWS utilizada

A arquitetura AWS utilizada neste projeto foi planejada para garantir a escalabilidade, disponibilidade e segurança do site estático. Para isso, foram utilizados os seguintes serviços da AWS:

- **S3 (Simple Storage Service)**: Utilizado para armazenar os arquivos do site estático .

- **Route 53**: Utilizado para rotear o tráfego da internet para o site estático .

- **CloudFront**: Melhorando a velocidade de acesso ao site para os usuários finais  .

- **Certificate Manager**: Garante a segurança das comunicações entre o site estático e os usuários finais  .

- **AWS Shield**: Ajuda a manter o site estático seguro e disponível mesmo durante ataques DDoS  .

- **AWS WAF**: Firewall de aplicação web que monitora e controla o acesso ao site estático, protegendo-o contra ataques comuns à segurança da web, como injeção SQL ou cross-site scripting (XSS)  .

A utilização desses serviços foi planejada para otimizar os recursos e custos da arquitetura, garantindo a segurança e disponibilidade do site estático.

<div style="display: flex; justify-content: center;">
    <img src="img\arquitetura-aws.png" height="400" />
</div>

## Agradecimentos

Gostaríamos de agradecer a todos os colegas do grupo do TCC (Manoela Araújo, Francieli Alves Araujo e Renato Cunha Jr.) pela dedicação e aplicação de seus conhecimentos e saberes que contribuíram para o desenvolvimento do TCC. Agradecemos também à mentora do grupo (Giovanna Moreira) pelas dicas e auxílios no desenvolvimento do TCC.

Agradecemos à professora Juliana Aguiar e à instituição Escola da Nuvem por proporcionarem todo o conhecimento e embasamento sobre a AWS e suas soluções.

Obrigado a todos que contribuíram para o sucesso deste projeto!



