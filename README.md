# Orquestração de Containers com Kubernetes

1. O que é um POD? <br>
   R: POD em Kubernetes é a menor unidade de computação publicável em um computador que podemos criar e gerenciar. <br>
   O Kubernetes faz acesso ao POD e não ao container diretamente

2. O que é um Replication Controller e ReplicaSets? <br>
   R: Nos ajuda a executar múltiplas instâncias de um pod/container no nosso cluster Kubernets. Ele faz isso replicando o pod/container existente.

3. O que é o Deployments? <br>
   R: O Deployment, "encapsula" todo processo de criação de PODs e ReplicaSets 

4. O que é o Namespace? <br>
   R: Namespace é um "espaço" na qual separamos nossos recursos dentro do Kubernetes em áreas separadas.

5. O que é o Service? <br>
   R: Services em Kubernetes permite a comunicação entre os diversos componentes de uma aplicação com o mundo externo á ela.
   Além disso permite que possamos conectar facilmente uma aplicação com outra e claro com usuários externos.

6. Para criar todos os recursos de uma única vez, utilizar: 
   ```
   kubectl create -f .\deployments\ --save-config --record
   ```
7. Pegando IP dos Services 
   ```
   minikube service result --url -n vote
   ```