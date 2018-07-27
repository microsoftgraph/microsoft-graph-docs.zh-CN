# <a name="open-the-onenote-client"></a><span data-ttu-id="c7a7a-101">打开 OneNote 客户端</span><span class="sxs-lookup"><span data-stu-id="c7a7a-101">Open the OneNote client</span></span>

<span data-ttu-id="c7a7a-102">可以使用页面或笔记本的 **links** 属性将 OneNote 应用程序打开到特定的页面或笔记本。</span><span class="sxs-lookup"><span data-stu-id="c7a7a-102">You can use the **links** property of a page or notebook to open a OneNote application to a particular page or notebook.</span></span> 

<span data-ttu-id="c7a7a-103">**links** 属性是一个 JSON 对象，它包含两个 URL。</span><span class="sxs-lookup"><span data-stu-id="c7a7a-103">The **links** property is a JSON object that contains two URLs.</span></span> <span data-ttu-id="c7a7a-104">URL 将在 OneNote 客户端应用程序或 OneNote Online 中打开页面或笔记本。</span><span class="sxs-lookup"><span data-stu-id="c7a7a-104">The URLs will open the page or notebook in the OneNote client application or in OneNote Online.</span></span>

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

- <span data-ttu-id="c7a7a-105">**oneNoteClientUrl**</span><span class="sxs-lookup"><span data-stu-id="c7a7a-105">**oneNoteClientUrl**</span></span> 

    - <span data-ttu-id="c7a7a-106">打开 OneNote 客户端（如果设备上已安装）。</span><span class="sxs-lookup"><span data-stu-id="c7a7a-106">oneNoteClientUrl - Opens the OneNote client if it is already installed on the device.</span></span> <span data-ttu-id="c7a7a-107">此 URL 包括 *onenote* 前缀。</span><span class="sxs-lookup"><span data-stu-id="c7a7a-107">This URL includes the *onenote* prefix.</span></span>
    - <span data-ttu-id="c7a7a-108">如果设备上安装了特定于语言的版本，则打开该版本。</span><span class="sxs-lookup"><span data-stu-id="c7a7a-108">Opens the language-specific version if one is installed on the device.</span></span> <span data-ttu-id="c7a7a-109">否则，请使用平台语言设置。</span><span class="sxs-lookup"><span data-stu-id="c7a7a-109">Otherwise, uses the platform language setting.</span></span>

- <span data-ttu-id="c7a7a-110">**oneNoteWebUrl**</span><span class="sxs-lookup"><span data-stu-id="c7a7a-110">**oneNoteWebUrl**</span></span> 

    - <span data-ttu-id="c7a7a-111">打开 OneNote Online（如果设备上的默认浏览器支持）。</span><span class="sxs-lookup"><span data-stu-id="c7a7a-111">oneNoteWebUrl - Opens OneNote Online if the default browser on the device supports it.</span></span> 
    - <span data-ttu-id="c7a7a-112">使用浏览器语言设置。</span><span class="sxs-lookup"><span data-stu-id="c7a7a-112">Uses the browser language setting.</span></span>


<span data-ttu-id="c7a7a-113">OneNote API 在以下操作的 HTTP 响应中返回 **links** 属性：</span><span class="sxs-lookup"><span data-stu-id="c7a7a-113">The OneNote API returns the **links** property in the HTTP response for the following operations:</span></span>

- <span data-ttu-id="c7a7a-114">通过发送 [`POST pages`](../api-reference/v1.0/api/section_post_pages.md) 请求创建页面。</span><span class="sxs-lookup"><span data-stu-id="c7a7a-114">Create a page by sending a [`POST pages`](../api-reference/v1.0/api/section_post_pages.md) request</span></span>

- <span data-ttu-id="c7a7a-115">通过发送 [`POST notebooks`](../api-reference/v1.0/api/onenote_post_notebooks.md) 请求创建笔记本。</span><span class="sxs-lookup"><span data-stu-id="c7a7a-115">Create a notebook by sending a [`POST notebooks`](../api-reference/v1.0/api/onenote_post_notebooks.md) request</span></span>

- <span data-ttu-id="c7a7a-116">通过发送 [`GET pages`](../api-reference/v1.0/api/page_get.md) 或 [`GET pages/{id}`](../api-reference/v1.0/api/page_get.md) 请求获取页面元数据。</span><span class="sxs-lookup"><span data-stu-id="c7a7a-116">Get page metadata by sending a [`GET pages`](../api-reference/v1.0/api/page_get.md) or [`GET pages/{id}`](../api-reference/v1.0/api/page_get.md) request</span></span>

- <span data-ttu-id="c7a7a-117">通过发送 [`GET notebooks`](../api-reference/v1.0/api/notebook_get.md) 或 [`GET notebooks/{id}`](../api-reference/v1.0/api/notebook_get.md) 请求获取笔记本元数据。</span><span class="sxs-lookup"><span data-stu-id="c7a7a-117">Get notebook metadata by sending a [`GET notebooks`](../api-reference/v1.0/api/notebook_get.md) or [`GET notebooks/{id}`](../api-reference/v1.0/api/notebook_get.md) request</span></span>

<span data-ttu-id="c7a7a-118">下面的示例显示如何检查响应的状态代码、分析 JSON 以提取 URL，然后打开 OneNote 客户端。</span><span class="sxs-lookup"><span data-stu-id="c7a7a-118">The following examples show how to check the status code of the response, parse the JSON to extract the URLs, and then open the OneNote client.</span></span>

## <a name="ios-example"></a><span data-ttu-id="c7a7a-119">iOS 示例</span><span class="sxs-lookup"><span data-stu-id="c7a7a-119">iOS example</span></span>

<span data-ttu-id="c7a7a-120">下面的示例从 JSON 响应获取 OneNote 客户端 URL。</span><span class="sxs-lookup"><span data-stu-id="c7a7a-120">The following example gets the OneNote client URLs from the JSON response.</span></span> <span data-ttu-id="c7a7a-121">它使用 AFNetworking 库 (http://afnetworking.com/)) 提取两个 URL。</span><span class="sxs-lookup"><span data-stu-id="c7a7a-121">It uses the AFNetworking library (http://afnetworking.com/) to extract the two URLs.</span></span> <span data-ttu-id="c7a7a-122">在示例中，`created` 是指向用于存储响应值的 **ONSCPSStandardResponse** 对象的指针，`responseObject` 包含已分析的 JSON。</span><span class="sxs-lookup"><span data-stu-id="c7a7a-122">In the example, `created` is a pointer to the ONSCPSStandardResponse object used to store the response values, and `responseObject` holds the parsed JSON.</span></span>

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

<span data-ttu-id="c7a7a-123">分析响应中的 URL 后，可以通过使用以下代码打开 OneNote。</span><span class="sxs-lookup"><span data-stu-id="c7a7a-123">After you parse the URLs from the response, you can open OneNote by using the following code.</span></span> <span data-ttu-id="c7a7a-124">使用 `oneNoteClientUrl` 打开已安装的 OneNote 客户端，或使用 `oneNoteWebURL` 打开 OneNote Online。</span><span class="sxs-lookup"><span data-stu-id="c7a7a-124">Use `oneNoteClientUrl` to open the installed OneNote client or `oneNoteWebURL` to open OneNote Online.</span></span>

```objc
NSURL *url = [NSURL URLWithString:standardResponse.oneNoteWebUrl];
[[UIApplication sharedApplication] openURL:url];
```

## <a name="android-example"></a><span data-ttu-id="c7a7a-125">Android 示例</span><span class="sxs-lookup"><span data-stu-id="c7a7a-125">Android example</span></span>

<span data-ttu-id="c7a7a-126">首先，检查成功的状态代码，然后分析 JSON。</span><span class="sxs-lookup"><span data-stu-id="c7a7a-126">First, check for the success status code and then parse the JSON.</span></span> <span data-ttu-id="c7a7a-127">该示例假定已发送 POST 请求，因此，它会检查 `201 Created` 状态代码。</span><span class="sxs-lookup"><span data-stu-id="c7a7a-127">The example assumes a POST request was sent, so it checks for a `201 Created` status code.</span></span> <span data-ttu-id="c7a7a-128">如果发出了 `GET` 请求，则应检查 `200` 状态代码。</span><span class="sxs-lookup"><span data-stu-id="c7a7a-128">If you made a `GET` request, check for a `200` status code instead.</span></span>

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

<span data-ttu-id="c7a7a-129">借助响应属性，应用可以打开 OneNote Online，如下面的示例中所示。</span><span class="sxs-lookup"><span data-stu-id="c7a7a-129">Using the response properties, your app can open OneNote Online, as shown in the following example.</span></span>

```java 
if (response.getResponseCode() == 201) {
    Uri uriUrl = Uri.parse(response.getOneNoteWebUrl);  
    Intent launchBrowser = new Intent(Intent.ACTION_VIEW, uriUrl); 
    startActivity(launchBrowser);
}
```

<br/>

<span data-ttu-id="c7a7a-130">或者，应用可以打开 Android 设备上的 OneNote 客户端。</span><span class="sxs-lookup"><span data-stu-id="c7a7a-130">Or your app can open the OneNote client on an Android device.</span></span> <span data-ttu-id="c7a7a-131">使用 `oneNoteClientUrl` 属性时，必须先用大括号 `{ }` 将 GUID 字符串括起来，然后再开始操作。</span><span class="sxs-lookup"><span data-stu-id="c7a7a-131">When using the `oneNoteClientUrl` property, you must surround the GUID strings with braces `{ }` before starting the Intent.</span></span> <span data-ttu-id="c7a7a-132">以下示例演示如何执行此操作。</span><span class="sxs-lookup"><span data-stu-id="c7a7a-132">The following example shows how to do that.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="c7a7a-133">另请参阅</span><span class="sxs-lookup"><span data-stu-id="c7a7a-133">See also</span></span>

- [<span data-ttu-id="c7a7a-134">获取 OneNote 内容和结构</span><span class="sxs-lookup"><span data-stu-id="c7a7a-134">Get OneNote content and structure</span></span>](onenote-get-content.md)
- [<span data-ttu-id="c7a7a-135">创建 OneNote 页</span><span class="sxs-lookup"><span data-stu-id="c7a7a-135">Create OneNote pages</span></span>](onenote-create-page.md)