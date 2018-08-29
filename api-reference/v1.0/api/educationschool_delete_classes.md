# <a name="remove-educationclass"></a><span data-ttu-id="784f3-101">删除 educationClass</span><span class="sxs-lookup"><span data-stu-id="784f3-101">Remove educationClass</span></span>

<span data-ttu-id="784f3-102">从学校删除课程。</span><span class="sxs-lookup"><span data-stu-id="784f3-102">Delete a class from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="784f3-103">权限</span><span class="sxs-lookup"><span data-stu-id="784f3-103">Permissions</span></span>
<span data-ttu-id="784f3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="784f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="784f3-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="784f3-106">Permission type</span></span>      | <span data-ttu-id="784f3-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="784f3-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="784f3-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="784f3-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="784f3-109">不支持。</span><span class="sxs-lookup"><span data-stu-id="784f3-109">Not supported.</span></span>  |
|<span data-ttu-id="784f3-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="784f3-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="784f3-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="784f3-111">Not supported.</span></span>  |
|<span data-ttu-id="784f3-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="784f3-112">Application</span></span> | <span data-ttu-id="784f3-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="784f3-113">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="784f3-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="784f3-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/classes/{classId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="784f3-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="784f3-115">Request headers</span></span>
| <span data-ttu-id="784f3-116">标头</span><span class="sxs-lookup"><span data-stu-id="784f3-116">Header</span></span>       | <span data-ttu-id="784f3-117">值</span><span class="sxs-lookup"><span data-stu-id="784f3-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="784f3-118">授权</span><span class="sxs-lookup"><span data-stu-id="784f3-118">Authorization</span></span>  | <span data-ttu-id="784f3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="784f3-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="784f3-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="784f3-121">Request body</span></span>
<span data-ttu-id="784f3-122">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="784f3-122">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="784f3-123">响应</span><span class="sxs-lookup"><span data-stu-id="784f3-123">Response</span></span>
<span data-ttu-id="784f3-124">如果成功，此方法将返回 `204 No Content` 响应代码和响应正文。</span><span class="sxs-lookup"><span data-stu-id="784f3-124">If successful, this method returns a `204 No Content` response code and a response body.</span></span>

## <a name="example"></a><span data-ttu-id="784f3-125">示例</span><span class="sxs-lookup"><span data-stu-id="784f3-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="784f3-126">请求</span><span class="sxs-lookup"><span data-stu-id="784f3-126">Request</span></span>
<span data-ttu-id="784f3-127">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="784f3-127">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}/classes/{class-id}
```

##### <a name="response"></a><span data-ttu-id="784f3-128">响应</span><span class="sxs-lookup"><span data-stu-id="784f3-128">Response</span></span>
<span data-ttu-id="784f3-129">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="784f3-129">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 204 No Content
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