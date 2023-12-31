# dbt Test Results Analytics

This example Meltano project, built as a Matatika workspace for the [Matatika CE](https://github.com/Matatika/matatika-ce), is a quick and easy way to get started with insights into your dbt test results.

[![IMAGE ALT TEXT](http://img.youtube.com/vi/KLX4sNqvVIk/3.jpg)](https://www.youtube.com/watch?v=KLX4sNqvVIk "Matatika GitHub Analytics Project")

---

## Prerequisites

**NB - Currently this project is only supported to work on Linux and MacOS**

1. Get Docker - [https://docs.docker.com/get-docker/](https://docs.docker.com/get-docker/)

---

## From 0 to ELT in seconds

Using Matatika you can run this example with only docker and we create all the following for you:
- Postgres data warehouse
- Preconfigured pipelines to get example data then run dbt models and tests
- Lab (UI for Meltano) to run and schedule pipelines
- Simple charts that can be embedded anywhere [https://github.com/Matatika/dataset-component-example](https://github.com/Matatika/dataset-component-example)

### Steps

1. [Clone and start Matatika CE](https://github.com/Matatika/matatika-ce#how-to-get-started)

2. Clone this repository into the `matatika-ce/workspaces` directory

3. Once [Matatika CE](https://github.com/Matatika/matatika-ce) is started and your workspace is deployed, login to the Lab [https://localhost:3443](https://localhost:3443)

4. Run the `IMDB Data` Pipeline by clicking the Play button.

    This pipeline will bring in some example data from our example repo: [imdb_top_20_films.csv](https://github.com/Matatika/matatika-examples/blob/master/example_adding_a_custom_data_source/imdb_top_20_films.csv), and create a dbt model. 

    The model it created can be found in the `transforms/models` directory in this workspace. 

    We have also included some test for this model so everything in this example is easy to use and understand.

5. Once the `IMDB Data` pipeline has completed, run the `Model Validation` pipeline.

    This pipeline will run the dbt tests in your workspace, and store them as data in your workspace's database. Then using this data we build dbt models to report from.

6. Once the `Model Validation` pipeline is complete, in the bottom left click `Switch To App` to see insights into your dbt test results.

---

### Support

Join our community on the [Matatika Slack](https://join.slack.com/t/matatika/shared_invite/zt-19n1bfokx-F31DNitTpSxWCFO2aFlgxg) to get help and updates.

You can read more about Matatika and our Lab in our [Documentation](https://www.matatika.com/docs/).
