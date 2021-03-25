<!--
Author: Amy Coughlin, A Cloud Guru, 2021
This is free and unencumbered software released into the public domain.
http://unlicense.org/ 
-->
<html>
<head>
	<title>A Cloud Guru DP-900 Azure Data Fundamentals Bingo</title>
	
	<style>
	h2 {color:white;text-align:center;padding:10px;border:1px solid green;}
	body {background:rgb(6,12,89);font-family:Verdana;margin-left:20px;margin-right:20px;color:white}
	td {

		height: 120px;
		width: 120px;
		text-align: center;
		vertical-align: middle;
		border-top:1px solid lightgray;
		border-left:1px solid lightgray;
		border-bottom:1px solid darkgray;
		border-right:1px solid darkgray;
	}
	.noJavascript {
		background-color:#FF7F7F;
		color:red;
		padding:5px;
		margin:20px 50px;
		border:1px solid red;
	}
	.selectedOn {
		background:#00CB85;
	}
	.selectedOff { 
		background: transparent;
	}

	.grid-container {
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-gap: 20px;
	}

	a { 
		color:#5A80FC;
	}
	h3 {
		color:#FC8918;
	}
	td label { 
		cursor:pointer;
	}
	input[type=radio]:checked {
  		outline: 3px solid #FC8918;     
	} 
	form { 
		margin:5px;
		padding:5px;
		color:#00CB85;
	}

	#instructions {
		display:none;
		border: 1px solid #00CB85;
		margin:10px;
		padding:20px;
	}
	</style>
	
	<script type="text/javascript">
/* 		dictionary objects, each with 25 terms and definitions -- 
		fill in with "Bingo Free Space 1": "",  "Bingo Free Space 2": "", etc. as necessary to get 25.
		  ***Be sure to escape quotes in definitions with \" and remove the final comma at the end of the if copy-pasting
		Alter game button parameters to point to the correct dictionary object
*/
		gameA = {
			"ARM Templates": "\"Infrastructure as code,\" written in JSON to define and configure Azure resources",
			"Azure CLI": "A command-line language that can be used in a Bash shell to interact with Azure data resources",
			"Non-Relational": "A data storage resource that stores semi-structured data or non-structured data",
			"Visualization": "A data technique that translates information into a visual context to make it easier to understand and gain insights",
			"PowerShell": "A scripting language that has many uses, among them, interacting with Azure data resources.",
			"Big Data": "A term that has come to refer to massive amounts of data that is produced in large volumes, at high speed, with a lot of variety in terms of form or content.",
			"Graph": "A type of database made up of nodes and edges, which is particularly well-suited to to  social networking applications and certain scientific applications",
			"JSON": "A type of semi-structured data in human-readable form and stored on \"documents\"; similar in nature to XML and YAML",
			"Cloud Shell": "A web based command-line terminal resource, accessible from the Azure Portal",
			"Deploy": "After provisinging the storage account or underlying database insfrastructure, a database administrator or a data engineer will ______ specific resources into that infrastructure.",
			"Wide-Column": "Also known as column-family, this type of database stores tables with rows, where a different set of columns can be defined for each row",
			"Unstructured": "Data that has no defined structure, often referred to as \"blobs\" but may, nonetheless include metadata associated with files such as PDFs, images, and videos.",
			"Semi-Structured": "Data that is flexibly organized around entities that can have varying types and amounts of associated descriptive data and hierarchical data per defined entity",
			"Structured": "Data that is highly-organized, with strong rules around the type, form, and format of the stored data. This type of data is very tightly associated with relational databases",
			"Data Engineer": "Data wrangling and implementing data-driven artificial intelligence solutions both fall within the many possible specializations undertaken by this data professional.",
			"Data Analyst": "Exploring and analyzing data and building business-friendly data models falls under the responsibilitys of this data professional.",
			"Analytics Workload": "Larger, richer data sets optimized for decision support and complex questions posed of the data.",
			"SQL": "Many data sources can be queried by by some variant of this declarative language.",
			"Transactional Workload": "Operational data that is processed in short, precise, isolated actions. Optimized for speed and accuracy within the interaction.",
			"Key-Value": "Semi-structured format, where entities are organized into tables with rows uniquely identified by a key and a flexible number of columns;  similar to wide-column data format",
			"Provision": "The act of setting up the underlying infrastructure of a cloud data resource",
			"Database Administrator": "This data professional will often be responsible for setting up database security and cyrption configurations as well as managing and monitoring IaaS infrastructure.",
			"Data Lake": "This resource captures real-time and external data -- often both relational and non-relational -- into an organized data store that can be queried directly.",
			"Modern Data Warehouse": "This resource combines internal and eternal data in multiple forms into a unified solution for analytics.",
			"Relational": "Type of database where structured data is organized in to tables with rows and columns, where each row is an entity, with pre-defined columns that are the same for every row"
		};
		
		gameB = {
			"Consistency": "A data concept that describes how well or how quickly data is kept \"in sync\" with itself and with replicas of itself.",
			"Primary Key": "A data construct made up of one or more bits of data that uniquely identify an entity in a data store; examples include a key on a row in a table, or a key on a JSON document",
			"Non-Relational": "A data storage resource that stores semi-structured data or non-structured data",
			"Schema-on-read": "A hallmark of semi-structured data, where the desired form of the returned data is determined by the query",
			"Schema-on-write": "A hallmark of structured, relational data, where the desired form of the data is determined ahead of time and enforced when the data is written to the data tables",
			"Partition Key": "A key in certain types of data resources that buckets multiple items, which could be rows or documents, under a particular category or common filter value",
			"Graph": "A type of database made up of nodes and edges, which is particularly well-suited to to  social networking applications and certain scientific applications",
			"Column-Family": "A type of database that stores tables with rows, where a different set of columns can be defined for each row; also referred to as a wide-column database.",
			"IaaS": "Acronym that describes the form of Azure service provided by SQL Server on a virtual machine.",
			"OLAP": "An acronym describing a type of data workload that is most appropriate for decision support and business intelligence.",
			"OLTP": "An acronym describing a type of data workload that is most appropriate for operational data interactions.",
			"Unstructured": "Data that has no defined structure, often referred to as \"blobs\" but may, nonetheless include metadata associated with files such as PDFs, images, and videos.",
			"Semi-Structured": "Data that is flexibly organized around entities that can have varying types and amounts of associated descriptive data and hierarchical data per defined entity",
			"Structured": "Data that is highly-organized, with strong rules around the type, form, and format of the stored data. This type of data is very tightly associated with relational databases",
			"API": "Describes a means for other systems or humans to interact with a resource, such as a cloud database, using an \"interface\" that hides the complexity of the source system ",
			"Business Intelligence": "Describes the use of computing and data resources to aid the identification, discovery and analysis of critical business data",
			"Nodes and Edges": "In graph databases, Entities and Relationships are also referred to as these two terms.",
			"Row Key": "Key-value data resources can combine this with the partition key to form a primary key, which enables fast retrieval of individual entities in a table.",
			"Analytics Workload": "Larger, richer data sets optimized for decision support and complex questions posed of the data.",
			"SQL": "Many data sources can be queried by by some variant of this declarative language.",
			"PaaS": "Most, but not all, Azure data services fall under the _____ service category, where Azure handles most of the administrative tasks of patching, backups, OS updates and so on.",
			"Transactional Workload": "Operational data that is processed in short, precise, isolated actions. Optimized for speed and accuracy within the interaction.",
			"Key-Value": "Semi-structured format, where entities are organized into tables with rows uniquely identified by a key and a flexible number of columns;  similar to wide-column data format",
			"Relational": "Type of database where structured data is organized in to tables with rows and columns, where each row is an entity, with pre-defined columns that are the same for every row",
			"Querying": "Writing code or interacting with a UI to \"read\" data from one or more data sources and return the requested data in a particular form or format"
		};
		gameC = {
			"Eventual Consistency": "A database configuration that favors fast performance over ensuring that data sources are in perfect sync at all times.",
			"Azure Data Lake Storage Gen2": "A form of blob storage optimized for analytics support with a hierarchical folder structure and able to store both relational and non-relational data",
			"Partition Key": "A key in certain types of data resources that buckets multiple items, which could be rows or documents, under a particular category or common filter value",
			"Big Data": "A term that has come to refer to massive amounts of data that is produced in large volumes, at high speed, with a lot of variety in terms of form or content.",
			"Azure Storage Explorer": "A tool designed to manage data stored in a wide variety of formats in Azure using a familiar interface.",
			"AZCopy": "A tool designed to move large volumes of data in and out of Azure Storage",
			"Cloud Shell": "A web based command-line terminal resource, accessible from the Azure Portal",
			"SMB": "A Windows system protocol for file sharing that allows applications to read and write to files over network connected computers",
			"IaaS": "Acronym that describes the form of Azure service provided by SQL Server on a virtual machine.",
			"Azure Blob Storage": "An Azure data resource well suited for storing and serving up unstructured data in the form of images, videos and PDFs",
			"Azure Table Storage": "An Azure storage resource that employs the key-value type of semi-structured data",
			"Azure Files": "Azure data resource that mimicks on-premises file shares and allows applications and humans to interact with it the same way they do on servers and desktop computers",
			"Unstructured": "Data that has no defined structure, often referred to as \"blobs\" but may, nonetheless include metadata associated with files such as PDFs, images, and videos.",
			"Semi-Structured": "Data that is flexibly organized around entities that can have varying types and amounts of associated descriptive data and hierarchical data per defined entity",
			"API": "Describes a means for other systems or humans to interact with a resource, such as a cloud database, using an \"interface\" that hides the complexity of the source system ",
			"Concurrency": "Describes the operation and impact on data when more than one human or system is operating over the same data at the same time.",
			"Document": "In a data sense, this describes a data container that stores human-readable, semi-structured data in the form of JSON, XML, YAML, and others.",
			"Row Key": "Key-value data resources can combine this with the partition key to form a primary key, which enables fast retrieval of individual entities in a table.",
			"NoSQL": "Often used interchangably with the term \"non-relational.\"",
			"Key-Value": "Semi-structured format, where entities are organized into tables with rows uniquely identified by a key and a flexible number of columns;  similar to wide-column data format",
			"Encryption": "The process of encoding data such that it can be interpreted by a system or human consumer only if they have a key is passed etween the source and the requester",
			"Data Lake": "This resource captures real-time and external data -- often both relational and non-relational -- into an organized data store that can be queried directly.",
			"Consistency": "A data concept that describes how well or how quickly data is kept \"in sync\" with itself and with replicas of itself.",
			"Primary Key": "A data construct made up of one or more bits of data that uniquely identify an entity in a data store; examples include a key on a row in a table, or a key on a JSON document",
			"Non-Relational": "A data storage resource that stores semi-structured data or non-structured data"
		};
		gameD = {
			"ARM Templates": "\"Infrastructure as code,\" written in JSON to define and configure Azure resources",
			"Azure CLI": "A command-line language that can be used in a Bash shell to interact with Azure data resources",
			"Partition Key": "A key in certain types of data resources that buckets multiple items, which could be rows or documents, under a particular category or common filter value",
			"Attribute Based Access Control": "A more granular form of access control that provides access rights based on user, environment, or resource attributes",
			"VNet": "A network in Azure that mimicks the form of on-premises, hardware-based networks",
			"Bash": "A popular shell language that can run Azure CLI commands",
			"TLS": "A protocol that protects data in motion, for example, traveling between the cloud services and customers.",
			"PowerShell": "A scripting language that has many uses, among them, interacting with Azure data resources.",
			"Firewall": "A security device, in the form of software or hardware, that filters traffic to resources, such as databases",
			"Transparent Encryption": "A security feature that protects an entire database file (data at rest) so that it cannot be read unless the host application is secured using the same key.",
			"Access": "A security-related concept that describes what entities can interact with which systems and what they can do during those interactions",
			"Authentication": "A security-related process where a human user or a system is confirmed to be who they say they are",
			"JSON": "A type of semi-structured data in human-readable form and stored on \"documents\"; similar in nature to XML and YAML",
			"Cloud Shell": "A web based command-line terminal resource, accessible from the Azure Portal",
			"IaaS": "Acronym that describes the form of Azure service provided by SQL Server on a virtual machine.",
			"Deploy": "After provisinging the storage account or underlying database insfrastructure, a database administrator or a data engineer will ______ specific resources into that infrastructure.",
			"RBAC": "An acronym describing a form of access control that depends on putting users in groups, or roles, and providing permissions to those groups, rather than individually to users",
			"PaaS": "Most, but not all, Azure data services fall under the _____ service category, where Azure handles most of the administrative tasks of patching, backups, OS updates and so on.",
			"Transactional Workload": "Operational data that is processed in short, precise, isolated actions. Optimized for speed and accuracy within the interaction.",
			"Provision": "The act of setting up the underlying infrastructure of a cloud data resource",
			"Encryption": "The process of encoding data such that it can be interpreted by a system or human consumer only if they have a key is passed etween the source and the requester",
			"Database Administrator": "This data professional will often be responsible for setting up database security and cyrption configurations as well as managing and monitoring IaaS infrastructure.",
			"Redundancy": "This term has two meanings in the data realm: 1) The existence of the same piece of data in more than one place, which is acceptable -- even optimal in some systems -- but not in others and 2) A form of replication of cloud assets than improve accessibility and disaster recovery.",
			"Private Link": "Use this service to bring certain PaaS services hosted on Azure into your private virtual network.",
			"Bingo Free Space 1": ""
		};
		gameE = {
			"Index": " A data structure that copies and re-orders data or contains pointers to data to improve the speed of data retrieval operations, often at the cost of speed for write operations",
			"Azure SQL Managed Instance": "A cloud-based PaaS offering that is as compatible as possible with the full Microsoft SQL Server platform while still providing the benefits of a fully managed service.",
			"Consistency": "A data concept that describes how well or how quickly data is kept \"in sync\" with itself and with replicas of itself.",
			"Primary Key": "A data construct made up of one or more bits of data that uniquely identify an entity in a data store; examples include a key on a row in a table, or a key on a JSON document",
			"Schema-on-write": "A hallmark of structured, relational data, where the desired form of the data is determined ahead of time and enforced when the data is written to the data tables",
			"Normalization": "A process of organizing data into tables and establishing relationships between those tables in a way designed both to protect the data and to make the database more flexible.",
			"ACID": "Acronym that describes a set of database properties that intend to guarantee data validity despite errors, power failures, concurrent use and other risks to data integrity",
			"OLTP": "An acronym describing a type of data workload that is most appropriate for operational data interactions.",
			"Azure Database for PostgreSQL": "An Azure PaaS offering that is based on the community edition of a relational database that offers many of the advanced features only otherwise found in Azure SQL Database",
			"SQL Server on Virtual Machine": "An IaaS relational database service offered in Azure",
			"Azure Database for MySQL": "Azure PaaS offering that is based on the community edition of a popular open source database, with with some of the advanced features of the Oracle enterprise edition.",
			"Azure SQL Database": "Azure's cornerstone PaaS relational data resource, available in multiple configurations from a single database to databases that approach full Microsof SQL Server capabilities",
			"Azure Data Studio": "Cross-platform database tool for data professionals using on-premises and cloud data platforms on Windows, macOS, and Linux.",
			"Concurrency": "Describes the operation and impact on data when more than one human or system is operating over the same data at the same time.",
			"SQL": "Many data sources can be queried by by some variant of this declarative language.",
			"PaaS": "Most, but not all, Azure data services fall under the _____ service category, where Azure handles most of the administrative tasks of patching, backups, OS updates and so on.",
			"Transactional Workload": "Operational data that is processed in short, precise, isolated actions. Optimized for speed and accuracy within the interaction.",
			"Stored Procedures": "Prepared database code that you can save, so the code can be reused, often with improved performance over ad hoc code.",
			"Azure Database for MariaDB": "Relational database service in the Microsoft cloud that supports multiple tiers of the community edition, which was orignially forked off of MySQL",
			"Azure SQL Elastic Pools": "Solution for managing and scaling multiple Azure SQL databases that have varying and unpredictable usage demands by flexibly sharing set resources on a single server",
			"3NF Data Model": "The most commonly applied data model form employed in relational databases optimized for transactional workloads",
			"Redundancy": "This term has two meanings in the data realm: 1) The existence of the same piece of data in more than one place, which is acceptable -- even optimal in some systems -- but not in others and 2) A form of replication of cloud assets than improve accessibility and disaster recovery.",
			"SSMS": "Tool used to manage and query databases using both UI features and T-SQL code",
			"Relational": "Type of database where structured data is organized in to tables with rows and columns, where each row is an entity, with pre-defined columns that are the same for every row",
			"Querying": "Writing code or interacting with a UI to \"read\" data from one or more data sources and return the requested data in a particular form or format"
		};
		gameF = {
			"Non-Relational": "A data storage resource that stores semi-structured data or non-structured data",
			"Eventual Consistency": "A database configuration that favors fast performance over ensuring that data sources are in perfect sync at all times.",
			"Multi-Model": "A database that can support more than one data format",
			"Schema-on-read": "A hallmark of semi-structured data, where the desired form of the returned data is determined by the query",
			"Partition Key": "A key in certain types of data resources that buckets multiple items, which could be rows or documents, under a particular category or common filter value",
			"Gremlin": "A language used for querying/traversing across the a graph data source",
			"Firewall": "A security device, in the form of software or hardware, that filters traffic to resources, such as databases",
			"Graph": "A type of database made up of nodes and edges, which is particularly well-suited to to  social networking applications and certain scientific applications",
			"JSON": "A type of semi-structured data in human-readable form and stored on \"documents\"; similar in nature to XML and YAML",
			"Cassandra": "A wide-column database that is supported on Azure through a Cosmos DB API",
			"Wide-Column": "Also known as column-family, this type of database stores tables with rows, where a different set of columns can be defined for each row",
			"Azure Table Storage": "An Azure storage resource that employs the key-value type of semi-structured data",
			"MongoDB": "BSON document database that is supported on Azure through a Cosmos DB API",
			"Semi-Structured": "Data that is flexibly organized around entities that can have varying types and amounts of associated descriptive data and hierarchical data per defined entity",
			"API": "Describes a means for other systems or humans to interact with a resource, such as a cloud database, using an \"interface\" that hides the complexity of the source system ",
			"Index": " A data structure that copies and re-orders data or contains pointers to data to improve the speed of data retrieval operations, often at the cost of speed for write operations",
			"Consistency": "A data concept that describes how well or how quickly data is kept \"in sync\" with itself and with replicas of itself.",
			"Concurrency": "Describes the operation and impact on data when more than one human or system is operating over the same data at the same time.",
			"Document": "In a data sense, this describes a data container that stores human-readable, semi-structured data in the form of JSON, XML, YAML, and others.",
			"Nodes and Edges": "In graph databases, Entities and Relationships are also referred to as these two terms.",
			"PaaS": "Most, but not all, Azure data services fall under the _____ service category, where Azure handles most of the administrative tasks of patching, backups, OS updates and so on.",
			"Cosmos DB": "Multi-model database designed for global distribution and high performance",
			"Key-Value": "Semi-structured format, where entities are organized into tables with rows uniquely identified by a key and a flexible number of columns;  similar to wide-column data format",
			"SQL/Core API": "The primary interface for interacting with Cosmos DB",
			"Redundancy": "This term has two meanings in the data realm: 1) The existence of the same piece of data in more than one place, which is acceptable -- even optimal in some systems -- but not in others and 2) A form of replication of cloud assets than improve accessibility and disaster recovery."
		};
		gameG = {
			"Azure Data Lake Storage Gen2": "A form of blob storage optimized for analytics support with a hierarchical folder structure and able to store both relational and non-relational data",
			"U-SQL": "A language used for batch jobs over large amounts of data in Azure Data Lake Analytics",
			"OLAP": "An acronym describing a type of data workload that is most appropriate for decision support and business intelligence.",
			"Azure Databricks": "Analytics service built on Apache Spark that supports data processing, machine learining and analytics via code in notebooks using SQL, R, Python and Scala",
			"Azure Analytics Service": "Based on SQL Server Analytics, an analytics service that operates over tabular and dimensional data models",
			"Streaming Workload": "Data is gathered an processed very near to the time it is generated, from micro-seconds to a few minutes, such that the data is delivered in a near continuious fashion.",
			"Batch Workload": "Data is gathered from one or more sources at regular intervals, usually measured in hours or days, and processed all the same time.",
			"Data Factory": "Data processing service in Azure that provides a UI to orchestrate and data processing activities; Syanpse Pipelines are built on the same platform as this resource",
			"Star Data Model": "Denormalized analytics data model that centers on fact tables, with dimension tables directly related to the facts",
			"PolyBase": "Feature in Synapse Analytics that allows direct loading of data in other forms and formats, such as blobs in parquet format, using T-SQL",
			"Analytics Workload": "Larger, richer data sets optimized for decision support and complex questions posed of the data.",
			"Azure Synapse Analytics": "Modern data warehouse and analytics service, based on SQL Data Warehouse, but that also includes Spark technolgies and deep integration with other big data resources",
			"ETL": "One of two major approaches to data processing that performs the transformation in memory or in a staging environment before the final load into the destination data store",
			"ELT": "One of two major approaches to data processing that performs the transformation step within the final storage destination",
			"Dimension": "One of two primary table types in star and snowflacke data models, this tble type often represents people, places, objects, and time",
			"Fact": "One of two primary table types in star and snowflake data models, this table type often represents events or activities of the data, such as invoices or medical claims",
			"Apache Spark": "Open-source analytics engine used for big data processing",
			"Azure HDInsight": "Open-source big data processing service, similar in purpose to Azure Synapse analytics",
			"Pipeline": "Primary orchestration structure for Data Factory, which organizes activities over data sets into a logical workflow",
			"Ingestion": "Process of pulling data into a data platform environment from multiple sources, via either batch processing or stream processing",
			"Snowflake Data Model": "Semi-normalized analytics data model that centers on fact tables, with dimensions related to facts but also related to other dimensions",
			"Transformation": "Step in both of the two major approaches to data processing, where data is converted into a form most appropriate for analytical processing and analysis",
			"Extract": "Step in both of the two major approaches to data processing, where ingested data is selectively pulled into the process for transformation and final storage",
			"Load": "Step in both of the two major approaches to data processing, whereby the data come to rest in a particular data resource for consumption by other processes or humans ",
			"Data Processing": "The act of gathering, cleansing, transforming, and storing data from multiple sources for use by other systems and processes or for further analysis and reporting"
		};
		gameH = {
			"Dataset": "A collection of data from one or more sources used to generate visualizations that can be aggregated into reports",
			"Dashboard": "A collection of visualizations in Power BI that are organized around a theme an allow for drill-down for further detail",
			"Visualization": "A data technique that translates information into a visual context to make it easier to understand and gain insights",
			"Microsoft Power BI Desktop": "A downloadable tool used to create interactive reports and visualizations",
			"Workspace": "A place to collaborate in building Power BI assets in the Power BI Service",
			"Tile": "A resizable component on a Power BI dashboard; each one displays a visualization that can be as complex as a bubble chart or as simple as a single value",
			"Power BI Report Builder": "A service evolved out of similar tooling for SQL Server Reporting Services and now used to build paginated reports in Power BI",
			"Pie Chart": "A simple, relative-measure chart that is useful only for a small number of categories",
			"Diagnostic": "Analytics technique that focuses on surfacing the reasons behind a particular event or scenario",
			"Prescriptive": "Analytics technique that offers recommendations by asserting required actions to achieve a target metric or goal",
			"Descriptive": "Analytics technique that presents historical and current data to help understand the state of a business or a system",
			"Predictive": "Analytics technique that projects future events based on past trends or similar scenarios",
			"Cognitive": "Analytics technique whose hallmark is the ability to make additional inferences based on analyzing more or more metrics",
			"Bar Chart": "Chart that allows for analysis of differences across a set of categories",
			"Line Chart": "Chart that allows for the measure of numeric data over two axes, with the x-axis often representing time",
			"Scatter Chart": "Chart that presents the relationship between two metrics using dots on on x and y axes",
			"Key Influencer": "Chart that surfaces the factors that affect a key metric",
			"Data Analyst": "Exploring and analyzing data and building business-friendly data models falls under the responsibilitys of this data professional.",
			"Analytics Workload": "Larger, richer data sets optimized for decision support and complex questions posed of the data.",
			"Microsoft Power BI Service": "Online platform focused on building, publishing, and sharing dashboards",
			"Microsoft Power BI Mobile": "Service designed for viewing shared Power BI dashboards and reports",
			"Bubble Chart": "Similar to a scatter chart but with a third dimension represented by the size of the dots",
			"Paginated Report": "Specialized Power BI report used to generate and share longer tabular data that can be formatted to fit well on a standard printed page",
			"Tree Map": "Visualization that uses interlocking rectangles, with color coding, size, and position to express relative value and some simple hierarchies",
			"Bingo Free Space 1": ""
		};

		
	function generate(game) {
		var usedTerms = [];
		
		var node = document.getElementById("grid");
		var nodeDef = document.getElementById("definitions");
		
/* 		if(node.innerHTML && !confirm("Are you sure you want to regenerate the game?"))
			return; */
		//randomly fill the bingo card/grid
		var html = '<h3>Buzzword Bingo Card</strong></h3><table border="0">';
		for(var y = 0; y < 5; y++) {
			html += "<tr>"
			for(var x = 0; x < 5; x++) {
				do {
					var i = Math.round(Math.random() * 24);
					var terms = Object.keys(game);
					var term = terms[i];
				} while(usedTerms.indexOf(term) >= 0);
				usedTerms.push(term);
				//show grid cell already selected if it is a free space
				if (term.includes("Bingo Free Space"))
				html += '<td id="key_' + term + '" Class="selectedOn">FREE SPACE!</td>';
				else
				html += '<td id="key_' + term + '" onclick="javascript:dabCard(\'key_' + term + '\',\'def_' + term + '\');">' + term + '</td>';

			}
			html += "</tr>"
		}
			html += "</table>";
			//load the grid in the randomized order
		node.innerHTML = html;

		//load the list of definitions in the original order from the dictionary object (so will be different from random loop that filled the bingo grid)
		var definitionsHTML = "</br><fieldset><legend>Definitions and Descriptions</legend></br>";
			//for each key (term) in the dictionary of terms
			for(var trm in game){
    			//Return the value (definition) for the current key
   				var definition = game[trm];
				//only create a definition entry if the dictionary entry is not a free space
				if (!trm.includes("Bingo Free Space"))
					{definitionsHTML += '<input type="radio" name="definitions" id="def_' + trm + '" value="key_' + trm + '"><label for="def_' + trm + '">'+ definition + '</label></br></br>';
					}
			}
			definitionsHTML += "</fieldset>";
			nodeDef.innerHTML = definitionsHTML;


		}

		function toggle(id){
		var elem = document.getElementById(id);
		if (elem.style.display == "block")
			elem.style.display = "none";
		else
			elem.style.display = "block";
		}	

		function dabCard(selectedKeyId,correctDefinitionId){
		var node = document.getElementById(selectedKeyId);
		var nodeDef = document.getElementById(correctDefinitionId);
		 if (nodeDef.checked)
			node.className="selectedOn";
		}
		
	</script>
</head>
<body>
<a><img src="AcgLogo.png" alt="acloudguru.com" width="200"></a></br>
<h1>Azure Data Fundamentals Bingo</h1>

<p>Built to support lessons presented in the DP-900 Azure Data Fundamentals exam prep course</p>

<a href="javascript:toggle('instructions');">Show/Hide Instructions...</a>

<noscript>
<div class="noJavascript">
<strong>Oops!</strong>
<p><em>
You do not have JavaScript enabled. Please enable JavaScript to use this application.
</em></p>
</div>
</noscript>

<div id="instructions">
<ol>
	<noscript><li>Enable JavaScript</li></noscript>
	<li>Click the appropriate lesson button, below, to generate your Bingo game; the position of each term on the Bingo card is randomly generated.</li>
	<li>Select a description or definition from the list. Go through the list in any order that suits you. Note: The definitions are meant as hints to jog your memory, not has full technical descriptions, with all caveats or scenarios required to fully describe the feature or service.
	<li>Find and select the correct match on the Bingo card. </li>
	<li>When you have filled an entire row, column, diagonal, the whole board, or when you simply have had enough and believe you know all there is to know, yell &quot;Bingo!&quot; Really, really loudly.</li>
	<li>No, the game will not tell you when you have Bingo. Yes, this is a low-tech game.</li>
	<li>Want more of a challenge? Try selecting correct matches on the Bingo card for as long as you can <strong>without</strong> achieving a row, column, or diagonal Bingo.</li>
	<li>Need more reinforcement? Click the same button to generate a new Bingo card with all the same words but in a different random configuraton.</li>
	<li>Your prize? Confirmation and reinforcement of the knowledge gained. You're welcome!</li>
</ol>
</div>
<form>
<input type="button" value="Azure Data Essentials" onClick="generate(gameA);"/>
<input type="button" value="Comparing Azure Data Offerings" onClick="generate(gameB);"/>
<input type="button" value="Azure Storage Options" onClick="generate(gameC);"/>
<input type="button" value="Azure Data Resource Management" onClick="generate(gameD);"/>
<input type="button" value="Azure Relational Data" onClick="generate(gameE);"/>
<input type="button" value="Azure Cosmos DB" onClick="generate(gameF);"/>
<input type="button" value="Azure Synapse Analytics - Plus" onClick="generate(gameG);"/>
<input type="button" value="Microsoft Power BI" onClick="generate(gameH);"/>
</form>
<div class="grid-container">

    <div id="definitions">
    </div>
  
    <div id="grid">
    </div>

</div>

</body>
</html>
