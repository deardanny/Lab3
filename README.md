# Lab3

A Java servlet application that lets a visitor enter a keyword and request a picture. The repository ships the compiled application in `ROOT.war`.

## Run locally

From the repository root, run:

```sh
docker build -t lab3 .
docker run --rm -p 127.0.0.1:8080:8080 lab3
```

Open <http://localhost:8080/>. Tomcat serves `ROOT.war` at the root URL. The welcome route is `getAnInterestingPicture`, and the form sends the keyword in the `searchWord` query parameter.
