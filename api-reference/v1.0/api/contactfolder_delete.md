# <a name="delete-contactfolder"></a><span data-ttu-id="3ea92-101">删除 contactFolder</span><span class="sxs-lookup"><span data-stu-id="3ea92-101">Delete contactFolder</span></span>

<span data-ttu-id="3ea92-102">删除默认 contactFolder 以外的 contactFolder。</span><span class="sxs-lookup"><span data-stu-id="3ea92-102">Delete contactFolder other than the default contactFolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="3ea92-103">权限</span><span class="sxs-lookup"><span data-stu-id="3ea92-103">Permissions</span></span>
<span data-ttu-id="3ea92-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="3ea92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3ea92-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="3ea92-106">Permission type</span></span>      | <span data-ttu-id="3ea92-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3ea92-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ea92-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3ea92-108">Delegated (work or school account)</span></span> | <span data-ttu-id="3ea92-109">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ea92-109">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="3ea92-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3ea92-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ea92-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ea92-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="3ea92-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="3ea92-112">Application</span></span> | <span data-ttu-id="3ea92-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ea92-113">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ea92-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3ea92-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/contactFolders/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3ea92-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="3ea92-115">Request headers</span></span>
| <span data-ttu-id="3ea92-116">名称</span><span class="sxs-lookup"><span data-stu-id="3ea92-116">Name</span></span>       | <span data-ttu-id="3ea92-117">类型</span><span class="sxs-lookup"><span data-stu-id="3ea92-117">Type</span></span> | <span data-ttu-id="3ea92-118">说明</span><span class="sxs-lookup"><span data-stu-id="3ea92-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3ea92-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ea92-119">Authorization</span></span>  | <span data-ttu-id="3ea92-120">string</span><span class="sxs-lookup"><span data-stu-id="3ea92-120">string</span></span>  | <span data-ttu-id="3ea92-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3ea92-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ea92-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="3ea92-123">Request body</span></span>
<span data-ttu-id="3ea92-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3ea92-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ea92-125">响应</span><span class="sxs-lookup"><span data-stu-id="3ea92-125">Response</span></span>

<span data-ttu-id="3ea92-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3ea92-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ea92-128">示例</span><span class="sxs-lookup"><span data-stu-id="3ea92-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3ea92-129">请求</span><span class="sxs-lookup"><span data-stu-id="3ea92-129">Request</span></span>
<span data-ttu-id="3ea92-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3ea92-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contactfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="3ea92-131">响应</span><span class="sxs-lookup"><span data-stu-id="3ea92-131">Response</span></span>
<span data-ttu-id="3ea92-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3ea92-132">Here is an example of the response.</span></span> 
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
  "description": "Delete contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
