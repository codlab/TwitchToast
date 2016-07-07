# geekincwidget-simple

## Installation and requirements
```
git clone
npm install
```

## Server usage
```
npm start
```

## Local usage

Two web pages are provided to be used as :

- administration
- viewer, the page must be used in your OBS/XSplit clients


By default, the two urls are:

- the administration :  [localhost:8081/adminBeta.html](http://localhost:8081/adminBeta.html)
- the viewer :  [localhost:8081/xsplit.html](http://localhost:8081/xsplit.html)

## Components

The two pages communicate with each other through the server using websocket. The server is using a local storage to store the raw json of the admin/viewer pages

## Security

As for now, the two pages lacks of SSO. It is in the pipeline to add strong authentication to manage sessions for admin and direct link for the xsplit page

Moreover, currently, the json is saved and retrieved AS IS. In this way html can be injected in some part of the page. Some modification should be integrated to prevent such things.

## Licence

This project is licensed under the MIT license.
