Prior to Lucee 6, an empty value would be auto cast to null, since Lucee 6 only strings are handled this way [LDEV-4410](https://luceeserver.atlassian.net/browse/LDEV-4410)

In Lucee 6, this is no longer the default behavior and throws an exception, which matches ACF.

You can re-enable the old behavior by setting this environment variable or system property to `true`.

**Environment Variable:** `LUCEE_QUERY_ALLOWEMPTYASNULL=TRUE`  
**System Property:** `-Dlucee.query.allowemptyasnull="true"`
