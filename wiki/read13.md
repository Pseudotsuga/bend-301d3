# Update/Delete

The \<form> html element defines how data is sent from the client-side of an application to the server side. There are two main attributes of the \<form> element that enable this definition.

1. The action attribute defines the location where the data from the form will be sent. 
    - This attribute will accept absolute or relative paths.
    - The value of this attribute **must** be a valid url.
    - By default the data will be sent to the same page as the form if no alternative path is defined.

2. The method attribute defines the method (appropriately) by which the data will be sent. These methods correlate with the methods defined in the HyperText Transfer Protocol (HTTP).
    - The two most common methods for form submission are GET and POST.

    - In the event of a GET method:
      + GET requests are the browser asking the server for a resource at that location.  
      + The request data body will be empty, so key/value pairs from the form are simply appended on to the end of the URL. 
      + At the end of the general url you will see a **?** followed by key/value pairs separated by **&**.

    - In the event of a POST method:
      + The POST method is used when one desires the server to process something in the request and respond with the post-processed information.
      + No information is appended to the url, instead the information/data lives in the request body.

## References:
[HTML Forms](https://developer.mozilla.org/en-US/docs/Learn/HTML/Forms/Sending_and_retrieving_form_data)

[HTTP General Info](https://developer.mozilla.org/en-US/docs/Web/HTTP)