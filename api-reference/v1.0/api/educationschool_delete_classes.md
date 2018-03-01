# <a name="remove-educationclass"></a><span data-ttu-id="d186c-101">删除 educationClass</span><span class="sxs-lookup"><span data-stu-id="d186c-101">Remove educationClass</span></span>

<span data-ttu-id="d186c-102">从学校删除课程。</span><span class="sxs-lookup"><span data-stu-id="d186c-102">Delete a class from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="d186c-103">权限</span><span class="sxs-lookup"><span data-stu-id="d186c-103">Permissions</span></span>
<span data-ttu-id="d186c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d186c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d186c-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="d186c-106">Permission type</span></span>      | <span data-ttu-id="d186c-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d186c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d186c-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d186c-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="d186c-109">不支持。</span><span class="sxs-lookup"><span data-stu-id="d186c-109">Not supported.</span></span>  |
|<span data-ttu-id="d186c-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d186c-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d186c-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="d186c-111">Not supported.</span></span>  |
|<span data-ttu-id="d186c-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="d186c-112">Application</span></span> | <span data-ttu-id="d186c-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d186c-113">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d186c-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d186c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/classes/{classId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="d186c-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="d186c-115">Request headers</span></span>
| <span data-ttu-id="d186c-116">标头</span><span class="sxs-lookup"><span data-stu-id="d186c-116">Header</span></span>       | <span data-ttu-id="d186c-117">值</span><span class="sxs-lookup"><span data-stu-id="d186c-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d186c-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="d186c-118">Authorization</span></span>  | <span data-ttu-id="d186c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d186c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d186c-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="d186c-121">Request body</span></span>
<span data-ttu-id="d186c-122">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d186c-122">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="d186c-123">响应</span><span class="sxs-lookup"><span data-stu-id="d186c-123">Response</span></span>
<span data-ttu-id="d186c-124">如果成功，此方法将返回 `204 No Content` 响应代码和响应正文。</span><span class="sxs-lookup"><span data-stu-id="d186c-124">If successful, this method returns a `204 No Content` response code and a sharedDriveItem resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d186c-125">示例</span><span class="sxs-lookup"><span data-stu-id="d186c-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d186c-126">请求</span><span class="sxs-lookup"><span data-stu-id="d186c-126">Request</span></span>
<span data-ttu-id="d186c-127">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d186c-127">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/10001/classes/11001
```

##### <a name="response"></a><span data-ttu-id="d186c-128">响应</span><span class="sxs-lookup"><span data-stu-id="d186c-128">Response</span></span>
<span data-ttu-id="d186c-129">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d186c-129">The following is an example of the response.</span></span> 

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