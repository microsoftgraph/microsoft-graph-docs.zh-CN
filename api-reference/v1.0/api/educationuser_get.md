# <a name="get-educationuser"></a><span data-ttu-id="bc525-101">获取 educationUser</span><span class="sxs-lookup"><span data-stu-id="bc525-101">Get educationUser</span></span>

<span data-ttu-id="bc525-102">检索用户的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bc525-102">Retrieve the properties and relationships of user object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc525-103">权限</span><span class="sxs-lookup"><span data-stu-id="bc525-103">Permissions</span></span>
<span data-ttu-id="bc525-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="bc525-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bc525-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="bc525-106">Permission type</span></span>      | <span data-ttu-id="bc525-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bc525-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc525-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bc525-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="bc525-109">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="bc525-109">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="bc525-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bc525-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="bc525-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc525-111">Not supported.</span></span>  |
|<span data-ttu-id="bc525-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="bc525-112">Application</span></span> | <span data-ttu-id="bc525-113">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc525-113">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 
## <a name="http-request"></a><span data-ttu-id="bc525-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bc525-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me
GET /education/users/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bc525-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bc525-115">Optional query parameters</span></span>
<span data-ttu-id="bc525-116">此方法支持 [OData 查询参数](http://graph.microsoft.io/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bc525-116">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bc525-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="bc525-117">Request headers</span></span>
| <span data-ttu-id="bc525-118">标头</span><span class="sxs-lookup"><span data-stu-id="bc525-118">Header</span></span>       | <span data-ttu-id="bc525-119">值</span><span class="sxs-lookup"><span data-stu-id="bc525-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bc525-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc525-120">Authorization</span></span>  | <span data-ttu-id="bc525-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bc525-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bc525-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="bc525-123">Request body</span></span>
<span data-ttu-id="bc525-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bc525-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="bc525-125">响应</span><span class="sxs-lookup"><span data-stu-id="bc525-125">Response</span></span>
<span data-ttu-id="bc525-126">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationUser](../resources/educationuser.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bc525-126">If successful, this method returns a `200 OK` response code and an [event](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bc525-127">示例</span><span class="sxs-lookup"><span data-stu-id="bc525-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc525-128">请求</span><span class="sxs-lookup"><span data-stu-id="bc525-128">Request</span></span>
<span data-ttu-id="bc525-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bc525-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationuser"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/users/13012
```
##### <a name="response"></a><span data-ttu-id="bc525-130">响应</span><span class="sxs-lookup"><span data-stu-id="bc525-130">Response</span></span>
<span data-ttu-id="bc525-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bc525-131">The following is an example of the response.</span></span> 

><span data-ttu-id="bc525-p103">**注意：**为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bc525-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 508

{
  "id": "13012",
  "displayName": "Dion Matheson",
  "givenName": "Dion",
  "middleName": " ",
  "surname": "Matheson",
  "mail": "DionM@contoso.com",
  "mobilePhone": "+1 (253) 555-0101",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012"
    }
  },
  "externalSource": "sis",
  "mailingAddress": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  },
  "primaryRole": "student",
  "residenceAddress": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  },
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->