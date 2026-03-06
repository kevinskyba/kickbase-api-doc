<p align="center">
    <img src="https://upload.wikimedia.org/wikipedia/commons/a/a4/Kickbase_Logo_2023.svg"
    width="100">
</p>

<h1 align="center">
Kickbase API v4 Documentation
</h1>

<div align="center">

<a href="https://share.apidog.com/bca1f84a-99d7-4f8f-96a5-5e084ee24fe3">

![Static Badge](https://img.shields.io/badge/Browse%20Docs%20with%20apidog%20ui-585858?style=for-the-badge&logo=apidog)

</a>

</div>

<div align="center">

<a href="http://kevinskyba.github.io/kickbase-api-doc/index.html">

![Static Badge](https://img.shields.io/badge/Browse%20Docs%20with%20swagger%20ui-585858?style=for-the-badge&logo=swagger)

</a>

![Static Badge](https://img.shields.io/badge/version-4.5.0-%23ff4600?style=for-the-badge)
![Static Badge](https://img.shields.io/badge/license-MIT-%23ff4600?style=for-the-badge)
![Static Badge](https://img.shields.io/badge/contributers-3-%23ff4600?style=for-the-badge)

</div>

This repository contains the **API v4** documentation of the popular game **[kickbase](https://www.kickbase.com/)**.
This work is unofficial and not related to kickbase in any way. All of this was done for scientific reasons only and you
should not use it for anything else but for your personal learning!

## Usage

### Web

> **NEW!** Directly use the browseable and
> interactive [Apidog Web Version](https://share.apidog.com/fe2420a6-d929-409f-9b1d-35122923316d)

Use the browseable [Web Version](http://kevinskyba.github.io/kickbase-api-doc/index.html) made
with [Apidog](https://apidog.com/blog/export-postman-documentation-to-html-or-markdown/)
and [Swagger Hub](https://app.swaggerhub.com/)

**How to get started:**

1. Choose endpoint `/v4/user/login` from the `User` section
2. On the right hand side click the `"Try it out"` button

3. Fill in your kickbase email and password into the request body json

   ```json
   {
     "em": "your-kickbase-email",
     "loy": false,
     "pass": "your-kickbase-password",
     "rep": {}
   }
   ```

4. Click the `"Execute"` button and copy the property `"tkn"` from the response body json

   ```json
   {
       ...
       "tkn": "my-secret-access-token",
       ...
   }
   ```

5. Click `"Authorize"` at the top right corner of the page, paste in the `access token` into the value field and click
   again `"Authorize"`

6. Now you can try out any endpoint with your path and query params

### Local

#### Postman

Import the [Postman Collection JSON](kickbase-v4.postman_collection.json)
and [Postman Eniroment JSON](kickbase-v4.postman_environment.json) into your postman workspace

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

### API Documentation Status

This documentation contains all currently known endpoints, including their path parameters, query parameters, and
request bodies, as of March 6, 2026.

For GET requests, we provide response examples for most endpoints. However, for the majority of POST, PUT, and DELETE
requests, response examples are currently missing. Collecting and validating these responses requires significant setup
and time, and this project is maintained as a hobby project.

Descriptions have been added to most relevant endpoints. These descriptions were generated using Postman Generative AI.
While they appear largely accurate at first glance, they may still contain inaccuracies or hallucinations, so please
verify them before relying on them in production environments.

Please use the API responsibly. Avoid sending large numbers of requests or requesting excessive amounts of data at once.
It is possible that the service provider may monitor requests made outside their official applications and block access.
We do not take responsibility for any actions taken using this documentation.

If you encounter incorrect documentation or non-working endpoints, please open an issue.

### Contributing

We are always looking for contributors.

At the moment, the most valuable contributions would be:

- Collecting 2xx and 4xx responses
- Documenting response schemas
- Completing request body schemas

Having complete request and response schemas would allow us to generate an OpenAPI specification. This would enable
automatic generation of REST clients, for example:

- JavaScript clients using tools like Orval
- Python clients using frameworks such as FastAPI

These improvements would significantly increase the usability of this project.

Thank you!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
