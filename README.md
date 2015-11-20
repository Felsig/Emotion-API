# Emotion-API
[![Build status](https://ci.appveyor.com/api/projects/status/oscx09t7s06sgiqc?svg=true)](https://ci.appveyor.com/project/Felsig/emotion-api/branch/master)
[![License][license-image]][license-url]
[license-image]: http://img.shields.io/badge/license-MIT-green.svg
[license-url]: LICENSE

###Summary
.Net 4.6 class library that wraps the Microsoft Project Oxford [Emotion API](https://www.projectoxford.ai/doc/Emotion/overview) for easier, simpler use inside your .Net application.

###Usage examples
```c#
var client = new EmotionAPIClient("{your_api_key}");
var response = client.Post("{image_url}");

foreach(var item in response)
{
  // item.Scores.Anger;
  // item.FaceRectangle.Height;
  // ...
}
```

###License
Licensed under the MIT License
