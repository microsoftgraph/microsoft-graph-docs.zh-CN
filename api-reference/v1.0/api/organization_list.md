# <a name="list-organization"></a><span data-ttu-id="f8c76-101">列出组织</span><span class="sxs-lookup"><span data-stu-id="f8c76-101">List organization</span></span>



<span data-ttu-id="f8c76-102">检索 organization 对象列表。</span><span class="sxs-lookup"><span data-stu-id="f8c76-102">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="f8c76-103">权限</span><span class="sxs-lookup"><span data-stu-id="f8c76-103">Permissions</span></span>
<span data-ttu-id="f8c76-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f8c76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f8c76-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8c76-106">Permission type</span></span>      | <span data-ttu-id="f8c76-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f8c76-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8c76-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8c76-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f8c76-109">User.Read、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8c76-109">User.Read, Directory.Read.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="f8c76-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8c76-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8c76-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8c76-111">Not supported.</span></span>    |
|<span data-ttu-id="f8c76-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="f8c76-112">Application</span></span> | <span data-ttu-id="f8c76-113">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8c76-113">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="f8c76-114">注意：授予 User.Read 权限的应用程序仅能读取组织的 *id*、*displayName* 和 *verifiedDomains* 属性。</span><span class="sxs-lookup"><span data-stu-id="f8c76-114">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="f8c76-115">所有其他属性将返回 `null` 值。</span><span class="sxs-lookup"><span data-stu-id="f8c76-115">All other properties will return with `null` values.</span></span> <span data-ttu-id="f8c76-116">若要读取所有属性，请使用 Directory.Read.All。</span><span class="sxs-lookup"><span data-stu-id="f8c76-116">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="f8c76-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8c76-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f8c76-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f8c76-118">Optional query parameters</span></span>
<span data-ttu-id="f8c76-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f8c76-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f8c76-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8c76-120">Request headers</span></span>
| <span data-ttu-id="f8c76-121">名称</span><span class="sxs-lookup"><span data-stu-id="f8c76-121">Name</span></span>       | <span data-ttu-id="f8c76-122">类型</span><span class="sxs-lookup"><span data-stu-id="f8c76-122">Type</span></span> | <span data-ttu-id="f8c76-123">说明</span><span class="sxs-lookup"><span data-stu-id="f8c76-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f8c76-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8c76-124">Authorization</span></span>  | <span data-ttu-id="f8c76-125">string</span><span class="sxs-lookup"><span data-stu-id="f8c76-125">string</span></span>  | <span data-ttu-id="f8c76-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f8c76-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8c76-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f8c76-128">Request body</span></span>
<span data-ttu-id="f8c76-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f8c76-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8c76-130">响应</span><span class="sxs-lookup"><span data-stu-id="f8c76-130">Response</span></span>

<span data-ttu-id="f8c76-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [organization](../resources/organization.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f8c76-131">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f8c76-132">示例</span><span class="sxs-lookup"><span data-stu-id="f8c76-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f8c76-133">请求</span><span class="sxs-lookup"><span data-stu-id="f8c76-133">Request</span></span>
<span data-ttu-id="f8c76-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f8c76-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```http
GET https://graph.microsoft.com/beta/organization
```
##### <a name="response"></a><span data-ttu-id="f8c76-135">响应</span><span class="sxs-lookup"><span data-stu-id="f8c76-135">Response</span></span>
<span data-ttu-id="f8c76-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f8c76-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
          "assignedDateTime": "2016-10-19T10:37:00Z",
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