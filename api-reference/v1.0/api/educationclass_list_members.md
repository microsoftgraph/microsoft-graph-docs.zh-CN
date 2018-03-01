# <a name="list-members"></a><span data-ttu-id="61cdb-101">列出成员</span><span class="sxs-lookup"><span data-stu-id="61cdb-101">List members</span></span>

<span data-ttu-id="61cdb-102">检索参加课程的教师和学生。</span><span class="sxs-lookup"><span data-stu-id="61cdb-102">Retrieves the teachers and students for a class.</span></span> <span data-ttu-id="61cdb-103">请注意是否使用了委派令牌，只有课程的其他成员才能看到成员。</span><span class="sxs-lookup"><span data-stu-id="61cdb-103">Note that if the delegated token is used, members can only be seen by other members of the class.</span></span>

## <a name="permissions"></a><span data-ttu-id="61cdb-104">权限</span><span class="sxs-lookup"><span data-stu-id="61cdb-104">Permissions</span></span>
<span data-ttu-id="61cdb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="61cdb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="61cdb-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="61cdb-107">Permission type</span></span>      | <span data-ttu-id="61cdb-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="61cdb-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61cdb-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="61cdb-109">Delegated (work or school account)</span></span> |  <span data-ttu-id="61cdb-110">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="61cdb-110">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="61cdb-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="61cdb-111">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="61cdb-112">不支持</span><span class="sxs-lookup"><span data-stu-id="61cdb-112">Not supported</span></span>  |
|<span data-ttu-id="61cdb-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="61cdb-113">Application</span></span> | <span data-ttu-id="61cdb-114">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61cdb-114">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="61cdb-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="61cdb-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="61cdb-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="61cdb-116">Optional query parameters</span></span>
<span data-ttu-id="61cdb-117">此方法支持 [OData 查询参数](http://graph.microsoft.io/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="61cdb-117">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="61cdb-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="61cdb-118">Request headers</span></span>
| <span data-ttu-id="61cdb-119">标头</span><span class="sxs-lookup"><span data-stu-id="61cdb-119">Header</span></span>       | <span data-ttu-id="61cdb-120">值</span><span class="sxs-lookup"><span data-stu-id="61cdb-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="61cdb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="61cdb-121">Authorization</span></span>  | <span data-ttu-id="61cdb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="61cdb-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="61cdb-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="61cdb-124">Request body</span></span>
<span data-ttu-id="61cdb-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="61cdb-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="61cdb-126">响应</span><span class="sxs-lookup"><span data-stu-id="61cdb-126">Response</span></span>
<span data-ttu-id="61cdb-127">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationUser](../resources/educationuser.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="61cdb-127">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="61cdb-128">示例</span><span class="sxs-lookup"><span data-stu-id="61cdb-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="61cdb-129">请求</span><span class="sxs-lookup"><span data-stu-id="61cdb-129">Request</span></span>
<span data-ttu-id="61cdb-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="61cdb-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/11016/members
```
##### <a name="response"></a><span data-ttu-id="61cdb-131">响应</span><span class="sxs-lookup"><span data-stu-id="61cdb-131">Response</span></span>
<span data-ttu-id="61cdb-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="61cdb-132">The following is an example of the response.</span></span> 

><span data-ttu-id="61cdb-p104">**注意：**为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="61cdb-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 593

{
  "value": [
    {
      "id": "13013",
      "displayName": "Ora Klein",
      "givenName": "Ora",
      "middleName": " ",
      "surname": "Klein",
      "mail": "OraK@contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "School of Fine Art",
      "mailingAddress": {
        "city": "Buffalo",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "NY",
        "street": "12345 Main St."
      },
      "primaryRole": "teacher",
      "externalId": "13013",
      "teacherNumber": "8802",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
    },
    {
      "id": "13005",
      "displayName": "Erna Parker",
      "givenName": "Erna",
      "middleName": " ",
      "surname": "Parker",
      "mail": "ernap@contoso.com",
      "mobilePhone": "+1 (253) 555-0104",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "School of Fine Art",
      "mailingAddress": {
        "city": "Buffalo",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "NY",
        "street": "12345 Main St."
      },
      "primaryRole": "student",
      "externalId": "13005",
      "birthDate": "2001-01-01T00:00:00Z",
      "gender": "female",
      "grade": "9",
      "graduationYear": "2019",
      "studentNumber": "13005",
      "residenceAddress": {
        "city": "Long Beach",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Maple St."
      },
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->