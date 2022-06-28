## Anotações Reuniões prof. Bruno
[Memória](https://fragrant-acoustic-8d1.notion.site/Mem-ria-Reuni-es-Wesley-PHD-01872e68357d4af9bce0dce1ef60445e)



## Códigos e arquiteturas desenvolvidas para aprendizagem - P4



### [1] - Topologia-1-Estrela. 4 hosts, 1 switch
![](https://raw.githubusercontent.com/wesleytessaro/Cmbr-DT/main/%5B1%5D%20-%20Topologia-1-Estrela/pod-topo/Topologia1.jpg)

#### Como executar

Dentro da pasta [1] - Topologia-1-Estrela

Executar o mininet
```sh
make run
```

Testar a conectividade com todos os hosts
ex.
```sh
pingall
```

ou 
```sh
h1 ping h2
```


### [2] -Topologia-2-Caminhos Estáticos
![](https://github.com/wesleytessaro/Cmbr-DT/blob/main/%5B2%5D%20-Topologia-2-Caminhos%20Est%C3%A1ticos/Caminhos.jpg)


#### Como executar

Dentro da pasta [2] -Topologia-2-Caminhos Estáticos

Executar o mininet
```sh
make run
```

Abrir o xterm para h1 e h3
ex.
```sh
xterm h1 h3
```

Ao abrir, dentro do xterm h3 abrir o receive.py
ou 
```sh
./receive.py
```

Ao abrir, dentro do xterm h1 abrir o send.py para 10.0.3.1
```sh
./send.py 10.0.3.1

2 2 2
```

### [3] - Tuneis + P4Runtime
![](https://github.com/wesleytessaro/Cmbr-DT/blob/main/%5B3%5D%20-%20P4Runtime/Esquematico.drawio2.png)


#### Como executar

Dentro da pasta [3] - P4Runtime

Executar o mininet
```sh
sudo make
```

ex. Testar o ping entre h1 -> h2
```sh
h1 ping h2
```

ex. Testar o ping entre h1 -> h3
```sh
h1 ping h3
```

Em outro terminal, executar o arquivo mycontroller.py. Verificar se as regras foram escritas nos switches
```sh
sudo ./mycontroller.py
```


