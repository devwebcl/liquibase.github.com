---
layout: default
title: Change dropView
---

<!-- ====================================================== -->
<!-- GENERATED BY ChangeDocGenerator DO NOT MODIFY MANUALLY -->
<!-- ====================================================== -->

# Change: 'dropView'

Drops an existing view

## Available Attributes ##

<table>
<tr><th>Name</th><th>Description</th><th>Required&nbsp;For</th><th>Since</th></tr>
<tr><td style='vertical-align: top'>catalogName</td><td>Name of the catalog</td><td style='vertical-align: top'></td><td style='vertical-align: top'>3.0</td></tr>
<tr><td style='vertical-align: top'>schemaName</td><td>Name of the schema</td><td style='vertical-align: top'></td><td style='vertical-align: top'></td></tr>
<tr><td style='vertical-align: top'>viewName</td><td>Name of the view to drop</td><td style='vertical-align: top'>all</td><td style='vertical-align: top'></td></tr>
</table>

## XML Sample ##

{% highlight xml %}
<changeSet author="liquibase-docs" id="dropView-example">
    <dropView catalogName="cat"
            schemaName="public"
            viewName="A String"/>
</changeSet>
{% endhighlight %}

## YAML Sample ##

{% highlight yaml %}
changeSet:
  id: dropView-example
  author: liquibase-docs
  changes:
  - dropView:
      catalogName: cat
      schemaName: public
      viewName: A String

{% endhighlight %}

## JSON Sample ##

{% highlight json %}
{
  "changeSet": {
    "id": "dropView-example",
    "author": "liquibase-docs",
    "changes": [
      {
        "dropView": {
          "catalogName": "cat",
          "schemaName": "public",
          "viewName": "A String"
        }
      }]
    
  }
}

{% endhighlight %}

## SQL Generated From Above Sample (MySQL)

{% highlight sql %}
DROP VIEW cat.A String;


{% endhighlight %}

## Database Support

<table style='border:1;'>
<tr><th>Database</th><th>Notes</th><th>Easy Rollback</th></tr>
<tr><td>Cache</td><td><b>Supported</b></td><td>No</td></tr>
<tr><td>DB2</td><td><b>Supported</b></td><td>No</td></tr>
<tr><td>DB2i</td><td><b>Supported</b></td><td>No</td></tr>
<tr><td>Derby</td><td><b>Supported</b></td><td>No</td></tr>
<tr><td>Firebird</td><td><b>Supported</b></td><td>No</td></tr>
<tr><td>H2</td><td><b>Supported</b></td><td>No</td></tr>
<tr><td>HyperSQL</td><td><b>Supported</b></td><td>No</td></tr>
<tr><td>Informix</td><td><b>Supported</b></td><td>No</td></tr>
<tr><td>MySQL</td><td><b>Supported</b></td><td>No</td></tr>
<tr><td>Oracle</td><td><b>Supported</b></td><td>No</td></tr>
<tr><td>PostgreSQL</td><td><b>Supported</b></td><td>No</td></tr>
<tr><td>SAP DB</td><td><b>Supported</b></td><td>No</td></tr>
<tr><td>SQL Server</td><td><b>Supported</b></td><td>No</td></tr>
<tr><td>SQLite</td><td><b>Supported</b></td><td>No</td></tr>
<tr><td>Sybase</td><td><b>Supported</b></td><td>No</td></tr>
<tr><td>Sybase Anywhere</td><td><b>Supported</b></td><td>No</td></tr>
</table>