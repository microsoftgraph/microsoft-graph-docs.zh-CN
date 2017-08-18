# <a name="list-overrides"></a><span data-ttu-id="76084-101">列出替代</span><span class="sxs-lookup"><span data-stu-id="76084-101">List overrides</span></span>

<span data-ttu-id="76084-102">获取用户设置为始终以特定方式对来自特定发件人的邮件进行分类的替代。</span><span class="sxs-lookup"><span data-stu-id="76084-102">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="76084-p101">每个替代均对应一个发件人的 SMTP 地址。最初，用户没有任何替代。</span><span class="sxs-lookup"><span data-stu-id="76084-p101">Each override corresponds to an SMTP address of a sender. Initially, a user does not have any overrides.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="76084-105">先决条件</span><span class="sxs-lookup"><span data-stu-id="76084-105">Prerequisites</span></span>
<span data-ttu-id="76084-106">要执行此 API，需要以下**范围**：*Mail.Read*</span><span class="sxs-lookup"><span data-stu-id="76084-106">The following **scopes** are required to execute this API: *Mail.Read*</span></span>
## <a name="http-request"></a><span data-ttu-id="76084-107">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="76084-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="76084-108">请求标头</span><span class="sxs-lookup"><span data-stu-id="76084-108">Request headers</span></span>
| <span data-ttu-id="76084-109">名称</span><span class="sxs-lookup"><span data-stu-id="76084-109">Name</span></span>       | <span data-ttu-id="76084-110">类型</span><span class="sxs-lookup"><span data-stu-id="76084-110">Type</span></span> | <span data-ttu-id="76084-111">说明</span><span class="sxs-lookup"><span data-stu-id="76084-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="76084-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="76084-112">Authorization</span></span>  | <span data-ttu-id="76084-113">string</span><span class="sxs-lookup"><span data-stu-id="76084-113">string</span></span>  | <span data-ttu-id="76084-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="76084-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="76084-116">请求正文</span><span class="sxs-lookup"><span data-stu-id="76084-116">Request body</span></span>
<span data-ttu-id="76084-117">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="76084-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76084-118">响应</span><span class="sxs-lookup"><span data-stu-id="76084-118">Response</span></span>

<span data-ttu-id="76084-p103">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) 对象集合。如果用户未设置任何替代，则返回空集合。</span><span class="sxs-lookup"><span data-stu-id="76084-p103">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body. An empty collection is returned if the user doesn't have any overrides set up.</span></span>
## <a name="example"></a><span data-ttu-id="76084-121">示例</span><span class="sxs-lookup"><span data-stu-id="76084-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="76084-122">请求</span><span class="sxs-lookup"><span data-stu-id="76084-122">Request</span></span>
<span data-ttu-id="76084-123">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="76084-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides
```
##### <a name="response"></a><span data-ttu-id="76084-124">响应</span><span class="sxs-lookup"><span data-stu-id="76084-124">Response</span></span>
<span data-ttu-id="76084-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="76084-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "classifyAs": "focused",
      "senderEmailAddress": {
        "name": "Fanny Downs",
        "address": "fannyd@adatum.onmicrosoft.com"
      },
      "id": "98f5bdef-576a-404d-a2ea-07a3cf11a9b9"
    },
    {
      "classifyAs": "other",
      "senderEmailAddress": {
        "name": "Randi Welch",
        "address": "randiw@adatum.onmicrosoft.com"
      },
      "id": "98f5bdef-576a-404d-a2ea-07a3cf34af4r"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List overrides",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->