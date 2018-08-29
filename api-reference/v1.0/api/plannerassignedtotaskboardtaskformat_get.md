# <a name="get-plannerassignedtotaskboardtaskformat"></a><span data-ttu-id="ef5db-101">获取 plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="ef5db-101">Get plannerAssignedToTaskBoardTaskFormat</span></span>

<span data-ttu-id="ef5db-102">检索 **plannerAssignedToTaskBoardTaskFormat** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ef5db-102">Retrieve the properties and relationships of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ef5db-103">权限</span><span class="sxs-lookup"><span data-stu-id="ef5db-103">Permissions</span></span>
<span data-ttu-id="ef5db-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ef5db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ef5db-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="ef5db-106">Permission type</span></span>      | <span data-ttu-id="ef5db-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ef5db-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef5db-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ef5db-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ef5db-109">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef5db-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ef5db-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ef5db-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef5db-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="ef5db-111">Not supported.</span></span>    |
|<span data-ttu-id="ef5db-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="ef5db-112">Application</span></span> | <span data-ttu-id="ef5db-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ef5db-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef5db-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ef5db-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}/assignedToTaskBoardFormat
```
## <a name="request-headers"></a><span data-ttu-id="ef5db-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="ef5db-115">Request headers</span></span>
| <span data-ttu-id="ef5db-116">名称</span><span class="sxs-lookup"><span data-stu-id="ef5db-116">Name</span></span>      |<span data-ttu-id="ef5db-117">说明</span><span class="sxs-lookup"><span data-stu-id="ef5db-117">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ef5db-118">授权</span><span class="sxs-lookup"><span data-stu-id="ef5db-118">Authorization</span></span>  | <span data-ttu-id="ef5db-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ef5db-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ef5db-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="ef5db-121">Request body</span></span>
<span data-ttu-id="ef5db-122">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ef5db-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef5db-123">响应</span><span class="sxs-lookup"><span data-stu-id="ef5db-123">Response</span></span>

<span data-ttu-id="ef5db-124">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ef5db-124">If successful, this method returns a `200 OK` response code and [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="ef5db-p103">此方法可以返回任何 [HTTP 状态代码](../../../concepts/errors.md)。应用应当为此方法处理的最常见的错误为 403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner_overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="ef5db-p103">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="ef5db-128">示例</span><span class="sxs-lookup"><span data-stu-id="ef5db-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ef5db-129">请求</span><span class="sxs-lookup"><span data-stu-id="ef5db-129">Request</span></span>
<span data-ttu-id="ef5db-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ef5db-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerassignedtotaskboardtaskformat"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/assignedToTaskBoardFormat
```
##### <a name="response"></a><span data-ttu-id="ef5db-131">响应</span><span class="sxs-lookup"><span data-stu-id="ef5db-131">Response</span></span>
<span data-ttu-id="ef5db-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ef5db-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 225

{
  "unassignedOrderHint": "RWk1",
  "orderHintsByAssignee": {
    "6463a5ce-2119-4198-9f2a-628761df4a62":"85752723360752+",
    "aaa27244-1db4-476a-a5cb-004607466324":"90057581;"
  },
  "id": "01gzSlKkIUSUl6DF_EilrmQAKDhh"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerAssignedToTaskBoardTaskFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->