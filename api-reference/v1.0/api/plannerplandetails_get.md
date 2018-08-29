# <a name="get-plannerplandetails"></a><span data-ttu-id="3b30f-101">获取 plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="3b30f-101">Get plannerPlanDetails</span></span>

<span data-ttu-id="3b30f-102">检索 **plannerplandetails** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3b30f-102">Retrieve the properties and relationships of **plannerplandetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3b30f-103">权限</span><span class="sxs-lookup"><span data-stu-id="3b30f-103">Permissions</span></span>
<span data-ttu-id="3b30f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="3b30f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3b30f-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="3b30f-106">Permission type</span></span>      | <span data-ttu-id="3b30f-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3b30f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b30f-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3b30f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="3b30f-109">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b30f-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3b30f-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3b30f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b30f-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="3b30f-111">Not supported.</span></span>    |
|<span data-ttu-id="3b30f-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="3b30f-112">Application</span></span> | <span data-ttu-id="3b30f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="3b30f-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b30f-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3b30f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/{id}/details
```

## <a name="request-headers"></a><span data-ttu-id="3b30f-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="3b30f-115">Request headers</span></span>
| <span data-ttu-id="3b30f-116">名称</span><span class="sxs-lookup"><span data-stu-id="3b30f-116">Name</span></span>      |<span data-ttu-id="3b30f-117">说明</span><span class="sxs-lookup"><span data-stu-id="3b30f-117">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3b30f-118">授权</span><span class="sxs-lookup"><span data-stu-id="3b30f-118">Authorization</span></span>  | <span data-ttu-id="3b30f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3b30f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3b30f-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="3b30f-121">Request body</span></span>
<span data-ttu-id="3b30f-122">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3b30f-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b30f-123">响应</span><span class="sxs-lookup"><span data-stu-id="3b30f-123">Response</span></span>

<span data-ttu-id="3b30f-124">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [plannerPlanDetails](../resources/plannerplandetails.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3b30f-124">If successful, this method returns a `200 OK` response code and [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.</span></span>

<span data-ttu-id="3b30f-p103">此方法可以返回任何 [HTTP 状态代码](../../../concepts/errors.md)。应用应当为此方法处理的最常见的错误为 403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner_overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="3b30f-p103">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="3b30f-128">示例</span><span class="sxs-lookup"><span data-stu-id="3b30f-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3b30f-129">请求</span><span class="sxs-lookup"><span data-stu-id="3b30f-129">Request</span></span>
<span data-ttu-id="3b30f-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3b30f-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerplandetails"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/plans/{plan-id}/details
```
##### <a name="response"></a><span data-ttu-id="3b30f-131">响应</span><span class="sxs-lookup"><span data-stu-id="3b30f-131">Response</span></span>
<span data-ttu-id="3b30f-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3b30f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlanDetails"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 373

{
  "sharedWith": {
    "aaa27244-1db4-476a-a5cb-004607466324" : true,
    "6463a5ce-2119-4198-9f2a-628761df4a62" : true
  },
  "categoryDescriptions": {
    "category1": "Indoors",
    "category2": "Outdoors",
    "category3": null,
    "category4": null,
    "category5": "Needs materials",
    "category6": "Needs equipment"
  },
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerPlanDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->