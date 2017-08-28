# <a name="list-acceptedsenders"></a><span data-ttu-id="50a88-101">列出 acceptedSender</span><span class="sxs-lookup"><span data-stu-id="50a88-101">List acceptedSenders</span></span>

<span data-ttu-id="50a88-102">获取此组 acceptedSenders 列表中的用户或组列表。</span><span class="sxs-lookup"><span data-stu-id="50a88-102">Get a list of users or groups that are in the acceptedSenders list for this group.</span></span>

<span data-ttu-id="50a88-p101">接受的发件人列表中的用户可以发布到组对话（在 GET 请求 URL 中标识）。确保未在接受的发件人和拒绝的发件人列表中指定同一用户或组，否则会发生错误。</span><span class="sxs-lookup"><span data-stu-id="50a88-p101">Users in the accepted senders list can post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>
## <a name="permissions"></a><span data-ttu-id="50a88-105">权限</span><span class="sxs-lookup"><span data-stu-id="50a88-105">Permissions</span></span>
<span data-ttu-id="50a88-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="50a88-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="50a88-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="50a88-108">Permission type</span></span>      | <span data-ttu-id="50a88-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="50a88-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50a88-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="50a88-110">Delegated (work or school account)</span></span> | <span data-ttu-id="50a88-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50a88-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="50a88-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="50a88-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50a88-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="50a88-113">Not supported.</span></span>    |
|<span data-ttu-id="50a88-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="50a88-114">Application</span></span> | <span data-ttu-id="50a88-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50a88-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="50a88-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="50a88-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/acceptedSenders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="50a88-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="50a88-117">Optional query parameters</span></span>
<span data-ttu-id="50a88-118">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="50a88-118">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="50a88-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="50a88-119">Request headers</span></span>
| <span data-ttu-id="50a88-120">标头</span><span class="sxs-lookup"><span data-stu-id="50a88-120">Header</span></span>       | <span data-ttu-id="50a88-121">值</span><span class="sxs-lookup"><span data-stu-id="50a88-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="50a88-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="50a88-122">Authorization</span></span>  | <span data-ttu-id="50a88-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="50a88-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="50a88-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="50a88-125">Request body</span></span>
<span data-ttu-id="50a88-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="50a88-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50a88-127">响应</span><span class="sxs-lookup"><span data-stu-id="50a88-127">Response</span></span>

<span data-ttu-id="50a88-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="50a88-128">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="50a88-129">示例</span><span class="sxs-lookup"><span data-stu-id="50a88-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="50a88-130">请求</span><span class="sxs-lookup"><span data-stu-id="50a88-130">Request</span></span>
<span data-ttu-id="50a88-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="50a88-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_acceptedsenders"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/acceptedSenders
```
##### <a name="response"></a><span data-ttu-id="50a88-132">响应</span><span class="sxs-lookup"><span data-stu-id="50a88-132">Response</span></span>
<span data-ttu-id="50a88-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="50a88-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List acceptedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->