#  Load Test 

## 1.Descrição

O **_load Test_** Surgiu devido à necessidade de fazer validações com Testes De Performance.


## 2.Preparação para Desenvolvimento
    
   - Instale o Docker : https://docs.docker.com/engine/install/ubuntu/

   - Suba o banco de dados influxDB e o Grafana : sudo docker-compose up -d influxdb grafana
   - Rode os testes : sudo docker-compose run k6 run /scripts/conexaoQA.js
    
   - Url do dashboard grafana : http://localhost:3000/d/k6/k6-load-testing-results?orgId=1&refresh=5s


   - Derruba os containers : sudo docker-compose down

### 3. Atenção

- caso a porta 3000 estiver sendo usada, favor altera e abrir novamente.
