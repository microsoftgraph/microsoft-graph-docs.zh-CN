# <a name="delete-a-user"></a><span data-ttu-id="04703-101">删除用户</span><span class="sxs-lookup"><span data-stu-id="04703-101">Delete a user</span></span>

<span data-ttu-id="04703-102">删除用户。</span><span class="sxs-lookup"><span data-stu-id="04703-102">Delete user.</span></span>
## <a name="permissions"></a><span data-ttu-id="04703-103">权限</span><span class="sxs-lookup"><span data-stu-id="04703-103">Permissions</span></span>
<span data-ttu-id="04703-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="04703-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="04703-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="04703-106">Permission type</span></span>      | <span data-ttu-id="04703-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="04703-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04703-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="04703-108">Delegated (work or school account)</span></span> | <span data-ttu-id="04703-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="04703-109">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="04703-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="04703-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04703-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="04703-111">Not supported.</span></span>    |
|<span data-ttu-id="04703-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="04703-112">Application</span></span> | <span data-ttu-id="04703-113">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04703-113">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="04703-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="04703-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="04703-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="04703-115">Request headers</span></span>
| <span data-ttu-id="04703-116">标头</span><span class="sxs-lookup"><span data-stu-id="04703-116">Header</span></span>       | <span data-ttu-id="04703-117">值</span><span class="sxs-lookup"><span data-stu-id="04703-117">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="04703-118">授权</span><span class="sxs-lookup"><span data-stu-id="04703-118">Authorization</span></span>  | <span data-ttu-id="04703-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="04703-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="04703-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="04703-121">Request body</span></span>
<span data-ttu-id="04703-122">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="04703-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04703-123">响应</span><span class="sxs-lookup"><span data-stu-id="04703-123">Response</span></span>

<span data-ttu-id="04703-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="04703-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04703-126">示例</span><span class="sxs-lookup"><span data-stu-id="04703-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="04703-127">请求</span><span class="sxs-lookup"><span data-stu-id="04703-127">Request</span></span>
<span data-ttu-id="04703-128">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="04703-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{user-id}
```
##### <a name="response"></a><span data-ttu-id="04703-129">响应</span><span class="sxs-lookup"><span data-stu-id="04703-129">Response</span></span>
<span data-ttu-id="04703-130">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="04703-130">Here is an example of the response.</span></span> 
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
  "description": "Delete user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->