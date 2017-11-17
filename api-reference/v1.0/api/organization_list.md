# <a name="list-organization"></a><span data-ttu-id="92ccd-101">列出组织</span><span class="sxs-lookup"><span data-stu-id="92ccd-101">List organization</span></span>

<span data-ttu-id="92ccd-102">检索 organization 对象列表。</span><span class="sxs-lookup"><span data-stu-id="92ccd-102">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="92ccd-103">权限</span><span class="sxs-lookup"><span data-stu-id="92ccd-103">Permissions</span></span>
<span data-ttu-id="92ccd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="92ccd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="92ccd-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="92ccd-106">Permission type</span></span>      | <span data-ttu-id="92ccd-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="92ccd-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92ccd-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="92ccd-108">Delegated (work or school account)</span></span> | <span data-ttu-id="92ccd-109">不支持。</span><span class="sxs-lookup"><span data-stu-id="92ccd-109">Not supported.</span></span>    |
|<span data-ttu-id="92ccd-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="92ccd-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92ccd-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="92ccd-111">Not supported.</span></span>    |
|<span data-ttu-id="92ccd-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="92ccd-112">Application</span></span> | <span data-ttu-id="92ccd-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="92ccd-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="92ccd-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="92ccd-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="92ccd-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="92ccd-115">Optional query parameters</span></span>
<span data-ttu-id="92ccd-116">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="92ccd-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="92ccd-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="92ccd-117">Request headers</span></span>
| <span data-ttu-id="92ccd-118">名称</span><span class="sxs-lookup"><span data-stu-id="92ccd-118">Name</span></span>       | <span data-ttu-id="92ccd-119">类型</span><span class="sxs-lookup"><span data-stu-id="92ccd-119">Type</span></span> | <span data-ttu-id="92ccd-120">说明</span><span class="sxs-lookup"><span data-stu-id="92ccd-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="92ccd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="92ccd-121">Authorization</span></span>  | <span data-ttu-id="92ccd-122">string</span><span class="sxs-lookup"><span data-stu-id="92ccd-122">string</span></span>  | <span data-ttu-id="92ccd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="92ccd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="92ccd-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="92ccd-125">Request body</span></span>
<span data-ttu-id="92ccd-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="92ccd-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92ccd-127">响应</span><span class="sxs-lookup"><span data-stu-id="92ccd-127">Response</span></span>

<span data-ttu-id="92ccd-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [organization](../resources/organization.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="92ccd-128">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="92ccd-129">示例</span><span class="sxs-lookup"><span data-stu-id="92ccd-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="92ccd-130">请求</span><span class="sxs-lookup"><span data-stu-id="92ccd-130">Request</span></span>
<span data-ttu-id="92ccd-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="92ccd-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```http
GET https://graph.microsoft.com/v1.0/organization
```
##### <a name="response"></a><span data-ttu-id="92ccd-132">响应</span><span class="sxs-lookup"><span data-stu-id="92ccd-132">Response</span></span>
<span data-ttu-id="92ccd-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="92ccd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 500

{
  "value": [
    {
      "assignedPlans": [
        {
          "assignedDateTime": "datetime-value",
          "capabilityStatus": "capabilityStatus-value",
          "service": "service-value",
          "servicePlanId": "servicePlanId-value"
        }
      ],
      "businessPhones": [
        "businessPhones-value"
      ],
      "city": "city-value",
      "country": "country-value",
      "countryLetterCode": "countryLetterCode-value",
      "displayName": "displayName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->