# <a name="list-threads"></a><span data-ttu-id="db969-101">列出线程</span><span class="sxs-lookup"><span data-stu-id="db969-101">List threads</span></span>

<span data-ttu-id="db969-102">获取组对话中的所有线程。</span><span class="sxs-lookup"><span data-stu-id="db969-102">Get all the threads in a group conversation.</span></span>

<span data-ttu-id="db969-103">注意：还可以 [获取组的所有线程](group_list_threads.md)。</span><span class="sxs-lookup"><span data-stu-id="db969-103">Note: You can also [get all the threads of a group](group_list_threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="db969-104">权限</span><span class="sxs-lookup"><span data-stu-id="db969-104">Permissions</span></span>
<span data-ttu-id="db969-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="db969-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="db969-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="db969-107">Permission type</span></span>      | <span data-ttu-id="db969-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="db969-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db969-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db969-109">Delegated (work or school account)</span></span> | <span data-ttu-id="db969-110">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="db969-110">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="db969-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db969-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db969-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="db969-112">Not supported.</span></span>    |
|<span data-ttu-id="db969-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="db969-113">Application</span></span> | <span data-ttu-id="db969-114">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="db969-114">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db969-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db969-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}/threads
```
## <a name="optional-query-parameters"></a><span data-ttu-id="db969-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="db969-116">Optional query parameters</span></span>
<span data-ttu-id="db969-117">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="db969-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="db969-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="db969-118">Request headers</span></span>
| <span data-ttu-id="db969-119">标头</span><span class="sxs-lookup"><span data-stu-id="db969-119">Header</span></span>       | <span data-ttu-id="db969-120">值</span><span class="sxs-lookup"><span data-stu-id="db969-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="db969-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="db969-121">Authorization</span></span>  | <span data-ttu-id="db969-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="db969-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="db969-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="db969-124">Request body</span></span>
<span data-ttu-id="db969-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="db969-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db969-126">响应</span><span class="sxs-lookup"><span data-stu-id="db969-126">Response</span></span>

<span data-ttu-id="db969-127">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationThread](../resources/conversationthread.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="db969-127">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="db969-128">示例</span><span class="sxs-lookup"><span data-stu-id="db969-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db969-129">请求</span><span class="sxs-lookup"><span data-stu-id="db969-129">Request</span></span>
<span data-ttu-id="db969-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="db969-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}/threads
```
##### <a name="response"></a><span data-ttu-id="db969-131">响应</span><span class="sxs-lookup"><span data-stu-id="db969-131">Response</span></span>
<span data-ttu-id="db969-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="db969-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 536

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
