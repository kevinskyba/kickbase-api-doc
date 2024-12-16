<p align="center">
    <img src="https://upload.wikimedia.org/wikipedia/commons/a/a4/Kickbase_Logo_2023.svg"
    width="100">
</p>

<h1 align="center">
Kickbase API v4 Documentation
</h1>

<div align="center">

<a href="http://kevinskyba.github.io/kickbase-api-doc/index.html">

![Static Badge](https://img.shields.io/badge/Browse%20Docs%20with%20swagger%20ui-585858?style=for-the-badge&logo=swagger)

</a>

![Static Badge](https://img.shields.io/badge/version-4.0.17-%23ff4600?style=for-the-badge)
![Static Badge](https://img.shields.io/badge/license-MIT-%23ff4600?style=for-the-badge)
![Static Badge](https://img.shields.io/badge/contributers-3-%23ff4600?style=for-the-badge)

</div>

This repository contains the **API v4** documentation of the popular game **[kickbase](https://www.kickbase.com/)**. This work is unofficial and not related to kickbase in any way. All of this was done for scientific reasons only and you should not use it for anything else but for your personal learning!

## Usage

### Web

Use the browseable [Web Version](http://kevinskyba.github.io/kickbase-api-doc/index.html) made with [Apidog](https://apidog.com/blog/export-postman-documentation-to-html-or-markdown/) and [Swagger Hub](https://app.swaggerhub.com/)

**How to get started:**

1. Make sure `"https://api.kickbase.com - Kickbase v4"` is selected in the `"Servers"` dropdown

2. Choose endpoint `/v4/user/login` from the `User` section

3. On the right hand side click the `"Try it out"` button

4. Fill in your kickbase email and password into the request body json

   ```json
   {
     "em": "your-kickbase-email",
     "loy": false,
     "pass": "your-kickbase-password",
     "rep": {}
   }
   ```

5. Click the `"Execute"` button and copy the property `"tkn"` from the response body json

   ```json
   {
       ...
       "tkn": "my-secret-access-token",
       ...
   }
   ```

6. Click `"Authorize"` at the top right corner of the page, paste in the `access token` into the value field and click again `"Authorize"`

7. Now you can try out any endpoint with your path and query params

### Local

#### Postman

Import the [Postman Collection JSON](kickbase-v4.postman_collection.json) and [Postman Eniroment JSON](kickbase-v4.postman_environment.json) into your postman workspace

#### Swagger

Import the [Swagger JSON](kickbase-v4.swagger.json) into your swagger hub

## Contributors

<table>
  <tbody>
    <tr>
        <td align="center" style="border: 1px solid white"><a href="https://github.com/kevinskyba"><img src="https://avatars.githubusercontent.com/u/1737255?v=4" width="100px;" style="border-radius: 10px; object-fit: contain;border: 2px solid #ff4600" alt="kevinskyba"/><br /><sub><b>kevinskyba</b></sub></a></td>
        <td align="center" style="border: 1px solid white"><a href="https://github.com/simonsagstetter"><img src="https://avatars.githubusercontent.com/u/44363600?v=4" width="100px;" style="border-radius: 10px; object-fit: contain;border: 2px solid #ff4600" alt="simonsagstetter"/><br /><sub><b>simonsagstetter</b></sub></a></td>
        <td align="center" style="border: 1px solid white"><a href="https://github.com/casudo"><img src="https://avatars.githubusercontent.com/u/55252063?v=4" width="100px;" style="border-radius: 10px; object-fit: contain;border: 2px solid #ff4600" alt="casudo"/><br /><sub><b>casudo</b></sub></a></td>
    </tr>
  </tbody>
</table>

## Issues

As all of the endpoints are **found by try and error**, this documentation **may be incomplete**. Most likely there are more endpoints. **In fact, most of the post, put or delete requests have missing request bodies**. If you have any further information about new or existing endpoints feel free to submit them in the issues. We'll review and add them to the documentation.

Thank you!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
