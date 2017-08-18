# <a name="list-attachments"></a><span data-ttu-id="c6616-101">列出附件</span><span class="sxs-lookup"><span data-stu-id="c6616-101">List attachments</span></span>

<span data-ttu-id="c6616-102">检索附加到帖子的 [attachment](../resources/attachment.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="c6616-102">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c6616-103">先决条件</span><span class="sxs-lookup"><span data-stu-id="c6616-103">Prerequisites</span></span>
<span data-ttu-id="c6616-104">要执行此 API，需要以下**范围**之一：</span><span class="sxs-lookup"><span data-stu-id="c6616-104">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="c6616-105">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6616-105">Group.Read.All</span></span>
* <span data-ttu-id="c6616-106">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6616-106">Group.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="c6616-107">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c6616-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="c6616-108">属于组的 [对话](../resources/conversation.md) 的 [线程](../resources/conversationthread.md) 中的 [帖子](../resources/post.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="c6616-108">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c6616-109">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c6616-109">Optional query parameters</span></span>
<span data-ttu-id="c6616-110">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c6616-110">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c6616-111">请求标头</span><span class="sxs-lookup"><span data-stu-id="c6616-111">Request headers</span></span>
| <span data-ttu-id="c6616-112">标头</span><span class="sxs-lookup"><span data-stu-id="c6616-112">Header</span></span>       | <span data-ttu-id="c6616-113">值</span><span class="sxs-lookup"><span data-stu-id="c6616-113">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c6616-114">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6616-114">Authorization</span></span>  | <span data-ttu-id="c6616-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c6616-p101">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c6616-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="c6616-117">Request body</span></span>
<span data-ttu-id="c6616-118">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c6616-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6616-119">响应</span><span class="sxs-lookup"><span data-stu-id="c6616-119">Response</span></span>

<span data-ttu-id="c6616-120">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Attachment](../resources/attachment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c6616-120">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c6616-121">示例</span><span class="sxs-lookup"><span data-stu-id="c6616-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c6616-122">请求</span><span class="sxs-lookup"><span data-stu-id="c6616-122">Request</span></span>
<span data-ttu-id="c6616-123">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c6616-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="c6616-124">响应</span><span class="sxs-lookup"><span data-stu-id="c6616-124">Response</span></span>
<span data-ttu-id="c6616-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c6616-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
      "id": "id-value",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "isInline": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
