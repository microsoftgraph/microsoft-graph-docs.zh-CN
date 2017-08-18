# <a name="get-conversationthread"></a><span data-ttu-id="0b1a5-101">获取 conversationThread</span><span class="sxs-lookup"><span data-stu-id="0b1a5-101">Get conversationThread</span></span>

<span data-ttu-id="0b1a5-p101">获取属于某个组的特定线程。可以指定父对话和线程，也可以指定线程，而不引用父对话。</span><span class="sxs-lookup"><span data-stu-id="0b1a5-p101">Get a specific thread that belongs to a group. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span> 
## <a name="prerequisites"></a><span data-ttu-id="0b1a5-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="0b1a5-104">Prerequisites</span></span>
<span data-ttu-id="0b1a5-105">要执行此 API，需要以下**范围**之一：*Group.ReadWrite.All；Group.Read.All*</span><span class="sxs-lookup"><span data-stu-id="0b1a5-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All; Group.Read.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="0b1a5-106">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b1a5-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
GET /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="0b1a5-107">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0b1a5-107">Optional query parameters</span></span>
<span data-ttu-id="0b1a5-108">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0b1a5-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0b1a5-109">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b1a5-109">Request headers</span></span>
| <span data-ttu-id="0b1a5-110">标头</span><span class="sxs-lookup"><span data-stu-id="0b1a5-110">Header</span></span>       | <span data-ttu-id="0b1a5-111">值</span><span class="sxs-lookup"><span data-stu-id="0b1a5-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0b1a5-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b1a5-112">Authorization</span></span>  | <span data-ttu-id="0b1a5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0b1a5-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0b1a5-115">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b1a5-115">Request body</span></span>
<span data-ttu-id="0b1a5-116">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0b1a5-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b1a5-117">响应</span><span class="sxs-lookup"><span data-stu-id="0b1a5-117">Response</span></span>

<span data-ttu-id="0b1a5-118">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationThread](../resources/conversationthread.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0b1a5-118">If successful, this method returns a `200 OK` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0b1a5-119">示例</span><span class="sxs-lookup"><span data-stu-id="0b1a5-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0b1a5-120">请求</span><span class="sxs-lookup"><span data-stu-id="0b1a5-120">Request</span></span>
<span data-ttu-id="0b1a5-121">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0b1a5-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversationthread"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="0b1a5-122">响应</span><span class="sxs-lookup"><span data-stu-id="0b1a5-122">Response</span></span>
<span data-ttu-id="0b1a5-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0b1a5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 419

{
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "datetime-value",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "ccRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
