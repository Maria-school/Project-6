## Описание эндпоинтов Swagger тестового API
***
## 1. GET/api​/v1​/Activities

1. HTTP-метод- GET
2. Полный URL запроса- https://fakerestapi.azurewebsites.net/api/v1/Activities
3. Заголовки запроса- "accept: text/plain; v=1.0"
4. Тело запроса -отсутствует
5. Статус-код ответа-200
6. Тело ответа 
```
  {
    "id": 1,
    "title": "Activity 1",
    "dueDate": "2023-06-14T05:42:26.0721103+00:00",
    "completed": false
  }
  ```
***
## 2. POST​/api​/v1​/Activities
1. HTTP-метод-POST
2. Полный URL запроса-https://fakerestapi.azurewebsites.net/api/v1/Activities
3. Заголовки запроса-"accept: text/plain; v=1.0" , "Content-Type: application/json; v=1.0"
4. Тело запроса 
```
{
  "id": 0,
  "title": "string",
  "dueDate": "2023-06-14T05:14:46.534Z",
  "completed": true
}
```
5. Статус-код ответа-200
6. Тело ответа 
```
{
  "id": 0,
  "title": "string",
  "dueDate": "2023-06-14T05:14:46.534Z",
  "completed": true
}
```

***
## 3. POST​/api​/v1​/Activities
1. HTTP-метод -POST
2. Полный URL запроса-https://fakerestapi.azurewebsites.net/api/v1/Activities
3. Заголовки запроса-"accept: text/plain; v=1.0" , "Content-Type: application/json; v=1.0" 
4. Тело запроса 
```
{
  "id": 7777888888888,
  "title": "string",
  "dueDate": "2023-06-14T05:14:46.534Z",
  "completed": true
}
```
5. Статус-код ответа-400
6. Тело ответа 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-0cb41bcdf7f070408cb668d973a34828-fb06fec53ad8ad41-00",
  "errors": {
    "$.id": [
      "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 0 | BytePositionInLine: 19."
    ]
  }
}
```

***
## 4. GET/api​/v1​/Activities​/{5}
1. HTTP-метод-GET
2. Полный URL запроса-https://fakerestapi.azurewebsites.net/api/v1/Activities/5
3. Заголовки запроса-"accept: text/plain; v=1.0"
4. Тело запроса -отсутствует
5. Статус-код ответа-200
6. Тело ответа 
```
{
  "id": 5,
  "title": "Activity 5",
  "dueDate": "2023-06-14T10:34:25.9936717+00:00",
  "completed": false
}
```

***
## 5. GET/api​/v1​/Activities​/{9999999999999}
1. HTTP-метод-GET
2. Полный URL запроса-https://fakerestapi.azurewebsites.net/api/v1/Activities/9999999999999
3. Заголовки запроса-"accept: text/plain; v=1.0"
4. Тело запроса -отсутствует
5. Статус-код ответа-400
6. Тело ответа 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-4676eeb6d0ddbb46a730347ec47a14cb-a49c79857ce31745-00",
  "errors": {
    "id": [
      "The value '9999999999999' is not valid."
    ]
  }
}
```

***
## 6. PUT/api​/v1​/Activities​/{2}
1. HTTP-метод-PUT
2. Полный URL запроса-https://fakerestapi.azurewebsites.net/api/v1/Activities/2
3. Заголовки запроса-"accept: text/plain; v=1.0" ,"Content-Type: application/json; v=1.0"
4. Тело запроса 
```
{
  "id": 2,
  "title": "string",
  "dueDate": "2023-06-14T05:40:03.471Z",
  "completed": true
}
```
5. Статус-код ответа-200
6. Тело ответа 
```
{
  "id": 2,
  "title": "string",
  "dueDate": "2023-06-14T05:40:03.471Z",
  "completed": true
}
```
***
## 7. PUT/api​/v1​/Activities​/{2222222222}
1. HTTP-метод-PUT
2. Полный URL запроса-https://fakerestapi.azurewebsites.net/api/v1/Activities/2222222222
3. Заголовки запроса-"accept: text/plain; v=1.0" ,  "Content-Type: application/json; v=1.0" 
4. Тело запроса
```
{
  "id": 2222222222,
  "title": "string",
  "dueDate": "2023-06-14T05:40:03.471Z",
  "completed": true
}
``` 
5. Статус-код ответа-400
6. Тело ответа 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-2d7f01aa0c895a45a61d0d05175a70f4-516f27468275a646-00",
  "errors": {
    "id": [
      "The value '2222222222' is not valid."
    ],
    "$.id": [
      "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 0 | BytePositionInLine: 16."
    ]
  }
}
```
***
## 8. DELETE​/api​/v1​/Activities​/{55}
1. HTTP-метод-DELETE
2. Полный URL запроса-https://fakerestapi.azurewebsites.net/api/v1/Activities/55
3. Заголовки запроса-"accept: */*"
4. Тело запроса -отсутствует
5. Статус-код ответа-200
6. Тело ответа -отсутствует

***
## 9. GET​/api​/v1​/Authors
1. HTTP-метод-GET
2. Полный URL запроса-https://fakerestapi.azurewebsites.net/api/v1/Authors
3. Заголовки запроса- "accept: text/plain; v=1.0"
4. Тело запроса  -отсутствует
5. Статус-код ответа-200
6. Тело ответа 
```
 {
    "id": 1,
    "idBook": 1,
    "firstName": "First Name 1",
    "lastName": "Last Name 1"
  }
  ```

***
## 10. POST​/api​/v1​/Authors
1. HTTP-метод-POST
2. Полный URL запроса-https://fakerestapi.azurewebsites.net/api/v1/Authors
3. Заголовки запроса-"accept: text/plain; v=1.0" , "Content-Type: application/json; v=1.0" 
4. Тело запроса 
```
{
  "id": 4,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
5. Статус-код ответа-200
6. Тело ответа 
```
{
  "id": 4,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```

***
## 11. POST​/api​/v1​/Authors
1. HTTP-метод-POST
2. Полный URL запроса-https://fakerestapi.azurewebsites.net/api/v1/Authors
3. Заголовки запроса-"accept: text/plain; v=1.0", "Content-Type: application/json; v=1.0" 
4. Тело запроса 
```
{
  "id": 4444444111111111144,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
5. Статус-код ответа-400
6. Тело ответа 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-e65bc183f7672041aebb5f13760ce156-61eb9b0a0bb7d74f-00",
  "errors": {
    "$.id": [
      "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 0 | BytePositionInLine: 25."
    ]
  }
}
```

***
## 12. GET​/api​/v1​/Authors​/authors​/books​/{idBook}=1
1. HTTP-метод-GET
2. Полный URL запроса-https://fakerestapi.azurewebsites.net/api/v1/Authors/authors/books/1
3. Заголовки запроса-"accept: text/plain; v=1.0"
4. Тело запроса -отсутствует
5. Статус-код ответа-200
6. Тело ответа 
```
  {
    "id": 1,
    "idBook": 1,
    "firstName": "First Name 1",
    "lastName": "Last Name 1"
  }
  ```

***
## 13. GET​/api​/v1​/Authors​/authors​/books​/{idBook}=1111111111111
1. HTTP-метод-GET
2. Полный URL запроса-https://fakerestapi.azurewebsites.net/api/v1/Authors/authors/books/1111111111111
3. Заголовки запроса- "accept: text/plain; v=1.0"
4. Тело запроса  -отсутствует
5. Статус-код ответа-400
6. Тело ответа 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-dd89c3b36cb19a4cba6f07b00582aed2-d0d1c4739a8c7942-00",
  "errors": {
    "idBook": [
      "The value '1111111111111' is not valid."
    ]
  }
}
```

***
## 14. GET​/api​/v1​/Authors​/{id}=8
1. HTTP-метод-GET
2. Полный URL запроса-https://fakerestapi.azurewebsites.net/api/v1/Authors/8
3. Заголовки запроса- "accept: text/plain; v=1.0"
4. Тело запроса  -отсутствует
5. Статус-код ответа-200
6. Тело ответа 
```
{
  "id": 8,
  "idBook": 3,
  "firstName": "First Name 8",
  "lastName": "Last Name 8"
}
```

***
## 15. GET​/api​/v1​/Authors​/{id}=875645
1. HTTP-метод-GET
2. Полный URL запроса-https://fakerestapi.azurewebsites.net/api/v1/Authors/875645
3. Заголовки запроса- "accept: text/plain; v=1.0"
4. Тело запроса-отсутствует
5. Статус-код ответа-404
6. Тело ответа 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-512b5a1f712e2c43bb0d95e45e4f0a80-f9a80320ae770d42-00"
}
```

***
## 16. PUT​/api​/v1​/Authors​/{id}=87
1. HTTP-метод-PUT
2. Полный URL запроса-https://fakerestapi.azurewebsites.net/api/v1/Authors/87
3. Заголовки запроса- "accept: text/plain; v=1.0" ,  "Content-Type: application/json; v=1.0"
4. Тело запроса 
```
{
  "id": 87,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
5. Статус-код ответа-200
6. Тело ответа 
```
{
  "id": 87,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```

***
## 17. PUT​/api​/v1​/Authors​/{id}=8776756657
1. HTTP-метод-PUT
2. Полный URL запроса-https://fakerestapi.azurewebsites.net/api/v1/Authors/8776756657
3. Заголовки запроса-"accept: text/plain; v=1.0" , "Content-Type: application/json; v=1.0" 
4. Тело запроса 
```
{
  "id": 8776756657,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
5. Статус-код ответа-400
6. Тело ответа 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-ca9e613062c0664e986ec388b7900f0a-92e8dd2484235846-00",
  "errors": {
    "id": [
      "The value '8776756657' is not valid."
    ],
    "$.id": [
      "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 0 | BytePositionInLine: 16."
    ]
  }
}
```

***
## 18. DELETE​/api​/v1​/Authors​/{id}=567
1. HTTP-метод-DELETE
2. Полный URL запроса-https://fakerestapi.azurewebsites.net/api/v1/Authors/567
3. Заголовки запроса-"accept: */*"
4. Тело запроса -отсутствует
5. Статус-код ответа-200
6. Тело ответа -отсутствует

***
## 19. GET​/api​/v1​/Books
1. HTTP-метод-GET
2. Полный URL запроса-https://fakerestapi.azurewebsites.net/api/v1/Books
3. Заголовки запроса-"accept: text/plain; v=1.0"
4. Тело запроса -отсутствует
5. Статус-код ответа-200
6. Тело ответа 
```
{
    "id": 1,
    "title": "Book 1",
    "description": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
    "pageCount": 100,
    "excerpt": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
    "publishDate": "2023-06-13T07:44:19.365156+00:00"
  }
  ```

***
## 20. POST/api​/v1​/Books
1. HTTP-метод-POST
2. Полный URL запроса-https://fakerestapi.azurewebsites.net/api/v1/Books
3. Заголовки запроса-accept: "accept: */*" ,  "Content-Type: application/json; v=1.0" 
4. Тело запроса 
```
{
  "id": 3,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-14T07:46:06.410Z"
}
```
5. Статус-код ответа-200
6. Тело ответа 
```
{
  "id": 3,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-14T07:46:06.41Z"
}
```

***
## 21. POST/api​/v1​/Books
1. HTTP-метод-POST
2. Полный URL запроса-https://fakerestapi.azurewebsites.net/api/v1/Books
3. Заголовки запроса-"accept: */*" ,  "Content-Type: application/json; v=1.0" 
4. Тело запроса 
```
{
  "id": 38768778000006,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-14T07:46:06.410Z"
}
```
5. Статус-код ответа-400
6. Тело ответа 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-e0482049a9994f4097338c9d93d9927e-3fa0557e847a884f-00",
  "errors": {
    "$.id": [
      "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 0 | BytePositionInLine: 20."
    ]
  }
}
```

***
## 22. GET/api​/v1​/Books​/{id}=50
1. HTTP-метод-GET
2. Полный URL запроса-https://fakerestapi.azurewebsites.net/api/v1/Books/50
3. Заголовки запроса "accept: text/plain; v=1.0"
4. Тело запроса -отсутствует
5. Статус-код ответа-200
6. Тело ответа 
```
{
  "id": 50,
  "title": "Book 50",
  "description": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
  "pageCount": 5000,
  "excerpt": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
  "publishDate": "2023-04-25T07:52:39.1803816+00:00"
}
```

***
## 23. GET/api​/v1​/Books​/{id}=50765789
1. HTTP-метод-GET
2. Полный URL запроса-https://fakerestapi.azurewebsites.net/api/v1/Books/50765789
3. Заголовки запроса-"accept: text/plain; v=1.0"
4. Тело запроса -отсутствует
5. Статус-код ответа-404
6. Тело ответа 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-63f22c7c78314c4da012c1ce459cf9d4-08b62347774dff43-00"
}
```

***
## 24. PUT​/api​/v1​/Books​/{id}=40
1. HTTP-метод-PUT
2. Полный URL запроса-https://fakerestapi.azurewebsites.net/api/v1/Books/40
3. Заголовки запроса-"accept: */*" ,  "Content-Type: application/json; v=1.0"
4. Тело запроса
```
{
  "id": 40,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-14T07:55:21.081Z"
}
``` 
5. Статус-код ответа-200
6. Тело ответа 
```
{
  "id": 40,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-14T07:55:21.081Z"
}
```

***
## 25. PUT​/api​/v1​/Books​/{id}=4087567645345
1. HTTP-метод-PUT
2. Полный URL запроса-https://fakerestapi.azurewebsites.net/api/v1/Books/4087567645345
3. Заголовки запроса-"accept: */*" ,  "Content-Type: application/json; v=1.0" 
4. Тело запроса 
```
{
  "id": 4087567645345,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-14T07:55:21.081Z"
}
```
5. Статус-код ответа-400
6. Тело ответа 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-b64a2648efce894a8cd461d6ae23ac99-d2419d6eb888b448-00",
  "errors": {
    "id": [
      "The value '4087567645345' is not valid."
    ],
    "$.id": [
      "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 0 | BytePositionInLine: 19."
    ]
  }
}
```

***
## 26. DELETE​/api​/v1​/Books​/{id}=7
1. HTTP-метод-DELETE
2. Полный URL запроса-https://fakerestapi.azurewebsites.net/api/v1/Books/7
3. Заголовки запроса- "accept: */*"
4. Тело запроса -отсутствует
5. Статус-код ответа-200
6. Тело ответа -отсутствует

***
## 27. GET​/api​/v1​/CoverPhotos
1. HTTP-метод-GET
2. Полный URL запроса- https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos
3. Заголовки запроса- "accept: text/plain; v=1.0"
4. Тело запроса -отсутствует
5. Статус-код ответа-200
6. Тело ответа 
```
  {
    "id": 1,
    "idBook": 1,
    "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 1&w=250&h=350"
  }
  ```

***
## 28. POST​/api​/v1​/CoverPhotos
1. HTTP-метод-POST
2. Полный URL запроса- https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos
3. Заголовки запроса- "accept: text/plain; v=1.0" , "Content-Type: application/json; v=1.0" 
4. Тело запроса 
```
{
  "id": 5,
  "idBook": 0,
  "url": "string"
}
```
5. Статус-код ответа-200
6. Тело ответа 
```
{
  "id": 5,
  "idBook": 0,
  "url": "string"
}
```

***
## 29. POST​/api​/v1​/CoverPhotos
1. HTTP-метод- POST
2. Полный URL запроса-https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos
3. Заголовки запроса -"accept: text/plain; v=1.0" ,  "Content-Type: application/json; v=1.0" 
4. Тело запроса 
```
{
  "id": 75674530000045,
  "idBook": 0,
  "url": "string"
}
```
5. Статус-код ответа-400
6. Тело ответа 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-a11fe9b9f7a87143a128d8755aa937b6-00b193b2486a244e-00",
  "errors": {
    "$.id": [
      "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 0 | BytePositionInLine: 20."
    ]
  }
}
```

***
## 30. GET​/api​/v1​/CoverPhotos​/books​/covers​/{idBook}=6
1. HTTP-метод-GET
2. Полный URL запроса- https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/books/covers/6
3. Заголовки запроса- "accept: text/plain; v=1.0"
4. Тело запроса -отсутствует
5. Статус-код ответа-200
6. Тело ответа 
```
[
  {
    "id": 6,
    "idBook": 6,
    "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 6&w=250&h=350"
  }
]
```

***
## 31. GET​/api​/v1​/CoverPhotos​/books​/covers​/{idBook}=600000000005
1. HTTP-метод-GET
2. Полный URL запроса-https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/books/covers/600000000005
3. Заголовки запроса- "accept: text/plain; v=1.0"
4. Тело запроса  -отсутствует
5. Статус-код ответа-400
6. Тело ответа 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-184d0a524120da4f8b1da7ef984698f8-7de85f884ab9bc48-00",
  "errors": {
    "idBook": [
      "The value '600000000005' is not valid."
    ]
  }
}
```

***
## 32. GET​/api​/v1​/CoverPhotos​/{id}=1
1. HTTP-метод-GET
2. Полный URL запроса- https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/1
3. Заголовки запроса - "accept: text/plain; v=1.0"
4. Тело запроса  -отсутствует
5. Статус-код ответа-200
6. Тело ответа 
```
{
  "id": 1,
  "idBook": 1,
  "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 1&w=250&h=350"
}
```

***
## 33. GET​/api​/v1​/CoverPhotos​/{id}=148697
1. HTTP-метод-GET
2. Полный URL запроса-https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/148697
3. Заголовки запроса-  "accept: text/plain; v=1.0"
4. Тело запроса  -отсутствует
5. Статус-код ответа-404
6. Тело ответа 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-1710dd6af8dfe44a99106b3636d45a03-6ff59fcb3e1f2d4b-00"
}
```

***
## 34. PUT​/api​/v1​/CoverPhotos​/{id}=804
1. HTTP-метод-PUT
2. Полный URL запроса- https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/804
3. Заголовки запроса-  "accept: text/plain; v=1.0" ,  "Content-Type: application/json; v=1.0"
4. Тело запроса 
```
{
  "id": 804,
  "idBook": 0,
  "url": "string"
}
```
5. Статус-код ответа-200
6. Тело ответа 
```
{
  "id": 804,
  "idBook": 0,
  "url": "string"
}
```

***
## 35. PUT​/api​/v1​/CoverPhotos​/{id}=8042342889779
1. HTTP-метод-PUT
2. Полный URL запроса- https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/8042342889779
3. Заголовки запроса- "accept: text/plain; v=1.0" , "Content-Type: application/json; v=1.0"
4. Тело запроса 
```
{
  "id": 8042342889779,
  "idBook": 0,
  "url": "string"
}
```
5. Статус-код ответа-400
6. Тело ответа 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-97c2f08cb6e5e945bb7b37497a537a2c-0a2ba6fd97e59647-00",
  "errors": {
    "id": [
      "The value '8042342889779' is not valid."
    ],
    "$.id": [
      "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 0 | BytePositionInLine: 19."
    ]
  }
}
```

***
## 36. DELETE​/api​/v1​/CoverPhotos​/{id}=3
1. HTTP-метод-DELETE
2. Полный URL запроса- https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/3
3. Заголовки запроса-"accept: */*"
4. Тело запроса  -отсутствует
5. Статус-код ответа-200
6. Тело ответа  -отсутствует

***
## 37.GET/api​/v1​/Users
1. HTTP-метод-GET
2. Полный URL запроса- https://fakerestapi.azurewebsites.net/api/v1/Users
3. Заголовки запроса-  "accept: text/plain; v=1.0"
4. Тело запроса -отсутствует
5. Статус-код ответа-200
6. Тело ответа 
```
 {
    "id": 1,
    "userName": "User 1",
    "password": "Password1"
  }
  ```

***
## 38. POST​/api​/v1​/Users
1. HTTP-метод-POST
2. Полный URL запроса-https://fakerestapi.azurewebsites.net/api/v1/Users
3. Заголовки запроса- "accept: */*" , "Content-Type: application/json; v=1.0"
4. Тело запроса 
```
{
  "id": 34,
  "userName": "string",
  "password": "string"
}
```
5. Статус-код ответа-200
6. Тело ответа 
```
{
  "id": 34,
  "userName": "string",
  "password": "string"
}
```

***
## 39. POST​/api​/v1​/Users
1. HTTP-метод-POST
2. Полный URL запроса-https://fakerestapi.azurewebsites.net/api/v1/Users
3. Заголовки запроса- "accept: */*" , "Content-Type: application/json; v=1.0"
4. Тело запроса 
```
{
  "id": 34654000064,
  "userName": "string",
  "password": "string"
}
```
5. Статус-код ответа-400
6. Тело ответа 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-b7c7f2b6a7f48540a7ec7771cb738378-3151d5e74adb4947-00",
  "errors": {
    "$.id": [
      "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 0 | BytePositionInLine: 17."
    ]
  }
}
```

***
## 40. GET​/api​/v1​/Users​/{id}=2
1. HTTP-метод-GET
2. Полный URL запроса- https://fakerestapi.azurewebsites.net/api/v1/Users/2
3. Заголовки запроса-  "accept: */*"
4. Тело запроса  -отсутствует
5. Статус-код ответа-200
6. Тело ответа 
```
{
  "id": 2,
  "userName": "User 2",
  "password": "Password2"
}
```

***
## 41. GET​/api​/v1​/Users​/{id}=37
1. HTTP-метод-GET
2. Полный URL запроса- https://fakerestapi.azurewebsites.net/api/v1/Users/37
3. Заголовки запроса- "accept: */*"
4. Тело запроса -отсутствует
5. Статус-код ответа-404
6. Тело ответа 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-eaf7d0af04e111409f87f9aaa28deaaf-50a0e75d43a8aa4a-00"
}
```

***
## 42. PUT​/api​/v1​/Users​/{id}=777
1. HTTP-метод-PUT
2. Полный URL запроса- https://fakerestapi.azurewebsites.net/api/v1/Users/777
3. Заголовки запроса-"accept: */*" ,"Content-Type: application/json; v=1.0"
4. Тело запроса 
```
{
  "id": 777,
  "userName": "string",
  "password": "string"
}
```
5. Статус-код ответа-200
6. Тело ответа 
```
{
  "id": 777,
  "userName": "string",
  "password": "string"
}
```

***
## 43. PUT​/api​/v1​/Users​/{id}=77765435456561
1. HTTP-метод-PUT
2. Полный URL запроса- https://fakerestapi.azurewebsites.net/api/v1/Users/77765435456561
3. Заголовки запроса - "accept: */*",  "Content-Type: application/json; v=1.0"
4. Тело запроса 
```
{
  "id": 77765435456561,
  "userName": "string",
  "password": "string"
}
```
5. Статус-код ответа-400
6. Тело ответа 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-fa6c982a2ac2f945a47980aff1971226-a1893ecec143ee44-00",
  "errors": {
    "id": [
      "The value '77765435456561' is not valid."
    ],
    "$.id": [
      "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 0 | BytePositionInLine: 20."
    ]
  }
}
```

***
## 44. DELETE/api​/v1​/Users​/{id}=55
1. HTTP-метод-DELETE
2. Полный URL запроса- https://fakerestapi.azurewebsites.net/api/v1/Users/55
3. Заголовки запроса -"accept: */*"
4. Тело запроса -отсутствует
5. Статус-код ответа-200
6. Тело ответа -отсутствует

***
