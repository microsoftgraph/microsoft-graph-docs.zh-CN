# <a name="create-educationclass"></a><span data-ttu-id="5a8c3-101">创建 educationClass</span><span class="sxs-lookup"><span data-stu-id="5a8c3-101">Create educationClass</span></span>

<span data-ttu-id="5a8c3-102">创建新课程。</span><span class="sxs-lookup"><span data-stu-id="5a8c3-102">Create a new class library project.</span></span> <span data-ttu-id="5a8c3-103">此操作还会创建通用组。</span><span class="sxs-lookup"><span data-stu-id="5a8c3-103">This will also create a universal group.</span></span> <span data-ttu-id="5a8c3-104">当使用此 API 创建课程时，会向组添加特殊属性，继而在 Microsoft Teams 中添加分配和特殊处理等功能。</span><span class="sxs-lookup"><span data-stu-id="5a8c3-104">When you use this API to create a class, it will add special properties to the group, which will add features such as assignments and special handling within Microsoft Teams.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a8c3-105">权限</span><span class="sxs-lookup"><span data-stu-id="5a8c3-105">Permissions</span></span>
<span data-ttu-id="5a8c3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5a8c3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5a8c3-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5a8c3-108">Permission type</span></span>      | <span data-ttu-id="5a8c3-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5a8c3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a8c3-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5a8c3-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="5a8c3-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a8c3-111">Not supported.</span></span>  |
|<span data-ttu-id="5a8c3-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5a8c3-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5a8c3-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a8c3-113">Not supported.</span></span>  |
|<span data-ttu-id="5a8c3-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="5a8c3-114">Application</span></span> | <span data-ttu-id="5a8c3-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a8c3-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5a8c3-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5a8c3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes
```
## <a name="request-headers"></a><span data-ttu-id="5a8c3-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="5a8c3-117">Request headers</span></span>
| <span data-ttu-id="5a8c3-118">标头</span><span class="sxs-lookup"><span data-stu-id="5a8c3-118">Header</span></span>       | <span data-ttu-id="5a8c3-119">值</span><span class="sxs-lookup"><span data-stu-id="5a8c3-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5a8c3-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a8c3-120">Authorization</span></span>  | <span data-ttu-id="5a8c3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5a8c3-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5a8c3-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5a8c3-123">Content-Type</span></span>  | <span data-ttu-id="5a8c3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5a8c3-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5a8c3-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="5a8c3-125">Request body</span></span>
<span data-ttu-id="5a8c3-126">在请求正文中，提供 [educationClass](../resources/educationclass.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5a8c3-126">In the request body, supply a JSON representation of an [invitation](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="5a8c3-127">响应</span><span class="sxs-lookup"><span data-stu-id="5a8c3-127">Response</span></span>
<span data-ttu-id="5a8c3-128">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5a8c3-128">If successful, this method returns a `201 Created` response code and an [event](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a8c3-129">示例</span><span class="sxs-lookup"><span data-stu-id="5a8c3-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5a8c3-130">请求</span><span class="sxs-lookup"><span data-stu-id="5a8c3-130">Request</span></span>
<span data-ttu-id="5a8c3-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5a8c3-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes
Content-type: application/json
Content-length: 224

{
  "description": "Health Level 1",
  "classCode": "Health 501",
  "displayName": "Health 1",
  "externalId": "11019",
  "externalName": "Health Level 1",
  "externalSource": "sis",
  "mailNickname": "fineartschool.net"
}
```

##### <a name="response"></a><span data-ttu-id="5a8c3-132">响应</span><span class="sxs-lookup"><span data-stu-id="5a8c3-132">Response</span></span>
<span data-ttu-id="5a8c3-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5a8c3-133">The following is an example of the response.</span></span> 

><span data-ttu-id="5a8c3-p104">**注意：**为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5a8c3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 224

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->