# <a name="list-classes"></a><span data-ttu-id="42e1f-101">列出课程</span><span class="sxs-lookup"><span data-stu-id="42e1f-101">List classes</span></span>

<span data-ttu-id="42e1f-102">检索 class 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="42e1f-102">Retrieve a list of class objects.</span></span> <span data-ttu-id="42e1f-103">请注意，如果使用委派令牌，成员只能看到有关其自己课程的信息。</span><span class="sxs-lookup"><span data-stu-id="42e1f-103">Note that if the delegated token is used, members can only see information about their own classes.</span></span> 

<!-- Please verify the revision to the delegated token text. -->

## <a name="permissions"></a><span data-ttu-id="42e1f-104">权限</span><span class="sxs-lookup"><span data-stu-id="42e1f-104">Permissions</span></span>
<span data-ttu-id="42e1f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="42e1f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="42e1f-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="42e1f-107">Permission type</span></span>      | <span data-ttu-id="42e1f-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="42e1f-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42e1f-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="42e1f-109">Delegated (work or school account)</span></span> |  <span data-ttu-id="42e1f-110">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="42e1f-110">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="42e1f-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="42e1f-111">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="42e1f-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="42e1f-112">Not supported.</span></span>  |
|<span data-ttu-id="42e1f-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="42e1f-113">Application</span></span> | <span data-ttu-id="42e1f-114">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42e1f-114">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="42e1f-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="42e1f-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/classes
GET /education/users/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="42e1f-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="42e1f-116">Optional query parameters</span></span>
<span data-ttu-id="42e1f-117">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="42e1f-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="42e1f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="42e1f-118">Request headers</span></span>
| <span data-ttu-id="42e1f-119">标头</span><span class="sxs-lookup"><span data-stu-id="42e1f-119">Header</span></span>       | <span data-ttu-id="42e1f-120">值</span><span class="sxs-lookup"><span data-stu-id="42e1f-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="42e1f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="42e1f-121">Authorization</span></span>  | <span data-ttu-id="42e1f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="42e1f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="42e1f-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="42e1f-124">Request body</span></span>
<span data-ttu-id="42e1f-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="42e1f-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="42e1f-126">响应</span><span class="sxs-lookup"><span data-stu-id="42e1f-126">Response</span></span>
<span data-ttu-id="42e1f-127">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationClass](../resources/educationclass.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="42e1f-127">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="42e1f-128">示例</span><span class="sxs-lookup"><span data-stu-id="42e1f-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="42e1f-129">请求</span><span class="sxs-lookup"><span data-stu-id="42e1f-129">Request</span></span>
<span data-ttu-id="42e1f-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="42e1f-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/me/classes
```
##### <a name="response"></a><span data-ttu-id="42e1f-131">响应</span><span class="sxs-lookup"><span data-stu-id="42e1f-131">Response</span></span>
<span data-ttu-id="42e1f-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="42e1f-132">The following is an example of the response.</span></span> 

><span data-ttu-id="42e1f-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="42e1f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 277

{
  "value": [
    {
      "id": "11019",
      "description": "Health Level 1",
      "classCode": "Health 501",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "displayName": "Health 1",
      "externalId": "11019",
      "externalName": "Health Level 1",
      "externalSource": "sis",
      "mailNickname": "fineartschool.net"
    } 
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List classes",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->