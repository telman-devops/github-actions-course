# github-actions-course


---
### Branch dispatch-event [Udemy lesson](https://www.udemy.com/course/github-actions/learn/lecture/17389694#overview)
```
https://api.github.com/repos/{owner}/{repo}/dispatches
```
#### Example [Github](https://docs.github.com/en/rest/reference/repos#create-a-repository-dispatch-event)
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

---
### Branch filtering-workflows-by-branches-tags-and-paths [Udemy lesson](https://www.udemy.com/course/github-actions/learn/lecture/17392734#overview)

```
on:
  push:
    branches:
      - master
      - "feature/**" # matches featur/featA, feature/featB, doesn't match feature/feat/a
      - "!feature/featc"
    tags: 
      - v1.*
    paths: 
      - "**.js"
      - "!filename.js"
    # paths-ignore:
    # - 'docs/**'
```

#### Example [Github](https://docs.github.com/en/rest/reference/repos#create-a-repository-dispatch-event)