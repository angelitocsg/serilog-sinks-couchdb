### Serilog.Sinks.CouchDB

A Serilog sink that writes events to Apache [CouchDB](http://couchdb.org).

**Package** - [Serilog.Sinks.CouchDB.DotNetCore](#)
| **Platforms** - .NET Core 3.1

You'll need to create a database on your CouchDB server. In the example shown, it is called `log`.

```csharp
var log = new LoggerConfiguration()
    .WriteTo.CouchDB("http://mycouchdb/log/")
    .CreateLogger();
```
