# kubernetes-task
Deploy a new container of SuperSet and airflow application with service


# Summary
- 1 Deploy a new container of SuperSet application
- 2  Create service for it and expose it
- 3 Do it with YAML and with scripted way
- 4 Deploy also Airflow application and expose it
- 5 Deploy jenkins with master and slave using helm chart



# solution
- 1 kubectl create deployment superset --image=amancevice/superset
- 2 kubectl expose deployment superset --type=NodePort --port=8088
![image](https://user-images.githubusercontent.com/113102456/211503621-674e65c0-ac2d-4ad5-b709-13d95f9bb973.png)
![image](https://user-images.githubusercontent.com/113102456/211503674-e9336d2d-70cd-4a9e-bcf7-0ec681097ae8.png)
- 3 
- 3.1 ![image](https://user-images.githubusercontent.com/113102456/220575952-15b9435e-71b7-435b-a499-2ac31a3925e1.png)
- 3.2 ![image](https://user-images.githubusercontent.com/113102456/220576015-ab5a3cb5-1aad-4bd9-bbfd-24727ed9c312.png)
- 4 
- Deploy:
- kubectl create deployment airflow --image=puckel/docker-airflow
- Expose:
- kubectl expose deployment airflow --type=NodePort --port=8088
- 5
