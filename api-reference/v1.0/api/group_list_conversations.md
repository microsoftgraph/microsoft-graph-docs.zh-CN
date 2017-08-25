# <a name="list-conversations"></a><span data-ttu-id="ae85d-101">列出对话</span><span class="sxs-lookup"><span data-stu-id="ae85d-101">List conversations</span></span>

<span data-ttu-id="ae85d-102">检索此组中的会话列表。</span><span class="sxs-lookup"><span data-stu-id="ae85d-102">Retrieve the list of conversations in this group.</span></span>
## <a name="permissions"></a><span data-ttu-id="ae85d-103">权限</span><span class="sxs-lookup"><span data-stu-id="ae85d-103">Permissions</span></span>
<span data-ttu-id="ae85d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ae85d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ae85d-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="ae85d-106">Permission type</span></span>      | <span data-ttu-id="ae85d-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ae85d-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="ae85d-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ae85d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ae85d-109">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae85d-109">Group.Read.All, Group.ReadWrite.All</span></span>    | 
|<span data-ttu-id="ae85d-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ae85d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae85d-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="ae85d-111">Not supported.</span></span>    | 
|<span data-ttu-id="ae85d-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="ae85d-112">Application</span></span> | <span data-ttu-id="ae85d-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae85d-113">Group.Read.All, Group.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ae85d-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ae85d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ae85d-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ae85d-115">Optional query parameters</span></span>
<span data-ttu-id="ae85d-116">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ae85d-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ae85d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="ae85d-117">Request headers</span></span>
| <span data-ttu-id="ae85d-118">标头</span><span class="sxs-lookup"><span data-stu-id="ae85d-118">Header</span></span>       | <span data-ttu-id="ae85d-119">值</span><span class="sxs-lookup"><span data-stu-id="ae85d-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ae85d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae85d-120">Authorization</span></span>  | <span data-ttu-id="ae85d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ae85d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ae85d-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="ae85d-123">Request body</span></span>
<span data-ttu-id="ae85d-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ae85d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae85d-125">响应</span><span class="sxs-lookup"><span data-stu-id="ae85d-125">Response</span></span>

<span data-ttu-id="ae85d-126">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Conversation](../resources/conversation.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ae85d-126">If successful, this method returns a `200 OK` response code and collection of [Conversation](../resources/conversation.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ae85d-127">示例</span><span class="sxs-lookup"><span data-stu-id="ae85d-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ae85d-128">请求</span><span class="sxs-lookup"><span data-stu-id="ae85d-128">Request</span></span>
<span data-ttu-id="ae85d-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ae85d-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversations"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations
```
##### <a name="response"></a><span data-ttu-id="ae85d-130">响应</span><span class="sxs-lookup"><span data-stu-id="ae85d-130">Response</span></span>
<span data-ttu-id="ae85d-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ae85d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "topic": "topic-value",
      "hasAttachments": true,
      "lastDeliveredDateTime": "datetime-value",
      "uniqueSenders": [
        "uniqueSenders-value"
      ],
      "preview": "preview-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List conversations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->