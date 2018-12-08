---
layout: post
title: JDBC Notes
categories: [it]
tags: [it, java, jdbc]
date: 2018-12-08
---

<div class="thi-step">
<div class="step">
<div class="step-number"></div>
<div class="step-content" markdown="1">
To load a spicific database driver and get a connection between java code and data source (here is a database).
{% highlight ruby %}
Class.forName("com.mysql.jdbc.Driver");
Connection conn = DriverManager.getConnection("jdbc:mysql://localhost/countries?" + "user=root&password=root");
{% endhighlight %}
</div>
</div>

<div class="step">
<div class="step-number"></div>
<div class="step-content" markdown="1">
Getted a connection
{% highlight ruby %}
Statement stmt = conn.createStatement();
{% endhighlight ruby %}
</div>
</div>
</div>

<div class="step">
<div class="step-number"></div>
<div class="step-content" markdown="1">
Execute a sql statement.
{% highlight ruby %}
String sql = "SELECT * FROM TABLE-NAME";
ResultSet rs = stmt.executeQuery(sql);
{% endhighlight ruby %}
</div>
</div>
</div>

<div class="step">
<div class="step-number"></div>
<div class="step-content" markdown="1">
Deal with the return result 
{% highlight ruby %}
while (rs.next()) {
  rs.getInt();
  rs.getString();
  rs.getDate();
}
{% endhighlight ruby %}
</div>
</div>
</div>

<div class="step">
<div class="step-number"></div>
<div class="step-content" markdown="1">
Close the statement session and the connection.
{% highlight ruby %}
stmt.close();
conn.close();
{% endhighlight ruby %}
{% include warning.html content="Must remember to close the connection" %}
</div>
</div>
</div>
