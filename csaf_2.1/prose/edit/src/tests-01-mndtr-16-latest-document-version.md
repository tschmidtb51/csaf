### Latest Document Version

It MUST be tested that document version has the same value as the `number` in the last item of the revision history when
it is sorted ascending by `date` and as a second level criteria `number`.
As the timestamps might use different timezones, the sorting MUST take timezones into account.
Build metadata is ignored in the comparison.
Any pre-release part is also ignored if the document status is `draft`.

The relevant path for this test is:

```
    /document/tracking/version
```

*Example 1 (which fails the test):*

```
  "tracking": {
    // ...
    "revision_history": [
      {
        "date": "2024-01-21T09:00:00.000Z",
        "number": "1",
        "summary": "Initial version."
      },
      {
        "date": "2024-01-21T10:00:00.000Z",
        "number": "2",
        "summary": "Second version."
      }
    ],
    // ...
    "version": "1"
  }
```

> The value of `number` of the last item after sorting is `2`. However, the document version is `1`.
