# ES|QL Visual Studio Code Extension

Use the [Elasticsearch Query Language](https://www.elastic.co/guide/en/elasticsearch/reference/master/esql.html) in VSCode notebooks and text files.

This extension is a fork of [Kusto Notebooks](https://marketplace.visualstudio.com/items?itemName=donjayamanne.kusto). It is not supported or maintained by Elastic but is a proof-of-concept designed to explore live editing features similar to those of Kusto. The goal of this project is to learn more about ES|QL and learn about its possible uses outside of a web browser.

<img src=https://raw.githubusercontent.com/notebookPowerTools/vscode-kusto/main/images/interactive_window.gif>

<img src=https://raw.githubusercontent.com/notebookPowerTools/vscode-kusto/main/images/notebook.gif>

<img src=https://raw.githubusercontent.com/notebookPowerTools/vscode-kusto/main/images/clusters.png>

# Features

* Run ES|QL Queries
* Graphs & Data Viewer
* Code Completion
* Syntax highlighting
* Code refactoring
* Code formatting
* Elasticsearch panel with access to Clusters, Indexes, etc
* Run ES|QL queries in Plain text files, Notebooks or in an Interactive Window

# Getting Started

* Open a `*.esql` file and start typing to get code completion.
* Open a `*.esql` file and click on the `Run Query` code lense
* Open a `*.esql` file as a notebook
* Create a file with extension `*.esqlnb` (or use the command `Create ES|QL Notebook`)
* Use the command `Configure Elasticsearch Connection` to configure the Elasticsearch connection.

# Works with Jupyter Notebooks as well (when using [kqlmagic](https://pypi.org/project/Kqlmagic/))
* This extension augments Jupyter Notebooks with Kusto language features, when using the [Jupyter](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter) extension.
* The extension will automatically detect the cluster and database from cells containing the connection information `kql AzureDataExplorer://code;cluster='help';database='Samples'`.

# Difference between Kusto Notebooks & Jupyter Notebooks  (with [kqlmagic](https://pypi.org/project/Kqlmagic/))
* Kusto Notebooks, there are no additional dependencies.
    * Authentication against Azure is handled by VS Code.
* With Jupyter Notebooks, you'll need to install Python and the [kqlmagic](https://pypi.org/project/Kqlmagic/) package.
    * You can use Python to further analyze the data.

# Roadmap

```[tasklist]
* [ ] Relicense to Elastic License
* [ ] Replace Azure connection with Elasticsearch connection
* [ ] Rename all the kustos
* [ ] Replace the kusto language logic with https://github.com/smith/kibana/tree/afd020c63da1aff540b778e2e4303723ee15e00d/packages/kbn-monaco/src/esql
* [ ] Replace react table with EUI data grid
* [ ] Replace plotly with Elastic charts
* [ ]Implement render function https://learn.microsoft.com/en-us/azure/data-explorer/kusto/query/renderoperator?pivots=azuredataexplorer
```

# Thanks to the contributors
[Don Jayamanne](https://github.com/DonJayamanne),
[Joyce Er](https://github.com/joyceerhl),
[SteVen Batten](https://github.com/sbatten),
[Peng Lyu](https://github.com/rebornix),
[Tanha Kabir](https://github.com/tanhakabir)

# License

MIT
