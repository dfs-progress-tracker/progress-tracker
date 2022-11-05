# Contributors
```
Zishan Kazi (pixel-z)
```

## Issue Resolved
- [Issue #3](https://github.com/AmitPandey-Research/dfs-backend/issues/3)
- [Issue #8](https://github.com/AmitPandey-Research/dfs-backend/issues/8)
## Files changed (Pull Request)
- [PR #7](https://github.com/AmitPandey-Research/dfs-backend/pull/7)

## Requirements Step

Working on the files:
- `token.js`
- `create_schema.sql`
- `dump_v2.sql`

Users and tokens are being loaded using the hardcoded code stored in users.json and tokens.json. Changing from loading from these json files to loading from tables (by executing sql query).

## Design Step
- Tech stack being used: `Javascript, SQL`
- Changing the schema and adding DfsUser table into the database and adding the sample values into it.
- Creating the relevant dump file (dump_v2.sql) for other users to add other the new table sample values

## Build Step
- Changing the code of loading data from user.json and tokens.json to loading it by running SQL queries (using execSql function)

- Files changed: [token.js](https://github.com/AmitPandey-Research/dfs-backend/blob/master/routes/auth/token.js)

- All changes: [PR #7](https://github.com/AmitPandey-Research/dfs-backend/pull/7)

## Testing Step
- Tested code for all possible conditions for login and signup.

![](https://imgur.com/xrvxglT.png)

![](https://imgur.com/ZNAfQzy.png)

![](https://imgur.com/eM7WVog.png)

![](https://imgur.com/RGq9y6v.png)