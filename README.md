Python requests with decorator, complete + authentication

Based on chepner's answer to:

https://stackoverflow.com/questions/60308891/python-requests-with-decorator

The code now has all types of requests covered, plus the possibility of having authentication on each request.

Pros:
1. Easy to read, less code, therefore easier to maintain.
2. Easy to add new methods or to update the existing ones.

Cons:
1. Can't get it to work on pytest.
2. A less "standard" API might cause hard to debug errors.
3. A less "standard" API might need changes to the wrapper that can be tricky.
4. Big performance loss because of all the nested function calls (methods/decorators are functions)
