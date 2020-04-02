---
title: 用户： revokeSignInSessions
description: 通过将**signInSessionsValidFromDateTime**用户属性重置为当前的日期时间来使向应用程序颁发的所有用户的刷新令牌失效（以及用户浏览器中的会话 cookie）。
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: cd85304459f0d3208b62f2976aa1a53bda8cb2b9
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2020
ms.locfileid: "43107344"
---
# <a name="user-revokesigninsessions"></a><span data-ttu-id="0dadf-103">用户： revokeSignInSessions</span><span class="sxs-lookup"><span data-stu-id="0dadf-103">user: revokeSignInSessions</span></span>

<span data-ttu-id="0dadf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0dadf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0dadf-105">通过将**signInSessionsValidFromDateTime**用户属性重置为当前的日期时间，使向用户（以及用户浏览器中的会话 cookie）发出的所有刷新令牌失效。</span><span class="sxs-lookup"><span data-stu-id="0dadf-105">Invalidates all the refresh tokens issued to applications for a user (as well as session cookies in a user's browser), by resetting the **signInSessionsValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="0dadf-106">通常，如果用户有丢失或被盗的设备，则执行此操作（由用户或管理员执行）。</span><span class="sxs-lookup"><span data-stu-id="0dadf-106">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span> <span data-ttu-id="0dadf-107">此操作通过要求用户再次登录到之前已同意的所有应用程序（独立于设备）来阻止对组织中的应用程序的数据的访问。</span><span class="sxs-lookup"><span data-stu-id="0dadf-107">This operation prevents access to the organization's data through applications on the device by requiring the user to sign in again to all applications that they have previously consented to, independent of device.</span></span>

<span data-ttu-id="0dadf-108">如果应用程序尝试使用无效刷新令牌兑换此用户的委派访问令牌，应用程序将收到错误。</span><span class="sxs-lookup"><span data-stu-id="0dadf-108">If the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="0dadf-109">如果发生这种情况，应用程序将需要通过向授权终结点发出请求来获取新的刷新令牌，这将强制用户登录。</span><span class="sxs-lookup"><span data-stu-id="0dadf-109">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

>[!NOTE]
><span data-ttu-id="0dadf-110">在调用**revokeSignInSessions**后，可能会有几分钟的短暂延迟才会被吊销令牌。</span><span class="sxs-lookup"><span data-stu-id="0dadf-110">After calling **revokeSignInSessions**, there might be a small delay of a few minutes before tokens are revoked.</span></span>

## <a name="permissions"></a><span data-ttu-id="0dadf-111">权限</span><span class="sxs-lookup"><span data-stu-id="0dadf-111">Permissions</span></span>

<span data-ttu-id="0dadf-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0dadf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0dadf-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="0dadf-114">Permission type</span></span>                        | <span data-ttu-id="0dadf-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0dadf-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0dadf-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0dadf-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="0dadf-117">Directory.accessasuser.all 的所有用户的读写。</span><span class="sxs-lookup"><span data-stu-id="0dadf-117">User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="0dadf-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0dadf-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0dadf-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="0dadf-119">Not supported.</span></span> |
|<span data-ttu-id="0dadf-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="0dadf-120">Application</span></span>                            | <span data-ttu-id="0dadf-121">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0dadf-121">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0dadf-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0dadf-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/revokeSignInSessions
POST /users/{id | userPrincipalName}/revokeSignInSessions
```

## <a name="request-headers"></a><span data-ttu-id="0dadf-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="0dadf-123">Request headers</span></span>
| <span data-ttu-id="0dadf-124">标头</span><span class="sxs-lookup"><span data-stu-id="0dadf-124">Header</span></span>       | <span data-ttu-id="0dadf-125">值</span><span class="sxs-lookup"><span data-stu-id="0dadf-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0dadf-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="0dadf-126">Authorization</span></span>  | <span data-ttu-id="0dadf-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0dadf-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0dadf-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0dadf-129">Content-Type</span></span>  | <span data-ttu-id="0dadf-130">application/json</span><span class="sxs-lookup"><span data-stu-id="0dadf-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0dadf-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="0dadf-131">Request body</span></span>
<span data-ttu-id="0dadf-132">此操作没有请求内容。</span><span class="sxs-lookup"><span data-stu-id="0dadf-132">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="0dadf-133">响应</span><span class="sxs-lookup"><span data-stu-id="0dadf-133">Response</span></span>

<span data-ttu-id="0dadf-134">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="0dadf-134">If successful, this method returns a `204 No Content` response code.</span></span>

>[!NOTE]
><span data-ttu-id="0dadf-135">此 API 存在一个[已知问题](/graph/known-issues#revoke-sign-in-sessions-returns-wrong-HTTP-code)。</span><span class="sxs-lookup"><span data-stu-id="0dadf-135">This API has a [known issue](/graph/known-issues#revoke-sign-in-sessions-returns-wrong-HTTP-code).</span></span> <span data-ttu-id="0dadf-136">它返回不同的 HTTP 响应代码。</span><span class="sxs-lookup"><span data-stu-id="0dadf-136">It returns a different HTTP response code.</span></span>

## <a name="example"></a><span data-ttu-id="0dadf-137">示例</span><span class="sxs-lookup"><span data-stu-id="0dadf-137">Example</span></span>
<span data-ttu-id="0dadf-138">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="0dadf-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="0dadf-139">请求</span><span class="sxs-lookup"><span data-stu-id="0dadf-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="0dadf-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="0dadf-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_revokesigninsessionss"
}-->
```http
POST https://graph.microsoft.com/beta/me/revokeSignInSessions
```
# <a name="c"></a>[<span data-ttu-id="0dadf-141">C#</span><span class="sxs-lookup"><span data-stu-id="0dadf-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-revokesigninsessionss-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0dadf-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0dadf-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-revokesigninsessionss-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0dadf-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0dadf-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-revokesigninsessionss-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0dadf-144">响应</span><span class="sxs-lookup"><span data-stu-id="0dadf-144">Response</span></span>
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
