# Contributors
```
Zishan Kazi (pixel-z)
```

## Issue Resolved
- Change backend to include token timeout and send to frontend
- https://github.com/AmitPandey-Research/dfs-frontend/issues/6

## Files changed (Pull Request)
- https://github.com/AmitPandey-Research/dfs-backend/pull/22

## Requirements Step

Working on the files:
- `src/request.js`
- `src/components/datasets/viewDatasetModal.js`
- `src/components/homepage/myRequests.js`
- `src/containers/verify/verify.js`

On login, store the timestamp along with the token. Add a `isTokenStillValid` function that checks if it has been more than x hrs since the token was generated. Read x from `creds.js` now, add this function before very request

Make a request module that exports a custom version of axios with heads to all hooks / components making requests. E.g: a module that exports

## Design Step
- Tech stack being used: `Javascript, SQL`
- Changing the schema and adding DfsUser table into the database and adding the sample values into it.
- Creating the relevant dump file (dump_v2.sql) for other users to add other the new table sample values

## Build Step

## Testing Step

