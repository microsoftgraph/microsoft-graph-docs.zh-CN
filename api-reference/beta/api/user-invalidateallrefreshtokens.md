---
title: 用户： invalidateAllRefreshTokens
description: 使用户的浏览器中颁发给应用程序和会话 cookie 的用户的所有刷新令牌失效。
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 8eccbef22631657a570062d1f0c1107fba63a70b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48017078"
---
# <a name="user-invalidateallrefreshtokens"></a><span data-ttu-id="5397d-103">用户： invalidateAllRefreshTokens</span><span class="sxs-lookup"><span data-stu-id="5397d-103">user: invalidateAllRefreshTokens</span></span>

<span data-ttu-id="5397d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5397d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5397d-105">通过将 **refreshTokensValidFromDateTime** 用户属性重置为当前的日期时间来使向应用程序颁发的所有用户的刷新令牌（以及用户浏览器中的会话 cookie）)  (。</span><span class="sxs-lookup"><span data-stu-id="5397d-105">Invalidates all of the user's refresh tokens issued to applications (as well as session cookies in a user's browser), by resetting the **refreshTokensValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="5397d-106">通常情况下，如果用户的设备丢失或被盗， (由用户或管理员) 执行此操作。</span><span class="sxs-lookup"><span data-stu-id="5397d-106">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span>  <span data-ttu-id="5397d-107">此操作将阻止访问通过设备上的应用程序访问的任何组织数据，而用户首次无需再次登录。</span><span class="sxs-lookup"><span data-stu-id="5397d-107">This operation would prevent access to any of the organization's data accessed through applications on the device without the user first being required to sign in again.</span></span> <span data-ttu-id="5397d-108">实际上，此操作会强制用户再次登录到他们之前同意的所有应用程序，而不依赖于设备。</span><span class="sxs-lookup"><span data-stu-id="5397d-108">In fact, this operation would force the user to sign in again for all applications that they have previously consented to, independent of device.</span></span>

<span data-ttu-id="5397d-109">对于开发人员，如果应用程序尝试使用无效刷新令牌兑换此用户的委派访问令牌，应用程序将收到错误。</span><span class="sxs-lookup"><span data-stu-id="5397d-109">For developers, if the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="5397d-110">如果发生这种情况，应用程序将需要通过向授权终结点发出请求来获取新的刷新令牌，这将强制用户登录。</span><span class="sxs-lookup"><span data-stu-id="5397d-110">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

## <a name="permissions"></a><span data-ttu-id="5397d-111">权限</span><span class="sxs-lookup"><span data-stu-id="5397d-111">Permissions</span></span>
<span data-ttu-id="5397d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5397d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

+ <span data-ttu-id="5397d-114">对于允许已登录用户使已登录的应用程序无效的应用程序，请执行以下操作： User. ReadWrite、Directory.accessasuser.all</span><span class="sxs-lookup"><span data-stu-id="5397d-114">For an application to allow the signed in user to invalidate applications they've consented to: User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>
+ <span data-ttu-id="5397d-115">对于允许管理员使用户同意的应用程序无效的应用程序，请执行以下操作： Directory.accessasuser.all</span><span class="sxs-lookup"><span data-stu-id="5397d-115">For an application to allow an administrator to invalidate applications a user has consented to: Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="5397d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5397d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/invalidateAllRefreshTokens
POST /users/{id | userPrincipalName}/invalidateAllRefreshTokens
```
## <a name="request-headers"></a><span data-ttu-id="5397d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="5397d-117">Request headers</span></span>
| <span data-ttu-id="5397d-118">标头</span><span class="sxs-lookup"><span data-stu-id="5397d-118">Header</span></span>       | <span data-ttu-id="5397d-119">值</span><span class="sxs-lookup"><span data-stu-id="5397d-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5397d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5397d-120">Authorization</span></span>  | <span data-ttu-id="5397d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5397d-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5397d-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="5397d-123">Request body</span></span>
<span data-ttu-id="5397d-124">此操作没有请求内容。</span><span class="sxs-lookup"><span data-stu-id="5397d-124">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="5397d-125">响应</span><span class="sxs-lookup"><span data-stu-id="5397d-125">Response</span></span>

<span data-ttu-id="5397d-126">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5397d-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5397d-127">示例</span><span class="sxs-lookup"><span data-stu-id="5397d-127">Example</span></span>
<span data-ttu-id="5397d-128">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="5397d-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5397d-129">请求</span><span class="sxs-lookup"><span data-stu-id="5397d-129">Request</span></span>
<span data-ttu-id="5397d-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5397d-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5397d-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="5397d-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_invalidateallrefreshtokens"
}-->
```http
POST https://graph.microsoft.com/beta/me/invalidateAllRefreshTokens
```
# <a name="c"></a>[<span data-ttu-id="5397d-132">C#</span><span class="sxs-lookup"><span data-stu-id="5397d-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-invalidateallrefreshtokens-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5397d-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5397d-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-invalidateallrefreshtokens-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5397d-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5397d-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-invalidateallrefreshtokens-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5397d-135">响应</span><span class="sxs-lookup"><span data-stu-id="5397d-135">Response</span></span>
<span data-ttu-id="5397d-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5397d-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: invalidateAllRefreshTokens",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


