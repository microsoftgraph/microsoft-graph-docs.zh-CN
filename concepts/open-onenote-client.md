---
title: 使用 OneNote API 打开 OneNote 客户端
description: 使用页面或笔记本的 links 属性将 OneNote 应用程序打开到特定页面或笔记本。 包括 iOS 和 Android 示例。
author: Jewan-microsoft
ms.localizationpriority: medium
ms.openlocfilehash: 92f469aa8eb7e508532d34b7d4efd0feac3ca411
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444787"
---
# <a name="open-the-onenote-client"></a>打开 OneNote 客户端

可以使用页面或笔记本的 **links** 属性将 OneNote 应用程序打开到特定的页面或笔记本。 

**links** 属性是一个 JSON 对象，它包含两个 URL。 URL 将在 OneNote 客户端应用程序或OneNote web 版中打开页面或笔记本。

```json
{ 
    "links": {
        "oneNoteClientUrl": {
            "href": "onenote:https://..."
        },
        "oneNoteWebUrl": {
            "href": "https://..."
        }
    }
}
```

- **oneNoteClientUrl**

  - 打开 OneNote 客户端（如果设备上已安装）。 此 URL 包括 *onenote* 前缀。
  - 如果设备上安装了特定于语言的版本，则打开该版本。 否则，请使用平台语言设置。

- **oneNoteWebUrl**

  - 如果设备上的默认浏览器支持，则打开OneNote web 版。
  - 使用浏览器语言设置。


OneNote API 在以下操作的 HTTP 响应中返回 **links** 属性：

- 通过发送 [`POST pages`](/graph/api/section-post-pages) 请求创建页面。

- 通过发送 [`POST notebooks`](/graph/api/onenote-post-notebooks) 请求创建笔记本。

- 通过发送 [`GET pages`](/graph/api/page-get) 或 [`GET pages/{id}`](/graph/api/page-get) 请求获取页面元数据。

- 通过发送 [`GET notebooks`](/graph/api/notebook-get) 或 [`GET notebooks/{id}`](/graph/api/notebook-get) 请求获取笔记本元数据。

下面的示例显示如何检查响应的状态代码、分析 JSON 以提取 URL，然后打开 OneNote 客户端。

## <a name="ios-example"></a>iOS 示例

下面的示例从 JSON 响应获取 OneNote 客户端 URL。 它使用 AFNetworking 库 (https://afnetworking.com/)) 提取两个 URL。 在示例中，`created` 是指向用于存储响应值的 **ONSCPSStandardResponse** 对象的指针，`responseObject` 包含已分析的 JSON。

```objc
    /* Import the JSON library */
    #import "AFURLRequestSerialization.h"

    - (void)connectionDidFinishLoading:(NSURLConnection *)connection {
            if(delegate) {
                  int status = [returnResponse statusCode];
                  ONSCPSStandardResponse *standardResponse = nil;
                  if (status == 201) {
                        ONSCPSCreateSuccessResponse *created = 
                              [[ONSCPSCreateSuccessResponse alloc] init];
                        created.httpStatusCode = status;
                        NSError *jsonError;
                        NSDictionary *responseObject = 
                              [NSJSONSerialization JSONObjectWithData:returnData options:0 error:&jsonError];
                        if(responseObject && !jsonError) {
                              created.oneNoteClientUrl = ((NSDictionary *)
                                    ((NSDictionary *)responseObject[@"links"])[@"oneNoteClientUrl"])[@"href"];
                              created.oneNoteWebUrl = ((NSDictionary *)
                                    ((NSDictionary *)responseObject[@"links"])[@"oneNoteWebUrl"])[@"href"];
                        }
                  standardResponse = created;
                  }
                  else {
                        ONSCPSStandardErrorResponse *error = [[ONSCPSStandardErrorResponse alloc] init];
                        error.httpStatusCode = status;
                        error.message = [[NSString alloc] initWithData:returnData 
                              encoding:NSUTF8StringEncoding];
                        standardResponse = error;
                  }
                  // Send the response back to the client.
                  if (standardResponse) {
                        [delegate exampleServiceActionDidCompleteWithResponse: standardResponse];
                  }
            }
      }
``` 

<br/>

分析响应中的 URL 后，可以通过使用以下代码打开 OneNote。 用于`oneNoteClientUrl`打开已安装的 OneNote 客户端或`oneNoteWebURL`打开OneNote web 版。

```objc
NSURL *url = [NSURL URLWithString:standardResponse.oneNoteWebUrl];
[[UIApplication sharedApplication] openURL:url];
```

## <a name="android-example"></a>Android 示例

首先，检查成功的状态代码，然后分析 JSON。 该示例假定已发送 POST 请求，因此，它会检查 `201 Created` 状态代码。 如果发出了 `GET` 请求，则应检查 `200` 状态代码。

```java
public ApiResponse getResponse() throws Exception {
    /* Get the HTTP response code and message from the connection object */
    int responseCode = mUrlConnection.getResponseCode();
    String responseMessage = mUrlConnection.getResponseMessage();
    String responseBody = null;

    /* Get the response if the new page was created successfully. */
    if ( responseCode == 201) {
        InputStream is = mUrlConnection.getInputStream();

        /* Verify that this byte array is big enough. */
        byte[] b1 = new byte[1024];
        StringBuffer buffer = new StringBuffer();

        /* Copy the body of the response into the new string. */
        /* Make sure the buffer is big enough. */
        while ( is.read(b1) != -1)
            buffer.append(new String(b1));

      /* When the returned data is complete, close the connection 
         and convert the byte array into a string. */
        mUrlConnection.disconnect();
        responseBody =  buffer.toString();
    }

    /* Create a new JSON object, and an object to hold the response URLs. */
    JSONObject responseObject = null;
    ApiResponse response = new ApiResponse();
    try {

        /* Store and verify the HTTP response code. */
        response.setResponseCode(responseCode);
        response.setResponseMessage(responseMessage);
        if ( responseCode == 201) {

            /* Retrieve the two URLs from the links property. */
            responseObject = new JSONObject(responseBody);
            String clientUrl = responseObject.getJSONObject(
                "links").getJSONObject("oneNoteClientUrl").getString("href");
            String webUrl = responseObject.getJSONObject(
                "links").getJSONObject("oneNoteWebUrl").getString("href");
            response.setOneNoteClientUrl(clientUrl);
            response.setOneNoteWebUrl(webUrl);
        }
    } catch (JSONException ex) {

        /* If the JSON was malformed or incomplete... */
        String msg = ex.getMessage();
        msg = msg;
    }
    return response;
}
```

<br/>

使用响应属性，应用可以打开OneNote web 版，如以下示例所示。

```java 
if (response.getResponseCode() == 201) {
    Uri uriUrl = Uri.parse(response.getOneNoteWebUrl);  
    Intent launchBrowser = new Intent(Intent.ACTION_VIEW, uriUrl); 
    startActivity(launchBrowser);
}
```

<br/>

或者，应用可以打开 Android 设备上的 OneNote 客户端。 使用 `oneNoteClientUrl` 属性时，必须先用大括号 `{ }` 将 GUID 字符串括起来，然后再开始操作。 以下示例演示如何执行此操作。

```java 
if (response.getResponseCode() == 201) {

    // Get the URL from the OneNote API JSON response.
    String onenoteClientUrl = obtainClientLinkFromJSONResponse();
    String androidClientUrl = 
        onenoteClientUrl.replaceAll(
            "=([0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{12})&",
            "={$1}&");

    // Open the URL: Open the newly created OneNote page.
    Uri uriUrl = Uri.parse(androidClientUrl);  
    Intent launchBrowser = new Intent(Intent.ACTION_VIEW, uriUrl); 
    startActivity(launchBrowser);
}
```

## <a name="see-also"></a>另请参阅

- [获取 OneNote 内容和结构](onenote-get-content.md)
- [创建 OneNote 页](onenote-create-page.md)
