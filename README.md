# dbt_snapshots

sudo apt-get install python3-venv
python3 -m venv myenv #to create env
source myenv/bin/activate  #TO ACTIVATE env
pip install dbt-postgres~=1.5.2
pip install dbt-core~=1.5.2
dbt init : project_name : pipeline_snapshot
sudo vi ~/.dbt/profiles.yml  add info about db
create snapshot file
create schema.yml (info about table & source) ## error source undefined ..


add : dags_are_paused_at_creation = True
Airflow consist of several components: Workers - Execute the assigned tasks. Scheduler - Responsible for adding the necessary tasks to the queue.

![image](https://github.com/IkramKheopsys/dbt_snapshots/assets/113558455/b04497b1-c2ae-4f29-b8a9-507bc742b93e)
docker build -t dbt-snapshot .
docker tag dbt-snapshot gcr.io/kheopsys-lab/dbt-snapshot:alpha 
docker push gcr.io/kheopsys-lab/dbt-snapshot:alpha

docker build -t dbt-snapshot4 .
docker tag dbt-snapshot4 gcr.io/kheopsys-lab/dbt-snapshot:alpha.1.4
docker push gcr.io/kheopsys-lab/dbt-snapshot:alpha.1.4
