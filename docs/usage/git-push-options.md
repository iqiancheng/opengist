# Push Options

Opengist has support for a few [Git push options](https://git-scm.com/docs/git-push#Documentation/git-push.txt--oltoptiongt). 

These options are passed to `git push` command and can be used to change the metadata of a gist.

## Set URL

```shell
git push -o url=mygist # Will set the URL to https://opengist.example.com/user/mygist
```

## Change title

```shell
git push -o title=Gist123
git push -o title="My Gist 123"
```

## Change description

```shell
git push -o description="This is my gist description"
# For descriptions with special characters, you can use URL encoding
git push -o description="Hello%20World%21"
```

Note: If your description contains spaces or special characters, you can either:
- Wrap it in quotes: `git push -o description="Hello World!"`
- Use URL encoding: `git push -o description=Hello%20World%21`

## Change visibility

```shell
git push -o visibility=public
git push -o visibility=unlisted
git push -o visibility=private
```
