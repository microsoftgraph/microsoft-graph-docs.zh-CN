# <a name="delete-directoryobject"></a><span data-ttu-id="29cb2-101">删除 directoryObject</span><span class="sxs-lookup"><span data-stu-id="29cb2-101">Delete directoryObject</span></span>

<span data-ttu-id="29cb2-102">删除 directoryObject。</span><span class="sxs-lookup"><span data-stu-id="29cb2-102">Deletes a directoryObject.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29cb2-103">先决条件</span><span class="sxs-lookup"><span data-stu-id="29cb2-103">Prerequisites</span></span>
<span data-ttu-id="29cb2-104">需要以下**范围**才能执行此 API：_Directory.AccessAsUser.All_</span><span class="sxs-lookup"><span data-stu-id="29cb2-104">The following **scopes** is required to execute this API: _Directory.AccessAsUser.All_</span></span>

<span data-ttu-id="29cb2-p101">**注意：**用户、组和联系人是 directory 对象的类型。因此，如果需要删除用户，可以而且应该使用以下**范围**：_User.ReadWrite.All_</span><span class="sxs-lookup"><span data-stu-id="29cb2-p101">**NOTE:** Users, groups, and contacts are types of directory object. As a result,if you need to delete users, the following **scope** can and should be used: _User.ReadWrite.All_</span></span>
## <a name="http-request"></a><span data-ttu-id="29cb2-107">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="29cb2-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="29cb2-108">请求标头</span><span class="sxs-lookup"><span data-stu-id="29cb2-108">Request headers</span></span>
| <span data-ttu-id="29cb2-109">名称</span><span class="sxs-lookup"><span data-stu-id="29cb2-109">Name</span></span>       | <span data-ttu-id="29cb2-110">类型</span><span class="sxs-lookup"><span data-stu-id="29cb2-110">Type</span></span> | <span data-ttu-id="29cb2-111">说明</span><span class="sxs-lookup"><span data-stu-id="29cb2-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="29cb2-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="29cb2-112">Authorization</span></span>  | <span data-ttu-id="29cb2-113">string</span><span class="sxs-lookup"><span data-stu-id="29cb2-113">string</span></span>  | <span data-ttu-id="29cb2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="29cb2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="29cb2-116">请求正文</span><span class="sxs-lookup"><span data-stu-id="29cb2-116">Request body</span></span>
<span data-ttu-id="29cb2-117">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="29cb2-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29cb2-118">响应</span><span class="sxs-lookup"><span data-stu-id="29cb2-118">Response</span></span>

<span data-ttu-id="29cb2-p103">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="29cb2-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29cb2-121">示例</span><span class="sxs-lookup"><span data-stu-id="29cb2-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="29cb2-122">请求</span><span class="sxs-lookup"><span data-stu-id="29cb2-122">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directoryObject/{id}
```
##### <a name="response"></a><span data-ttu-id="29cb2-123">响应</span><span class="sxs-lookup"><span data-stu-id="29cb2-123">Response</span></span>

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
  "description": "Delete directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->