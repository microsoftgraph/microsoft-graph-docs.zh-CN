# <a name="get-eventmessage"></a><span data-ttu-id="be455-101">获取 eventMessage</span><span class="sxs-lookup"><span data-stu-id="be455-101">Get eventMessage</span></span>

<span data-ttu-id="be455-102">检索 [eventMessage](../resources/eventmessage.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="be455-102">Retrieve the properties and relationships of [eventMessage](../resources/eventmessage.md) object.</span></span>

<span data-ttu-id="be455-103">目前，此操作返回纯 HTML 格式的事件消息正文。</span><span class="sxs-lookup"><span data-stu-id="be455-103">Currently, this operation returns event message bodies in only HTML format.</span></span>

## <a name="permissions"></a><span data-ttu-id="be455-104">权限</span><span class="sxs-lookup"><span data-stu-id="be455-104">Permissions</span></span>
<span data-ttu-id="be455-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="be455-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="be455-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="be455-107">Permission type</span></span>      | <span data-ttu-id="be455-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="be455-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be455-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="be455-109">Delegated (work or school account)</span></span> | <span data-ttu-id="be455-110">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="be455-110">Mail.Read</span></span>    |
|<span data-ttu-id="be455-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="be455-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be455-112">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="be455-112">Mail.Read</span></span>    |
|<span data-ttu-id="be455-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="be455-113">Application</span></span> | <span data-ttu-id="be455-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="be455-114">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="be455-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="be455-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}

GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="be455-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="be455-116">Optional query parameters</span></span>
<span data-ttu-id="be455-117">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="be455-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="be455-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="be455-118">Request headers</span></span>
| <span data-ttu-id="be455-119">名称</span><span class="sxs-lookup"><span data-stu-id="be455-119">Name</span></span>       | <span data-ttu-id="be455-120">类型</span><span class="sxs-lookup"><span data-stu-id="be455-120">Type</span></span> | <span data-ttu-id="be455-121">说明</span><span class="sxs-lookup"><span data-stu-id="be455-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="be455-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="be455-122">Authorization</span></span>  | <span data-ttu-id="be455-123">string</span><span class="sxs-lookup"><span data-stu-id="be455-123">string</span></span>  | <span data-ttu-id="be455-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="be455-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be455-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="be455-126">Request body</span></span>
<span data-ttu-id="be455-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="be455-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be455-128">响应</span><span class="sxs-lookup"><span data-stu-id="be455-128">Response</span></span>

<span data-ttu-id="be455-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [eventMessage](../resources/eventmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="be455-129">If successful, this method returns a `200 OK` response code and [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="be455-130">示例</span><span class="sxs-lookup"><span data-stu-id="be455-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="be455-131">请求</span><span class="sxs-lookup"><span data-stu-id="be455-131">Request</span></span>
<span data-ttu-id="be455-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="be455-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_eventmessage"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="be455-133">响应</span><span class="sxs-lookup"><span data-stu-id="be455-133">Response</span></span>
<span data-ttu-id="be455-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="be455-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventmessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "html",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value",
  "meetingMessageType": "meetingMessageType-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get eventMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
