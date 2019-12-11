# SchemaSpy
<strong>SchemaSpy to document database</strong>

Here you can learn, how to generate the database documentation from a simple MySQL schema
<h2>SchemmaSpy (Official description)</h2>
SchemaSpy is a Java-based tool (requires Java 5 or higher) that analyzes the metadata of a schema in a database and generates a visual representation of it in a browser-displayable format
<h2>Prerequisites</h2>
<li>Java 5 or higher installed</li>
<li>Access to a MySQL server installation</li>
<li>Graphviz installed → http://www.graphviz.org/</li>
<h2>Configuration and Execution</h2>
<ol><li>
Download SchemaSpy jar file (schemaSpy_5.0.0.jar)
</li></ol>
<ol start="2"><li>
Download the MySQL Java Connector jar file <strong>(mysql-connector-java-5.1.22.jar)</strong>
</li></ol>
<ol start="3"><li>
Execute the next command updating the parameter values based on your MySQL installation, MySQL credentials and the files downloaded previously (SchemaSpy and Java Connector)
</li></ol>

<h2>How to Execute</h2>

<br/>
<strong>Using Command</strong>

<li>java -jar C:\Users\XXXXX\Desktop\SchemaSpy\schemaSpy-6.1.0.jar -vizjs -t mysql -host <strong>HOSTNAME</strong> -db <strong>DATABASE</strong> -s <strong>SCHEMA</strong> -u <strong>USER</strong> -p <strong>PASSWORD</strong> -dp C:\Users\XXXXX\Desktop\mysql-connector-java-5.1.22.jar -o C:\Users\XXXXX\Desktop\SchemaSpy\DB_Documentation -gv C:\Program Files (x86)\Graphviz2.38</li>

<br/>
<strong>Using Property File</strong>

<li>java -jar C:\Users\XXXXX\Desktop\SchemaSpy\schemaSpy-6.1.0.jar -vizjs -configFile C:\Users\XXXXX\Desktop\SchemaSpy/schemaspy.properties</li>

<br/>
<strong>Property File</strong>
<li>schemaspy.t=mysql</li>
<li>schemaspy.dp=C:\Users\XXXXX\Downloads\mysql-connector-java-5.1.22.jar</li>
<li>schemaspy.host=localhost</li>
<li>schemaspy.port=3306</li>
<li>schemaspy.db=DATABASE</li>
<li>schemaspy.u=USER</li>
<li>schemaspy.p=PASSWORD</li>
<li>schemaspy.o=C:\Users\XXXXX\Desktop\SchemaSpy\DB_Documentation</li>
<li>schemaspy.s=SCHEMA</li>

<h1>Open the index.html file in order to refer the generated database documentation</h1>
