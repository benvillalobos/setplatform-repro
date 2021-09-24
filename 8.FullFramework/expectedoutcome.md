When building .sln files, this will likely fail with outputpath issues.
this is because of the AssignConfiguration target which forces platform and outputpath to be removed, which
apparently has precedence over undefining a property.

When building a csproj, just pass a platform that A can build as, and B will follow suit.