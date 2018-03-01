# <a name="delete-educationclass"></a><span data-ttu-id="0e3b5-101">删除 educationClass</span><span class="sxs-lookup"><span data-stu-id="0e3b5-101">Delete educationClass</span></span>

<span data-ttu-id="0e3b5-102">删除课程。</span><span class="sxs-lookup"><span data-stu-id="0e3b5-102">Delete a class.</span></span> <span data-ttu-id="0e3b5-103">课程也是通用组，因此删除课程时也会删除组。</span><span class="sxs-lookup"><span data-stu-id="0e3b5-103">Because a class is also a universal group, deleting a class deletes the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e3b5-104">权限</span><span class="sxs-lookup"><span data-stu-id="0e3b5-104">Permissions</span></span>
<span data-ttu-id="0e3b5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="0e3b5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0e3b5-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="0e3b5-107">Permission type</span></span>      | <span data-ttu-id="0e3b5-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0e3b5-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e3b5-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0e3b5-109">Delegated (work or school account)</span></span> |  <span data-ttu-id="0e3b5-110">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e3b5-110">Not supported.</span></span>  |
|<span data-ttu-id="0e3b5-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0e3b5-111">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0e3b5-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e3b5-112">Not supported.</span></span>  |
|<span data-ttu-id="0e3b5-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="0e3b5-113">Application</span></span> | <span data-ttu-id="0e3b5-114">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e3b5-114">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0e3b5-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e3b5-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}

```
## <a name="request-headers"></a><span data-ttu-id="0e3b5-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="0e3b5-116">Request headers</span></span>
| <span data-ttu-id="0e3b5-117">标头</span><span class="sxs-lookup"><span data-stu-id="0e3b5-117">Header</span></span>       | <span data-ttu-id="0e3b5-118">值</span><span class="sxs-lookup"><span data-stu-id="0e3b5-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0e3b5-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e3b5-119">Authorization</span></span>  | <span data-ttu-id="0e3b5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0e3b5-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0e3b5-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="0e3b5-122">Request body</span></span>
<span data-ttu-id="0e3b5-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0e3b5-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="0e3b5-124">响应</span><span class="sxs-lookup"><span data-stu-id="0e3b5-124">Response</span></span>
<span data-ttu-id="0e3b5-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0e3b5-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e3b5-127">示例</span><span class="sxs-lookup"><span data-stu-id="0e3b5-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0e3b5-128">请求</span><span class="sxs-lookup"><span data-stu-id="0e3b5-128">Request</span></span>
<span data-ttu-id="0e3b5-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0e3b5-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationclass"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/11022
```
##### <a name="response"></a><span data-ttu-id="0e3b5-130">响应</span><span class="sxs-lookup"><span data-stu-id="0e3b5-130">Response</span></span>
<span data-ttu-id="0e3b5-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0e3b5-131">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->