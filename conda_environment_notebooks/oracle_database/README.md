Oracle Database Conda Environment Family Notebooks
==================================================

The [Oracle Database conda environment family](https://docs.oracle.com/en-us/iaas/data-science/using/conda-database-fam.htm) is focused on the tools that are needed to interact with databases in general. However, there is an emphasis on using the Oracle Autonomous Databases. This [conda environment](https://docs.cloud.oracle.com/en-us/iaas/data-science/using/use-notebook-sessions.htm#conda_understand_environments) enables you to work seamlessly with Oracle Databases using the ADS [database connection module](https://docs.oracle.com/en-us/iaas/tools/ads-sdk/latest/ads.database.html#ads.database.connection.Connector), `SQLAlchemy` and `ipython-sql`. Use a notebook to create ETL jobs, batch transform data, and perform database queries. The ADS Connector provides a uniform interface to connect to databases. The conda includes support for Oracle Database, MySQL, and SQLite. However, other databases can be used with little to no modification to the conda environment. The `ipython-sql` magic extension (`%sql` or `%%sql`) allows you to connect to various databases and issue SQL commands directly in a notebook cell. You can build ETL jobs or integrate the results into your Python code.

The notebooks in this folder are meant to be run in the [Oracle Database conda environment family](https://docs.oracle.com/en-us/iaas/data-science/using/conda-database-fam.htm) conda environments.

# Notebook Descriptions

* `autonomous_database.ipynb`: This notebook demonstrates how to connect to an Oracle Autonomous Database (ADB) and perform popular CRUD operations. Oracle offers two types of ADB, the Autonomous Data Warehouse (ADW) and the Autonomous Transaction Processing (ATP) databases. In general, there are no differences in how a connection is made to these different types of databases. This notebook introduces how to pull data from an ADB into a notebook. It also demonstrates how to write generic SQL queries in the notebook and several ways to connect.
* `sqlmagic.ipynb`: This notebook demonstrates how to use SQL Magic to work with a database. Magic commands are a set of functions that are not valid Python code but can be run and executed in Jupyter Notebooks. There are two types of magic commands, line magics and cell magics. Line magics start with `%` and operate on a single line of input. Cell magics start with `%%`, and they work on multiple lines in a call. IPython SQL magic extension allows you to directly write SQL queries in Jupyter notebook cells.

