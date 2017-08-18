# <a name="list-rejectedsenders"></a><span data-ttu-id="97dbf-101">列出 rejectedSender</span><span class="sxs-lookup"><span data-stu-id="97dbf-101">List rejectedSenders</span></span>

<span data-ttu-id="97dbf-102">获取此组 rejectedSenders 列表中的用户或组列表。</span><span class="sxs-lookup"><span data-stu-id="97dbf-102">Get a list of users or groups that are in the rejectedSenders list for this group.</span></span> 

<span data-ttu-id="97dbf-p101">已拒绝的发件人列表中的用户无法发布到组对话（在 GET 请求 URL 中标识）。确保未在拒绝的发件人和接受的发件人列表中指定同一用户或组，否则会发生错误。</span><span class="sxs-lookup"><span data-stu-id="97dbf-p101">Users in the rejected senders list cannot post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="97dbf-105">先决条件</span><span class="sxs-lookup"><span data-stu-id="97dbf-105">Prerequisites</span></span>
<span data-ttu-id="97dbf-106">要执行此 API，需要以下**范围**之一：*Group.Read.All* 或 *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="97dbf-106">One of the following **scopes** is required to execute this API: *Group.Read.All* or *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="97dbf-107">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="97dbf-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/rejectedSenders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="97dbf-108">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="97dbf-108">Optional query parameters</span></span>
<span data-ttu-id="97dbf-109">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="97dbf-109">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="97dbf-110">请求标头</span><span class="sxs-lookup"><span data-stu-id="97dbf-110">Request headers</span></span>
| <span data-ttu-id="97dbf-111">标头</span><span class="sxs-lookup"><span data-stu-id="97dbf-111">Header</span></span>       | <span data-ttu-id="97dbf-112">值</span><span class="sxs-lookup"><span data-stu-id="97dbf-112">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="97dbf-113">Authorization</span><span class="sxs-lookup"><span data-stu-id="97dbf-113">Authorization</span></span>  | <span data-ttu-id="97dbf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="97dbf-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="97dbf-116">请求正文</span><span class="sxs-lookup"><span data-stu-id="97dbf-116">Request body</span></span>
<span data-ttu-id="97dbf-117">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="97dbf-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97dbf-118">响应</span><span class="sxs-lookup"><span data-stu-id="97dbf-118">Response</span></span>

<span data-ttu-id="97dbf-119">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="97dbf-119">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="97dbf-120">示例</span><span class="sxs-lookup"><span data-stu-id="97dbf-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="97dbf-121">请求</span><span class="sxs-lookup"><span data-stu-id="97dbf-121">Request</span></span>
<span data-ttu-id="97dbf-122">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="97dbf-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rejectedsenders"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders
```
##### <a name="response"></a><span data-ttu-id="97dbf-123">响应</span><span class="sxs-lookup"><span data-stu-id="97dbf-123">Response</span></span>
<span data-ttu-id="97dbf-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="97dbf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List rejectedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->