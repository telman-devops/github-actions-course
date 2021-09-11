# github-actions-course


---
### Dispatch event [Udemy lesson](https://www.udemy.com/course/github-actions/learn/lecture/17389694#overview)
```
https://api.github.com/repos/{owner}/{repo}/dispatches
```
### Example [Github](https://docs.github.com/en/rest/reference/repos#create-a-repository-dispatch-event)
```
https://api.github.com/repos/telman-devops/github-actions-course/dispatches
```
> Params with POST request
```
{
    "event_type":"build",
    "client_payload": {
        "env": "production"
    }
}
```