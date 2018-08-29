# <a name="get-conversation"></a><span data-ttu-id="13b16-101">获取对话</span><span class="sxs-lookup"><span data-stu-id="13b16-101">Get conversation</span></span>
<span data-ttu-id="13b16-102">获取 [conversation](../resources/conversation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="13b16-102">Get a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="13b16-103">权限</span><span class="sxs-lookup"><span data-stu-id="13b16-103">Permissions</span></span>
<span data-ttu-id="13b16-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="13b16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="13b16-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="13b16-106">Permission type</span></span>      | <span data-ttu-id="13b16-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="13b16-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13b16-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="13b16-108">Delegated (work or school account)</span></span> | <span data-ttu-id="13b16-109">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13b16-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="13b16-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="13b16-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13b16-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="13b16-111">Not supported.</span></span>    |
|<span data-ttu-id="13b16-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="13b16-112">Application</span></span> | <span data-ttu-id="13b16-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="13b16-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="13b16-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="13b16-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="13b16-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="13b16-115">Optional query parameters</span></span>
<span data-ttu-id="13b16-116">此方法支持 [OData 查询参数](../../../concepts/query_parameters.md) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="13b16-116">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="13b16-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="13b16-117">Request headers</span></span>
| <span data-ttu-id="13b16-118">标头</span><span class="sxs-lookup"><span data-stu-id="13b16-118">Header</span></span>       | <span data-ttu-id="13b16-119">值</span><span class="sxs-lookup"><span data-stu-id="13b16-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="13b16-120">授权</span><span class="sxs-lookup"><span data-stu-id="13b16-120">Authorization</span></span>  | <span data-ttu-id="13b16-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="13b16-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="13b16-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="13b16-123">Request body</span></span>
<span data-ttu-id="13b16-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="13b16-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13b16-125">响应</span><span class="sxs-lookup"><span data-stu-id="13b16-125">Response</span></span>
<span data-ttu-id="13b16-126">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversation](../resources/conversation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="13b16-126">If successful, this method returns a `200 OK` response code and a [conversation](../resources/conversation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13b16-127">示例</span><span class="sxs-lookup"><span data-stu-id="13b16-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="13b16-128">请求</span><span class="sxs-lookup"><span data-stu-id="13b16-128">Request</span></span>
<span data-ttu-id="13b16-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="13b16-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU="],
  "name": "get_group_conversation"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```

#### <a name="response"></a><span data-ttu-id="13b16-130">响应</span><span class="sxs-lookup"><span data-stu-id="13b16-130">Response</span></span>
<span data-ttu-id="13b16-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="13b16-131">The following is an example of the response.</span></span>
><span data-ttu-id="13b16-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="13b16-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 644

{
    "id": "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=",
    "topic": "New Training Plans",
    "hasAttachments": false,
    "lastDeliveredDateTime": "2017-07-31T18:59:05Z",
    "uniqueSenders": [
        "HR Taskforce"
    ],
    "preview": "Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
