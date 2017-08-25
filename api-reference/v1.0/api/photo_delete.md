# <a name="delete-photo"></a><span data-ttu-id="4d19e-101">删除照片</span><span class="sxs-lookup"><span data-stu-id="4d19e-101">Delete photo</span></span>

<span data-ttu-id="4d19e-102">删除照片。</span><span class="sxs-lookup"><span data-stu-id="4d19e-102">Delete a photo.</span></span>
## <a name="permissions"></a><span data-ttu-id="4d19e-103">权限</span><span class="sxs-lookup"><span data-stu-id="4d19e-103">Permissions</span></span>
<span data-ttu-id="4d19e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="4d19e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4d19e-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="4d19e-106">Permission type</span></span>      | <span data-ttu-id="4d19e-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4d19e-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="4d19e-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4d19e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4d19e-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4d19e-109">Files.ReadWrite</span></span>    | 
|<span data-ttu-id="4d19e-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4d19e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d19e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4d19e-111">Files.ReadWrite</span></span>    | 
|<span data-ttu-id="4d19e-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="4d19e-112">Application</span></span> | <span data-ttu-id="4d19e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d19e-113">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4d19e-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4d19e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/photo
DELETE /groups/{id}/photo
DELETE /drive/root/createdByUser/photo

```
## <a name="request-headers"></a><span data-ttu-id="4d19e-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="4d19e-115">Request headers</span></span>
| <span data-ttu-id="4d19e-116">名称</span><span class="sxs-lookup"><span data-stu-id="4d19e-116">Name</span></span>       | <span data-ttu-id="4d19e-117">类型</span><span class="sxs-lookup"><span data-stu-id="4d19e-117">Type</span></span> | <span data-ttu-id="4d19e-118">说明</span><span class="sxs-lookup"><span data-stu-id="4d19e-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4d19e-119">if-match</span><span class="sxs-lookup"><span data-stu-id="4d19e-119">if-match</span></span>  | <span data-ttu-id="4d19e-120">string</span><span class="sxs-lookup"><span data-stu-id="4d19e-120">string</span></span>  | <span data-ttu-id="4d19e-121">如果包含此请求标头，且提供的 eTag（或 cTag）与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。</span><span class="sxs-lookup"><span data-stu-id="4d19e-121">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>|
| <span data-ttu-id="4d19e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d19e-122">Authorization</span></span>  | <span data-ttu-id="4d19e-123">string</span><span class="sxs-lookup"><span data-stu-id="4d19e-123">string</span></span>  | <span data-ttu-id="4d19e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4d19e-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="4d19e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4d19e-126">Request body</span></span>
<span data-ttu-id="4d19e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4d19e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d19e-128">响应</span><span class="sxs-lookup"><span data-stu-id="4d19e-128">Response</span></span>

<span data-ttu-id="4d19e-p103">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4d19e-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d19e-131">示例</span><span class="sxs-lookup"><span data-stu-id="4d19e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4d19e-132">请求</span><span class="sxs-lookup"><span data-stu-id="4d19e-132">Request</span></span>
<span data-ttu-id="4d19e-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4d19e-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
"name": "delete_photo"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="4d19e-134">响应</span><span class="sxs-lookup"><span data-stu-id="4d19e-134">Response</span></span>
<span data-ttu-id="4d19e-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4d19e-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
