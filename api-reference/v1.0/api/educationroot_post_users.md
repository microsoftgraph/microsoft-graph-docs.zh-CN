# <a name="create-educationuser"></a><span data-ttu-id="b9fde-101">创建 educationUser</span><span class="sxs-lookup"><span data-stu-id="b9fde-101">Create educationUser</span></span>

<span data-ttu-id="b9fde-102">新建用户。</span><span class="sxs-lookup"><span data-stu-id="b9fde-102">Create a new user.</span></span>

<!-- Add some additional text to better distinguish this method from the user_post_users (https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_post_users) topic. -->

## <a name="permissions"></a><span data-ttu-id="b9fde-103">权限</span><span class="sxs-lookup"><span data-stu-id="b9fde-103">Permissions</span></span>
<span data-ttu-id="b9fde-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b9fde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b9fde-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9fde-106">Permission type</span></span>      | <span data-ttu-id="b9fde-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b9fde-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9fde-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9fde-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="b9fde-109">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9fde-109">Not supported.</span></span>  |
|<span data-ttu-id="b9fde-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9fde-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b9fde-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9fde-111">Not supported.</span></span>  |
|<span data-ttu-id="b9fde-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9fde-112">Application</span></span> | <span data-ttu-id="b9fde-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9fde-113">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b9fde-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9fde-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/users
```
## <a name="request-headers"></a><span data-ttu-id="b9fde-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="b9fde-115">Request headers</span></span>
| <span data-ttu-id="b9fde-116">标头</span><span class="sxs-lookup"><span data-stu-id="b9fde-116">Header</span></span>       | <span data-ttu-id="b9fde-117">值</span><span class="sxs-lookup"><span data-stu-id="b9fde-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b9fde-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9fde-118">Authorization</span></span>  | <span data-ttu-id="b9fde-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b9fde-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b9fde-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b9fde-121">Content-Type</span></span>  | <span data-ttu-id="b9fde-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b9fde-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b9fde-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9fde-123">Request body</span></span>
<span data-ttu-id="b9fde-124">在请求正文中，提供 [educationUser](../resources/educationuser.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b9fde-124">In the request body, supply a JSON representation of an [invitation](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="b9fde-125">响应</span><span class="sxs-lookup"><span data-stu-id="b9fde-125">Response</span></span>
<span data-ttu-id="b9fde-126">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [educationUser](../resources/educationuser.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b9fde-126">If successful, this method returns a `201 Created` response code and an [event](../resources/educationuser.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9fde-127">示例</span><span class="sxs-lookup"><span data-stu-id="b9fde-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b9fde-128">请求</span><span class="sxs-lookup"><span data-stu-id="b9fde-128">Request</span></span>
<span data-ttu-id="b9fde-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b9fde-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/users
Content-type: application/json
Content-length: 508

{
  "displayName": "Dion Matheson",
  "givenName": "Dion",
  "middleName": null,
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
  }
}
```

##### <a name="response"></a><span data-ttu-id="b9fde-130">响应</span><span class="sxs-lookup"><span data-stu-id="b9fde-130">Response</span></span>
<span data-ttu-id="b9fde-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b9fde-131">The following is an example of the response.</span></span> 

><span data-ttu-id="b9fde-p103">**注意：**为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b9fde-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 201 Created
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
      "id": "14012",
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
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->