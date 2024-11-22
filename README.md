# redirectUrlShortener
Projeto desenvolvido com o curso gratuito de Java da Rockseat, onde é realizada a criação de uma função que ira encurtar URL de paginas, codificando e armazenando as requisições dentro de um S3 da AWS. 

Esse arquivo corresponde a uma função lambda 'RedirectUrlShortenet' que é responsável por recuperar as informações de originalUrl e expirationTime, que estão armazenadas dentro dos objetos no bucket da AWS. Essa lambda é acionada quando o codigo obtido do retorno da função 'GenerateShortnerUrl' é incerido no endereço da api. O API Gateway será responsavel por direcionar as requisições para o local correto, utilizando o urlCode para redirecionar ao Url encurtado

https://7nkukb0h4c.execute-api.us-east-1.amazonaws.com/{urlCode}
