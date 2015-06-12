# Integration tests

* [Integration Testing](https://msdn.microsoft.com/en-us/library/aa292128(v=vs.71).aspx) page in MSDN
* [Integration Testing Principles](http://blogs.msdn.com/b/ploeh/archive/2006/11/15/integrationtestingprinciples.aspx) by Mark Seemann

## Databases in integration tests

*   [Do Not Depend on Your Data Being There][another-it-msdn]

    _Tests that depend on specific data should always create that data before they execute. If you assume that the data is there, the test becomes brittle. Undoubtedly, another developer or database administrator will delete or modify the test data and break the test._

## Dictionary

* brittle - хрупкий

[another-it-msdn]: https://msdn.microsoft.com/en-us/library/vstudio/hh323698(v=vs.100).aspx
