# <a name="list-rejectedsenders"></a><span data-ttu-id="a57ec-101">列出 rejectedSender</span><span class="sxs-lookup"><span data-stu-id="a57ec-101">List rejectedSenders</span></span>
<span data-ttu-id="a57ec-102">获取此组 rejectedSenders 列表中的用户或组列表。</span><span class="sxs-lookup"><span data-stu-id="a57ec-102">Get a list of users or groups that are in the rejectedSenders list for this group.</span></span> 

<span data-ttu-id="a57ec-p101">已拒绝的发件人列表中的用户无法发布到组对话（在 GET 请求 URL 中标识）。确保未在拒绝的发件人和接受的发件人列表中指定同一用户或组，否则会发生错误。</span><span class="sxs-lookup"><span data-stu-id="a57ec-p101">Users in the rejected senders list cannot post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="a57ec-105">权限</span><span class="sxs-lookup"><span data-stu-id="a57ec-105">Permissions</span></span>
<span data-ttu-id="a57ec-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a57ec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a57ec-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a57ec-108">Permission type</span></span>      | <span data-ttu-id="a57ec-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a57ec-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a57ec-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a57ec-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a57ec-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a57ec-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a57ec-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a57ec-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a57ec-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a57ec-113">Not supported.</span></span>    |
|<span data-ttu-id="a57ec-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a57ec-114">Application</span></span> | <span data-ttu-id="a57ec-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a57ec-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a57ec-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a57ec-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/rejectedSenders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a57ec-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a57ec-117">Optional query parameters</span></span>
<span data-ttu-id="a57ec-118">此方法支持 [OData 查询参数](../../../concepts/query_parameters.md) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a57ec-118">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a57ec-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a57ec-119">Request headers</span></span>
| <span data-ttu-id="a57ec-120">标头</span><span class="sxs-lookup"><span data-stu-id="a57ec-120">Header</span></span>       | <span data-ttu-id="a57ec-121">值</span><span class="sxs-lookup"><span data-stu-id="a57ec-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a57ec-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a57ec-122">Authorization</span></span>  | <span data-ttu-id="a57ec-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a57ec-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a57ec-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a57ec-125">Request body</span></span>
<span data-ttu-id="a57ec-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a57ec-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a57ec-127">响应</span><span class="sxs-lookup"><span data-stu-id="a57ec-127">Response</span></span>
<span data-ttu-id="a57ec-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a57ec-128">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a57ec-129">示例</span><span class="sxs-lookup"><span data-stu-id="a57ec-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a57ec-130">请求</span><span class="sxs-lookup"><span data-stu-id="a57ec-130">Request</span></span>
<span data-ttu-id="a57ec-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a57ec-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rejectedsenders"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders
```

#### <a name="response"></a><span data-ttu-id="a57ec-132">响应</span><span class="sxs-lookup"><span data-stu-id="a57ec-132">Response</span></span>
<span data-ttu-id="a57ec-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a57ec-133">The following is an example of the response.</span></span>
><span data-ttu-id="a57ec-134">**注意：**为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a57ec-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a57ec-135">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a57ec-135">All the properties will be returned from an actual call.</span></span>
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