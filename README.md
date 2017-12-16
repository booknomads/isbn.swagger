# BookNomads ISBN search API swagger spec

[![BookNomads](https://www.booknomads.com/img/logo-circle.png)](https://www.booknomads.com/dev)

2.5 million books processed from titelbank.nl

## https://www.booknomads.com/api/v0/isbn/{ISBN}
example usage:

```
$ curl -s https://www.booknomads.com/api/v0/isbn/9789000010134 | json_pp
{
   "LanguageCode" : "nl",
   "Title" : "Tobbe",
   "CoverThumb" : "data:image/jpeg;base64,/9j/2wCEAAgGBgcGBQgHBwcJ....",
   "Description" : "",
   "ISBN" : "9789000035526",
   "Subtitle" : "",
   "Subjects": ["Fictie 13-15 jaar"],
   "Authors" : [
      {
         "Name" : "M.  Engstrom"
      },
      {
         "Name" : "B.  Custers"
      }
   ]
}
```

The thumbnails are base64 encoded images(scaled to 200x200 using https://github.com/nfnt/resize).

Try it out at [https://app.swaggerhub.com/apis/BookNomads/book_by_isbn/1.0.0](https://app.swaggerhub.com/apis/BookNomads/book_by_isbn/1.0.0)

Read more at [https://www.booknomads.com/dev](https://www.booknomads.com/dev)

