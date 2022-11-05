## Requirements Step

[Issue 10](https://github.com/AmitPandey-Research/dfs-backend/issues/10)

Contributors : Shaantanu Kulkarni

Working on the files:
- Complete backend database

The backend code was scattered and had the following issues:
- Inconsistent naming of variables
- Too much cluttered code in one file
- Inadequate segregation of the files in a given directory

The following image shows the directory structure before refactoring

[](https://imgur.com/hA1j7AJ.png)

[](https://imgur.com/gl1trUJ.png)

As you can see that the file names are not intuitive and there is no proper documentation for the above.

### Requirements
- Segregating the files into particular directories
- Clean up the code so that there are no more than 2-3 requests per file
- Extracting repetitive code into functions and adding then into `utils.js` of each directory.

## Design Step
- Tech stack being used: `Javascript`
- Understanding the code so that segregating the files is easy.
- Identifying the endpoints and grouping requests based on **GET** and **POST** requests on particular tables in SQL database.
- Documentation for each of the directory with functionality of each function and endpoints.

## Implementation

Updated directory structure
![](https://imgur.com/1PLxpZY.png)
![](https://imgur.com/xduCurP.png)

Documentation for /routes/auth directory
![](https://imgur.com/fwwsGCa.png)