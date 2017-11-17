# <a name="get-domain"></a><span data-ttu-id="25912-101">获取 domain</span><span class="sxs-lookup"><span data-stu-id="25912-101">Get domain</span></span>

<span data-ttu-id="25912-102">检索 domain 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="25912-102">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="25912-103">权限</span><span class="sxs-lookup"><span data-stu-id="25912-103">Permissions</span></span>

<span data-ttu-id="25912-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="25912-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="25912-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="25912-106">Permission type</span></span>      | <span data-ttu-id="25912-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="25912-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25912-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="25912-108">Delegated (work or school account)</span></span> | <span data-ttu-id="25912-109">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="25912-109">Directory.Read.All</span></span>    |
|<span data-ttu-id="25912-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="25912-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25912-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="25912-111">Not supported.</span></span>    |
|<span data-ttu-id="25912-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="25912-112">Application</span></span> | <span data-ttu-id="25912-113">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25912-113">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="25912-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="25912-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="25912-115">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="25912-115">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="25912-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="25912-116">Optional query parameters</span></span>

<span data-ttu-id="25912-117">此方法支持 [OData 查询参数](http://graph.microsoft.io/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="25912-117">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="25912-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="25912-118">Request headers</span></span>

| <span data-ttu-id="25912-119">名称</span><span class="sxs-lookup"><span data-stu-id="25912-119">Name</span></span>      |<span data-ttu-id="25912-120">说明</span><span class="sxs-lookup"><span data-stu-id="25912-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="25912-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="25912-121">Authorization</span></span>  | <span data-ttu-id="25912-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="25912-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="25912-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="25912-124">Content-Type</span></span>  | <span data-ttu-id="25912-125">application/json</span><span class="sxs-lookup"><span data-stu-id="25912-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="25912-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="25912-126">Request body</span></span>
<span data-ttu-id="25912-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="25912-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25912-128">响应</span><span class="sxs-lookup"><span data-stu-id="25912-128">Response</span></span>

<span data-ttu-id="25912-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [domain](../resources/domain.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="25912-129">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="25912-130">示例</span><span class="sxs-lookup"><span data-stu-id="25912-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="25912-131">请求</span><span class="sxs-lookup"><span data-stu-id="25912-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domain"
}-->
```http
GET https://graph.microsoft.com/V1.0/domains/contoso.com
```
##### <a name="response"></a><span data-ttu-id="25912-132">响应</span><span class="sxs-lookup"><span data-stu-id="25912-132">Response</span></span>
<span data-ttu-id="25912-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="25912-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "id": "contoso.com",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->