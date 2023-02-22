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
