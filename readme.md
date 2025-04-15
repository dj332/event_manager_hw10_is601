# Event Manager

## To run application
```sh
docker compose up --build
```

Go to api endpoints by [http://localhost/docs](http://localhost/docs)


Go to database by [http://localhost:5050](http://localhost:5050)

postgres access:
- username: admin@example.com
- password: adminpassword


## Issues
### Issue 1
**Issue Title:** Data mismatch in endpoint and Postgres table during register

**Fix:** The given nickname at register endpoint is not stored in the database. Changed the functionality to store it in the database. If it already exists, it will generate a random nickname. This can be changed in the future, but currently it is a good solution.

**Link:**
Issue Link: [Issue 1](https://github.com/dj332/event_manager_hw10_is601/issues/1)

### Issue 2
**Issue Despcription:** User validation not implemented

**Fix:** Added user validation.

**Link:**
Issue Link: [Issue 2](https://github.com/dj332/event_manager_hw10_is601/issues/2)

### Issue 3
**Issue Despcription:** Password validation is missing

**Fix:** Added password validation.

**Link:**
Issue Link: [Issue 3](https://github.com/dj332/event_manager_hw10_is601/issues/3)

### Issue 4
**Issue Despcription:** Profile and bio field tests absent

**Fix:** Profile and bio field edge-cases tests added.

**Link:**
Issue Link: [Issue 4](https://github.com/dj332/event_manager_hw10_is601/issues/4)

### Issue 5
**Issue Despcription:** User API test fails

**Fix:** Fixed user api tests.

**Link:**
Issue Link: [Issue 5](https://github.com/dj332/event_manager_hw10_is601/issues/5)

### Issue 6
**Issue Despcription:** test_user_schemas.py tests fail

**Fix:** Something here

**Link:**
Issue Link: [Issue 6](https://github.com/dj332/event_manager_hw10_is601/issues/6)

## Dockerhub
Dockerhub Link for this project: [Dockerhub Link](https://hub.docker.com/repository/docker/dhjariwala/hw10/general)
>To access this link you have to login to your dockerhub account.

## Learning from this assignment
### Chanllenges faced
1. While merging to the repository, I accidently pushed it to the main application of professor and not the forked repository.
2. Sometimes I know what the error is, but since there is no traceback of said errors, I had to guess where the error is being generated from.
3. The code has minimal documentation and comments makes it difficult to understand the code.
4. I forked the repository on a different account then what I have locally. This made it difficult to push the changes.

### Solutions implemented
1. Implemented the functionality to store the nickname in the database. If it already exists, it will generate a random nickname. This can be changed in the future, but currently it is a good solution.
2. Many tests were failing, sometime not because the function itself is wrong, but because of the way the tests are written. I had to write more code in [conftest.py](tests/conftest.py) to make the tests pass.
3. I solved the issue of different accounts on github by giving both accounts access to the repository.

### Insights gained
1. Learned how to use api endpoints to find errors in the application.
2. Learned how collaborating with others on github would look like.
3. Learned how to use github issues to track bugs and issues.
4. Expereinced small things that might go wrong while using github. For example, I had to give both accounts access to the repository, which needs to be avoided.

## Grading Rubric

| Criteria                                                                                                                | Points |
|-------------------------------------------------------------------------------------------------------------------------|--------|
| ✅ Resolved 5 issues related to username validation, password validation, and profile field edge cases                      | 30     |
| ✅ Resolved the issue demonstrated in the instructor video                                                                 | 20     |
| ✅ Increased test coverage to 90% by writing comprehensive test cases                                                      | 20     |
| ✅ Followed collaborative development practices using Git and GitHub (branching, pull requests, code reviews)              | 15     |
| ✅ Submitted a well-organized GitHub repository with clear documentation, links to closed issues, and a reflective summary | 15     |
| **Total**                                                                                                               | **100**|