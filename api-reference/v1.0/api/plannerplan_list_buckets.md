# <a name="list-buckets"></a><span data-ttu-id="4cbca-101">列出存储桶</span><span class="sxs-lookup"><span data-stu-id="4cbca-101">List buckets</span></span>

<span data-ttu-id="4cbca-102">检索 [plannerPlan](../resources/plannerplan.md) 对象包含的 **plannerbucket** 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="4cbca-102">Retrieve a list of **plannerbucket** objects contained by a [plannerPlan](../resources/plannerplan.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4cbca-103">权限</span><span class="sxs-lookup"><span data-stu-id="4cbca-103">Permissions</span></span>
<span data-ttu-id="4cbca-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="4cbca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4cbca-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="4cbca-106">Permission type</span></span>      | <span data-ttu-id="4cbca-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4cbca-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4cbca-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4cbca-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4cbca-109">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cbca-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4cbca-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4cbca-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4cbca-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="4cbca-111">Not supported.</span></span>    |
|<span data-ttu-id="4cbca-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="4cbca-112">Application</span></span> | <span data-ttu-id="4cbca-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="4cbca-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4cbca-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4cbca-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/{id}/buckets
```

## <a name="request-headers"></a><span data-ttu-id="4cbca-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="4cbca-115">Request headers</span></span>
| <span data-ttu-id="4cbca-116">名称</span><span class="sxs-lookup"><span data-stu-id="4cbca-116">Name</span></span>      |<span data-ttu-id="4cbca-117">说明</span><span class="sxs-lookup"><span data-stu-id="4cbca-117">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4cbca-118">授权</span><span class="sxs-lookup"><span data-stu-id="4cbca-118">Authorization</span></span>  | <span data-ttu-id="4cbca-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4cbca-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4cbca-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="4cbca-121">Request body</span></span>
<span data-ttu-id="4cbca-122">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4cbca-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4cbca-123">响应</span><span class="sxs-lookup"><span data-stu-id="4cbca-123">Response</span></span>

<span data-ttu-id="4cbca-124">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [plannerBucket](../resources/plannerbucket.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="4cbca-124">If successful, this method returns a `200 OK` response code and collection of [plannerBucket](../resources/plannerbucket.md) objects in the response body.</span></span>

<span data-ttu-id="4cbca-p103">此方法可以返回任何 [HTTP 状态代码](../../../concepts/errors.md)。应用应当为此方法处理的最常见的错误为 403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner_overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="4cbca-p103">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="4cbca-128">示例</span><span class="sxs-lookup"><span data-stu-id="4cbca-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4cbca-129">请求</span><span class="sxs-lookup"><span data-stu-id="4cbca-129">Request</span></span>
<span data-ttu-id="4cbca-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4cbca-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_buckets"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/plans/{plan-id}/buckets
```
##### <a name="response"></a><span data-ttu-id="4cbca-131">响应</span><span class="sxs-lookup"><span data-stu-id="4cbca-131">Response</span></span>
<span data-ttu-id="4cbca-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4cbca-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "value": [
    {
      "@odata.etag": "W/\"JzEtQnVja2V0QEBAQEBAQEBAQEBAQEBARCc=\"",
      "name": "To do",
      "planId": "2txjA-BMZEq-bKi6Wfj5aGQAB1OJ",
      "orderHint": "85752723360752+",
      "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
    }
  ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List buckets",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->