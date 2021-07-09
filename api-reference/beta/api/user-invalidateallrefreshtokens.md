---
title: user：invalidateAllRefreshTokens
description: 使颁发给用户浏览器中的应用程序和会话 Cookie 的用户刷新令牌失效。
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: a13982cb924c5c9b82c3248aefc13a54ec44bb2e
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351046"
---
# <a name="user-invalidateallrefreshtokens"></a><span data-ttu-id="f1e2c-103">user：invalidateAllRefreshTokens</span><span class="sxs-lookup"><span data-stu-id="f1e2c-103">user: invalidateAllRefreshTokens</span></span>

<span data-ttu-id="f1e2c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1e2c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1e2c-105">将 **refreshTokensValidFromDateTime** 用户属性重置为当前日期时间，使颁发给应用程序 (的所有用户刷新令牌以及用户浏览器) 中的会话 cookie 失效。</span><span class="sxs-lookup"><span data-stu-id="f1e2c-105">Invalidates all of the user's refresh tokens issued to applications (as well as session cookies in a user's browser), by resetting the **refreshTokensValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="f1e2c-106">通常，如果用户的设备丢失 (，则由) 管理员或管理员执行此操作。</span><span class="sxs-lookup"><span data-stu-id="f1e2c-106">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span>  <span data-ttu-id="f1e2c-107">此操作将阻止访问通过设备上的应用程序访问的任何组织数据，而无需首先要求用户重新登录。</span><span class="sxs-lookup"><span data-stu-id="f1e2c-107">This operation would prevent access to any of the organization's data accessed through applications on the device without the user first being required to sign in again.</span></span> <span data-ttu-id="f1e2c-108">事实上，此操作将强制用户重新登录之前已同意的所有应用程序，而与设备无关。</span><span class="sxs-lookup"><span data-stu-id="f1e2c-108">In fact, this operation would force the user to sign in again for all applications that they have previously consented to, independent of device.</span></span>

<span data-ttu-id="f1e2c-109">对于开发人员，如果应用程序尝试使用无效的刷新令牌为该用户兑换委派访问令牌，则应用程序将发生错误。</span><span class="sxs-lookup"><span data-stu-id="f1e2c-109">For developers, if the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="f1e2c-110">如果发生这种情况，应用程序将需要通过向授权终结点提出请求来获取新的刷新令牌，这将强制用户登录。</span><span class="sxs-lookup"><span data-stu-id="f1e2c-110">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1e2c-111">权限</span><span class="sxs-lookup"><span data-stu-id="f1e2c-111">Permissions</span></span>
<span data-ttu-id="f1e2c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f1e2c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

+ <span data-ttu-id="f1e2c-114">对于允许登录用户使已同意的应用程序无效的应用程序的应用程序：User.ReadWrite、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f1e2c-114">For an application to allow the signed in user to invalidate applications they've consented to: User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>
+ <span data-ttu-id="f1e2c-115">对于允许管理员使用户同意的应用程序无效的应用程序的应用程序：Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f1e2c-115">For an application to allow an administrator to invalidate applications a user has consented to: Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="f1e2c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f1e2c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/invalidateAllRefreshTokens
POST /users/{id | userPrincipalName}/invalidateAllRefreshTokens
```
## <a name="request-headers"></a><span data-ttu-id="f1e2c-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="f1e2c-117">Request headers</span></span>
| <span data-ttu-id="f1e2c-118">标头</span><span class="sxs-lookup"><span data-stu-id="f1e2c-118">Header</span></span>       | <span data-ttu-id="f1e2c-119">值</span><span class="sxs-lookup"><span data-stu-id="f1e2c-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f1e2c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1e2c-120">Authorization</span></span>  | <span data-ttu-id="f1e2c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f1e2c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f1e2c-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="f1e2c-123">Request body</span></span>
<span data-ttu-id="f1e2c-124">此操作没有请求内容。</span><span class="sxs-lookup"><span data-stu-id="f1e2c-124">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="f1e2c-125">响应</span><span class="sxs-lookup"><span data-stu-id="f1e2c-125">Response</span></span>

<span data-ttu-id="f1e2c-126">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f1e2c-126">If successful, this method returns `204 No Content` response code.</span></span>

>[!NOTE]
><span data-ttu-id="f1e2c-127">此 API 返回不同的 HTTP 响应代码，类似于 [revokeSignInSessions](user-revokesigninsessions.md) 操作。</span><span class="sxs-lookup"><span data-stu-id="f1e2c-127">This API returns a different HTTP response code, similar to the [revokeSignInSessions](user-revokesigninsessions.md) action.</span></span> <span data-ttu-id="f1e2c-128">有关详细信息，请参阅 [已知问题](/graph/known-issues#revoke-sign-in-sessions-returns-wrong-HTTP-code)。</span><span class="sxs-lookup"><span data-stu-id="f1e2c-128">For details, see [known issue](/graph/known-issues#revoke-sign-in-sessions-returns-wrong-HTTP-code).</span></span> 

## <a name="example"></a><span data-ttu-id="f1e2c-129">示例</span><span class="sxs-lookup"><span data-stu-id="f1e2c-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1e2c-130">请求</span><span class="sxs-lookup"><span data-stu-id="f1e2c-130">Request</span></span>
<span data-ttu-id="f1e2c-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f1e2c-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f1e2c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1e2c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_invalidateallrefreshtokens"
}-->
```http
POST https://graph.microsoft.com/beta/me/invalidateAllRefreshTokens
```
# <a name="c"></a>[<span data-ttu-id="f1e2c-133">C#</span><span class="sxs-lookup"><span data-stu-id="f1e2c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-invalidateallrefreshtokens-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f1e2c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1e2c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-invalidateallrefreshtokens-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f1e2c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f1e2c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-invalidateallrefreshtokens-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f1e2c-136">Java</span><span class="sxs-lookup"><span data-stu-id="f1e2c-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-invalidateallrefreshtokens-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f1e2c-137">响应</span><span class="sxs-lookup"><span data-stu-id="f1e2c-137">Response</span></span>
<span data-ttu-id="f1e2c-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f1e2c-138">The following is an example of the response.</span></span> 
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


