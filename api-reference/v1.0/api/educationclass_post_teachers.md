# <a name="add-teacher"></a><span data-ttu-id="2f4a3-101">添加教师</span><span class="sxs-lookup"><span data-stu-id="2f4a3-101">Add teacher</span></span>

<span data-ttu-id="2f4a3-102">向课程添加教师。</span><span class="sxs-lookup"><span data-stu-id="2f4a3-102">Add a teacher to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f4a3-103">权限</span><span class="sxs-lookup"><span data-stu-id="2f4a3-103">Permissions</span></span>
<span data-ttu-id="2f4a3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="2f4a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2f4a3-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f4a3-106">Permission type</span></span>      | <span data-ttu-id="2f4a3-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2f4a3-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f4a3-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f4a3-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="2f4a3-109">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f4a3-109">Not supported.</span></span>  |
|<span data-ttu-id="2f4a3-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f4a3-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2f4a3-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f4a3-111">Not supported.</span></span>  |
|<span data-ttu-id="2f4a3-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f4a3-112">Application</span></span> | <span data-ttu-id="2f4a3-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f4a3-113">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2f4a3-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f4a3-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/teachers/$ref
```
## <a name="request-headers"></a><span data-ttu-id="2f4a3-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f4a3-115">Request headers</span></span>
| <span data-ttu-id="2f4a3-116">标头</span><span class="sxs-lookup"><span data-stu-id="2f4a3-116">Header</span></span>       | <span data-ttu-id="2f4a3-117">值</span><span class="sxs-lookup"><span data-stu-id="2f4a3-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2f4a3-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f4a3-118">Authorization</span></span>  | <span data-ttu-id="2f4a3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2f4a3-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2f4a3-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2f4a3-121">Content-Type</span></span>  | <span data-ttu-id="2f4a3-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2f4a3-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2f4a3-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f4a3-123">Request body</span></span>
<span data-ttu-id="2f4a3-124">在请求正文中，提供 [educationUser](../resources/educationuser.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f4a3-124">In the request body, supply a JSON representation of an [invitation](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="2f4a3-125">响应</span><span class="sxs-lookup"><span data-stu-id="2f4a3-125">Response</span></span>
<span data-ttu-id="2f4a3-126">如果成功，此方法会在响应正文中返回 `204 No Content` 响应代码和 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2f4a3-126">If successful, this method returns a `204 No Content` response code and an [event](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f4a3-127">示例</span><span class="sxs-lookup"><span data-stu-id="2f4a3-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2f4a3-128">请求</span><span class="sxs-lookup"><span data-stu-id="2f4a3-128">Request</span></span>
<span data-ttu-id="2f4a3-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2f4a3-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/11017/teachers/$ref
Content-type: application/json
Content-length: 508

{
  "@odata.id":"https://graph.microsoft.com/v1.0/education/users/14011"
}
```

##### <a name="response"></a><span data-ttu-id="2f4a3-130">响应</span><span class="sxs-lookup"><span data-stu-id="2f4a3-130">Response</span></span>
<span data-ttu-id="2f4a3-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2f4a3-131">The following is an example of the response.</span></span> 

<!-- Add the educationClass object to the response -->

><span data-ttu-id="2f4a3-p103">**注意：**为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2f4a3-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
