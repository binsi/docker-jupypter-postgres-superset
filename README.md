# docker-jupypter-postgres-superset
A quick-to-setup docker architecture for data scientists with jupyter, postgres and superset

If you want to start the docker environment (jupyter, postgres, superset):
- in the same directory as the Dockerfile run $docker-compose up -d 
- Get URL+token for jupyter from $docker-compose logs jupyter
- Jupyter is running on port 8888, Superset on 8088 (credentials: admin/superset) and postgres on port 5432
- To enable a conversation between jupyter and postgres, start a terminal within the jupyter container and run $pip install psycopg2-binary
- Use the ipython notebook "proof-of-success" to test connection 
- Ta-da!
