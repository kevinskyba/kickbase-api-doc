# Kickbase API Doc

This repository contains the documentation of the API of the popular game [kickbase](https://www.kickbase.com/). This work is unofficial and not related to kickbase in any way. All of this was done for scientific reasons only and you should not use it for anything else but for your personal learning!

You may see the documentation [HERE](http://kevinskyba.github.io/kickbase-api-doc/index.html).

## Generate

This API is based on a postman collection. This collection is transformed to HTML using [postmanerator](https://github.com/aubm/postmanerator/).
In order to generate the API you use the following command:

```
postmanerator -collection=Kickbase.postman_collection.json -output=./docs/index.html -environment=Kickbase.postman_environment.json
```

## License

[MIT License](LICENSE.md)