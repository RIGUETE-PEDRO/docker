<h2>aprendendo sobre o docker</h2>
<h4>Docker é uma plataforma de contêinerização que permite empacotar, distribuir e executar aplicações de maneira isolada e portátil. Ele facilita a criação de ambientes leves e consistentes para o desenvolvimento e a execução de software.</h4>

<h4>comando do docker</h4>

<div>
<p>docker images</p>
<p>comando para ver as imagens intaladar </p>
</div>
<br>

<div>
<p>docker pull ubuntu</p>
<p>comando para baixar o ambiente ubuntu tambem usado para baixar node como outras coisas tambem podemos colocar a versao na frente assim exemplo (docker pull node:14.21.1-alpine) </p>
</div>

<div>
<p>docker rmi (nome da imagem) </p>
<p>com esse comadno desistalamos a imagem do docker</p>
</div>

<div>
<p>docker run -it (nome da imagem) </p>
<p>com esse comando rodamos a imagem do docker de forma interativa</p>
</div> 

<div>
<p>docker stop (nome da imagem) </p>
<p>com esse comando paramos a imagem do docker</p>
</div> 

<div>
<p>docker ps  </p>
<p>com esse comando vemos os conteines funcionando e tambem vemos nome id e quando foi criado</p>
</div> 

<div>
<p>docker ps -a  </p>
<p>com esse comando vemos todos os conteines e tambem vemos nome id e quando foi criado e quanto foram terminados</p>
</div> 

<div>
<p>docker rm $(docker ps -f status=exited -q)</p>
<p>comando para encerrar todo os que a gente saiu usando exit</p>
<p>docker ps -f status=exited -q  </p>
<p>com esse comando vemos todos os conteines que foram exit,podendo usar o nomes deles para voltar dps</p>
</div> 

<div>
<p>docker rm (nome do conteiner) </p>
<p>com esse comando apagamos o conteiner atravez do nome dele </p>
</div> 

<div>
<p>docker run -d --name (nome do conteiner) ubuntu  </p>
<p>com esse comando criamos um conteiner com o nome que  escolhermos </p>
</div> 