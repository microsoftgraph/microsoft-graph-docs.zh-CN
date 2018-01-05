# <a name="get-conversation-thread"></a><span data-ttu-id="95848-101">获取对话线程</span><span class="sxs-lookup"><span data-stu-id="95848-101">Get conversation thread</span></span>
<span data-ttu-id="95848-102">获取 [thread](../resources/conversationthread.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="95848-102">Get a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="95848-103">权限</span><span class="sxs-lookup"><span data-stu-id="95848-103">Permissions</span></span>
<span data-ttu-id="95848-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="95848-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="95848-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="95848-106">Permission type</span></span>      | <span data-ttu-id="95848-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="95848-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95848-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="95848-108">Delegated (work or school account)</span></span> | <span data-ttu-id="95848-109">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95848-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="95848-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="95848-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95848-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="95848-111">Not supported.</span></span>    |
|<span data-ttu-id="95848-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="95848-112">Application</span></span> | <span data-ttu-id="95848-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="95848-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="95848-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="95848-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="95848-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="95848-115">Optional query parameters</span></span>
<span data-ttu-id="95848-116">此方法支持 [OData 查询参数](../../../concepts/query_parameters.md) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="95848-116">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="95848-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="95848-117">Request headers</span></span>
| <span data-ttu-id="95848-118">标头</span><span class="sxs-lookup"><span data-stu-id="95848-118">Header</span></span>       | <span data-ttu-id="95848-119">值</span><span class="sxs-lookup"><span data-stu-id="95848-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="95848-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="95848-120">Authorization</span></span>  | <span data-ttu-id="95848-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="95848-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="95848-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="95848-123">Request body</span></span>
<span data-ttu-id="95848-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="95848-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95848-125">响应</span><span class="sxs-lookup"><span data-stu-id="95848-125">Response</span></span>
<span data-ttu-id="95848-126">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [thread](../resources/conversationthread.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="95848-126">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95848-127">示例</span><span class="sxs-lookup"><span data-stu-id="95848-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="95848-128">请求</span><span class="sxs-lookup"><span data-stu-id="95848-128">Request</span></span>
<span data-ttu-id="95848-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="95848-129">The following is an example of the request body.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_thread"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```

#### <a name="response"></a><span data-ttu-id="95848-130">响应</span><span class="sxs-lookup"><span data-stu-id="95848-130">Response</span></span>
<span data-ttu-id="95848-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="95848-131">Here is an example of the response.</span></span>
><span data-ttu-id="95848-132">**注意：**为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="95848-132">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="95848-133">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="95848-133">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 655

{
    "id": "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==",
    "topic": "New Training Plans",
    "hasAttachments": false,
    "lastDeliveredDateTime": "2017-07-31T18:59:05Z",
    "uniqueSenders": [
        "HR Taskforce"
    ],
    "preview": "Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
    "isLocked": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversation thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
