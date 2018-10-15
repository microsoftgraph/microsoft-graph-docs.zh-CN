# <a name="add-a-student"></a><span data-ttu-id="e1bd6-101">添加学生</span><span class="sxs-lookup"><span data-stu-id="e1bd6-101">Add a student</span></span>

<span data-ttu-id="e1bd6-102">向课程添加成员。</span><span class="sxs-lookup"><span data-stu-id="e1bd6-102">Add a member to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1bd6-103">权限</span><span class="sxs-lookup"><span data-stu-id="e1bd6-103">Permissions</span></span>
<span data-ttu-id="e1bd6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e1bd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e1bd6-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="e1bd6-106">Permission type</span></span>      | <span data-ttu-id="e1bd6-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e1bd6-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1bd6-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e1bd6-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="e1bd6-109">不支持。</span><span class="sxs-lookup"><span data-stu-id="e1bd6-109">Not supported.</span></span>  |
|<span data-ttu-id="e1bd6-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e1bd6-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e1bd6-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="e1bd6-111">Not supported.</span></span>  |
|<span data-ttu-id="e1bd6-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="e1bd6-112">Application</span></span> | <span data-ttu-id="e1bd6-113">EduRoster.ReadWrite.All 以及 Member.Read.Hidden</span><span class="sxs-lookup"><span data-stu-id="e1bd6-113">EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e1bd6-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e1bd6-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="e1bd6-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="e1bd6-115">Request headers</span></span>
| <span data-ttu-id="e1bd6-116">标头</span><span class="sxs-lookup"><span data-stu-id="e1bd6-116">Header</span></span>       | <span data-ttu-id="e1bd6-117">值</span><span class="sxs-lookup"><span data-stu-id="e1bd6-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e1bd6-118">授权</span><span class="sxs-lookup"><span data-stu-id="e1bd6-118">Authorization</span></span>  | <span data-ttu-id="e1bd6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e1bd6-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e1bd6-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e1bd6-121">Content-Type</span></span>  | <span data-ttu-id="e1bd6-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e1bd6-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e1bd6-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="e1bd6-123">Request body</span></span>
<span data-ttu-id="e1bd6-124">在请求正文中，提供 [educationUser](../resources/educationuser.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1bd6-124">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="e1bd6-125">响应</span><span class="sxs-lookup"><span data-stu-id="e1bd6-125">Response</span></span>
<span data-ttu-id="e1bd6-126">如果成功，此方法会在响应正文中返回 `204 No Content` 响应代码和 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e1bd6-126">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1bd6-127">示例</span><span class="sxs-lookup"><span data-stu-id="e1bd6-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e1bd6-128">请求</span><span class="sxs-lookup"><span data-stu-id="e1bd6-128">Request</span></span>
<span data-ttu-id="e1bd6-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e1bd6-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/{class-id}/members/$ref
Content-type: application/json
Content-length: 56

{
  "@odata.id":"https://graph.microsoft.com/v1.0/education/users/13015"
}
```

##### <a name="response"></a><span data-ttu-id="e1bd6-130">响应</span><span class="sxs-lookup"><span data-stu-id="e1bd6-130">Response</span></span>
<span data-ttu-id="e1bd6-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e1bd6-131">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 204 No Content
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
