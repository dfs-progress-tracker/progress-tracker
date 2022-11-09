# Contributors
```
Zishan Kazi (pixel-z)
```

## Issue Resolved
- Change backend to include token timeout and send to frontend
- [Issue #6](https://github.com/AmitPandey-Research/dfs-frontend/issues/6)

## Files changed (Pull Request)
- [Frontend PR #33](https://github.com/AmitPandey-Research/dfs-frontend/pull/33)
- [Backend PR #22](https://github.com/AmitPandey-Research/dfs-backend/pull/22)
- [Backend PR #25](https://github.com/AmitPandey-Research/dfs-backend/pull/25)

## Requirements

Worked on the files:
- `tokens.js`
- `src/request.js`
- `src/components/homepage/myDatasets.js`
- `src/components/homepage/myModels.js`
- `src/components/homepage/myPermissionRequests.js`
- `src/components/homepage/myRequests.js`
- `src/components/datasets/allDatasets.js`
- `src/components/datasets/allVersions.js`
- `src/components/datasets/viewDatasetModal.js`
- `src/containers/datasetadd/addDataset.js`
- `src/containers/datasets/domains.js`
- `src/containers/homepage/homepage.js`
- `src/containers/review/reviewPage.js`
- `src/containers/tnc-edit/TncEdit.jsx`
- `src/containers/upload/uploadPage.js`
- `src/containers/upload/uploaderPage.js`
- `src/containers/verify/verify.js`

On login, store the timestamp along with the token. Add a `isTokenStillValid` function that checks if it has been more than x hrs since the token was generated. Read x from `creds.js` now, add this function before very request

Make a request module that exports a custom version of axios with heads to all hooks / components making requests. E.g: a module that exports

## Design Step
- Tech stack being used: `ReactJS`
- Changed `/login` route, bug fixes in validTill.
- Changing all the axios requests and replacing through a wrapper function of `getWithLogin()` and `postWithLogin()`.
- The wrapper functions check whether the token is valid or not, if not, it redirects to login page. 
- Changed all the files where the user data is is being accessed using localStorage.