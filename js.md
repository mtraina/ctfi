**AJAX**  
AJAX, asynchronous javascript and XML, isa way to communicate with the server without reloading the page. Typically the browser makes a request to the server using XMLHttpRequest, when the data is received from the browser, it will perform the operation in the function *onreadystatechange*.

```javascript
httpRequest = new XMLHttpRequest();
httpRequest.onreadystatechange = handleResponse;
httpRequest.open('GET', 'http://www.foo.com');
httpRequest.send();

function handleResponse(){
  if(httpRequest.readyState === XMLHttpRequest.DONE){
    alert('the response status is: ' + httpRequest.status);
  }
}
```
