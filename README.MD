# bk's tryout: Create Github Action

followed: 
https://docs.github.com/en/actions/creating-actions/creating-a-javascript-action

```bash

git commit -m "My first action is ready"
git tag -a -m "My first action release" v1.1
git push --follow-tags
```

### instead of checking in node_modules


https://github.com/vercel/ncc

```bash
npm i -g @vercel/ncc
ncc build index.js --license licenses.txt
```





Template from tutorial: 
# Hello world javascript action

This action prints "Hello World" or "Hello" + the name of a person to greet to the log.

## Inputs

### `who-to-greet`

**Required** The name of the person to greet. Default `"World"`.

## Outputs

### `time`

The time we greeted you.

## Example usage

```yaml
uses: actions/hello-world-javascript-action@e76147da8e5c81eaf017dede5645551d4b94427b
with:
  who-to-greet: 'Mona the Octocat'
```
