---
title: user： revokeSignInSessions
description: 将 **signInSessionsValidFromDateTime** 用户属性重置为当前日期时间，使颁发给应用程序 (的所有用户刷新令牌以及用户浏览器) 中的会话 Cookie 失效。
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: ed8cbcf1e0b04bc93af06b699f37fe0f693280f5
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721381"
---
# <a name="user-revokesigninsessions"></a><span data-ttu-id="5a63e-103">user： revokeSignInSessions</span><span class="sxs-lookup"><span data-stu-id="5a63e-103">user: revokeSignInSessions</span></span>

<span data-ttu-id="5a63e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a63e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5a63e-105">将 **signInSessionsValidFromDateTime** 用户属性重置为当前日期时间，使颁发给用户 (应用程序的所有刷新令牌以及用户浏览器) 中的会话 Cookie 失效。</span><span class="sxs-lookup"><span data-stu-id="5a63e-105">Invalidates all the refresh tokens issued to applications for a user (as well as session cookies in a user's browser), by resetting the **signInSessionsValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="5a63e-106">通常，如果用户的设备丢失 (，则由) 管理员或管理员执行此操作。</span><span class="sxs-lookup"><span data-stu-id="5a63e-106">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span> <span data-ttu-id="5a63e-107">此操作通过要求用户重新登录到他们之前同意的所有应用程序（独立于设备）来阻止通过设备上的应用程序访问组织的数据。</span><span class="sxs-lookup"><span data-stu-id="5a63e-107">This operation prevents access to the organization's data through applications on the device by requiring the user to sign in again to all applications that they have previously consented to, independent of device.</span></span>

><span data-ttu-id="5a63e-108">如果应用程序尝试使用无效的刷新令牌兑换此用户的委派访问令牌，则应用程序将发生错误。</span><span class="sxs-lookup"><span data-stu-id="5a63e-108">If the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="5a63e-109">如果发生这种情况，应用程序将需要通过向授权终结点提出请求来获取新的刷新令牌，这将强制用户登录。</span><span class="sxs-lookup"><span data-stu-id="5a63e-109">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

>[!NOTE]
><span data-ttu-id="5a63e-110">调用 **revokeSignInSessions** 后，在吊销令牌之前，可能有几分钟的延迟。</span><span class="sxs-lookup"><span data-stu-id="5a63e-110">After calling **revokeSignInSessions**, there might be a small delay of a few minutes before tokens are revoked.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a63e-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="5a63e-111">Permissions</span></span>

<span data-ttu-id="5a63e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5a63e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a63e-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="5a63e-114">Permission type</span></span>                        | <span data-ttu-id="5a63e-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5a63e-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a63e-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5a63e-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="5a63e-117">User.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5a63e-117">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="5a63e-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5a63e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a63e-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a63e-119">Not supported.</span></span> |
|<span data-ttu-id="5a63e-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="5a63e-120">Application</span></span>                            | <span data-ttu-id="5a63e-121">User.ReadWrite.All、Directory.ReadWrite.All、</span><span class="sxs-lookup"><span data-stu-id="5a63e-121">User.ReadWrite.All, Directory.ReadWrite.All,</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a63e-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5a63e-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/revokeSignInSessions
POST /users/{id | userPrincipalName}/revokeSignInSessions
```

## <a name="request-headers"></a><span data-ttu-id="5a63e-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="5a63e-123">Request headers</span></span>
| <span data-ttu-id="5a63e-124">标头</span><span class="sxs-lookup"><span data-stu-id="5a63e-124">Header</span></span>       | <span data-ttu-id="5a63e-125">值</span><span class="sxs-lookup"><span data-stu-id="5a63e-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5a63e-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a63e-126">Authorization</span></span>  | <span data-ttu-id="5a63e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5a63e-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5a63e-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5a63e-129">Content-Type</span></span>  | <span data-ttu-id="5a63e-130">application/json</span><span class="sxs-lookup"><span data-stu-id="5a63e-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5a63e-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="5a63e-131">Request body</span></span>
<span data-ttu-id="5a63e-132">此操作没有请求内容。</span><span class="sxs-lookup"><span data-stu-id="5a63e-132">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="5a63e-133">响应</span><span class="sxs-lookup"><span data-stu-id="5a63e-133">Response</span></span>

<span data-ttu-id="5a63e-134">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5a63e-134">If successful, this method returns a `204 No Content` response code.</span></span>

>[!NOTE]
><span data-ttu-id="5a63e-135">此 API 存在一个[已知问题](/graph/known-issues#revoke-sign-in-sessions-returns-wrong-HTTP-code)。</span><span class="sxs-lookup"><span data-stu-id="5a63e-135">This API has a [known issue](/graph/known-issues#revoke-sign-in-sessions-returns-wrong-HTTP-code).</span></span> <span data-ttu-id="5a63e-136">它返回不同的 HTTP 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5a63e-136">It returns a different HTTP response code.</span></span>

## <a name="example"></a><span data-ttu-id="5a63e-137">示例</span><span class="sxs-lookup"><span data-stu-id="5a63e-137">Example</span></span>
<span data-ttu-id="5a63e-138">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="5a63e-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="5a63e-139">请求</span><span class="sxs-lookup"><span data-stu-id="5a63e-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5a63e-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a63e-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_revokesigninsessionss"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/revokeSignInSessions
```
# <a name="c"></a>[<span data-ttu-id="5a63e-141">C#</span><span class="sxs-lookup"><span data-stu-id="5a63e-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-revokesigninsessionss-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5a63e-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a63e-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-revokesigninsessionss-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5a63e-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a63e-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-revokesigninsessionss-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5a63e-144">Java</span><span class="sxs-lookup"><span data-stu-id="5a63e-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-revokesigninsessionss-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5a63e-145">响应</span><span class="sxs-lookup"><span data-stu-id="5a63e-145">Response</span></span>
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
  "description": "user: revokeSignInSessions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

