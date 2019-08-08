---
title: '用户: revokeSignInSessions'
description: 通过将**signInSessionsValidFromDateTime**用户属性重置为当前的日期时间来使向应用程序颁发的所有用户的刷新令牌失效 (以及用户浏览器中的会话 cookie)。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 72ac7892537799dce8259b226aea077e0e138596
ms.sourcegitcommit: eb5f63deafcdd6db44e791f2d1f4c46604ab06fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/07/2019
ms.locfileid: "36245568"
---
# <a name="user-revokesigninsessions"></a><span data-ttu-id="a9788-103">用户: revokeSignInSessions</span><span class="sxs-lookup"><span data-stu-id="a9788-103">user: revokeSignInSessions</span></span>

<span data-ttu-id="a9788-104">通过将**signInSessionsValidFromDateTime**用户属性重置为当前的日期时间, 使向用户 (以及用户浏览器中的会话 cookie) 发出的所有刷新令牌失效。</span><span class="sxs-lookup"><span data-stu-id="a9788-104">Invalidates all the refresh tokens issued to applications for a user (as well as session cookies in a user's browser), by resetting the **signInSessionsValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="a9788-105">通常, 如果用户有丢失或被盗的设备, 则执行此操作 (由用户或管理员执行)。</span><span class="sxs-lookup"><span data-stu-id="a9788-105">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span> <span data-ttu-id="a9788-106">此操作通过要求用户再次登录到之前已同意的所有应用程序 (独立于设备) 来阻止对组织中的应用程序的数据的访问。</span><span class="sxs-lookup"><span data-stu-id="a9788-106">This operation prevents access to the organization's data through applications on the device by requiring the user to sign in again to all applications that they have previously consented to, independent of device.</span></span>

><span data-ttu-id="a9788-107">如果应用程序尝试使用无效刷新令牌兑换此用户的委派访问令牌, 应用程序将收到错误。</span><span class="sxs-lookup"><span data-stu-id="a9788-107">If the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="a9788-108">如果发生这种情况, 应用程序将需要通过向授权终结点发出请求来获取新的刷新令牌, 这将强制用户登录。</span><span class="sxs-lookup"><span data-stu-id="a9788-108">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

>[!NOTE]
><span data-ttu-id="a9788-109">在调用**revokeSignInSessions**后, 可能会有几分钟的短暂延迟才会被吊销令牌。</span><span class="sxs-lookup"><span data-stu-id="a9788-109">After calling **revokeSignInSessions**, there might be a small delay of a few minutes before tokens are revoked.</span></span>

## <a name="permissions"></a><span data-ttu-id="a9788-110">权限</span><span class="sxs-lookup"><span data-stu-id="a9788-110">Permissions</span></span>

<span data-ttu-id="a9788-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a9788-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9788-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="a9788-113">Permission type</span></span>                        | <span data-ttu-id="a9788-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a9788-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9788-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a9788-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="a9788-116">Directory.accessasuser.all 的所有用户的读写。</span><span class="sxs-lookup"><span data-stu-id="a9788-116">User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="a9788-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a9788-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9788-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9788-118">Not supported.</span></span> |
|<span data-ttu-id="a9788-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="a9788-119">Application</span></span>                            | <span data-ttu-id="a9788-120">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a9788-120">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9788-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a9788-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/revokeSignInSessions
POST /users/{id | userPrincipalName}/revokeSignInSessions
```

## <a name="request-headers"></a><span data-ttu-id="a9788-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="a9788-122">Request headers</span></span>
| <span data-ttu-id="a9788-123">标头</span><span class="sxs-lookup"><span data-stu-id="a9788-123">Header</span></span>       | <span data-ttu-id="a9788-124">值</span><span class="sxs-lookup"><span data-stu-id="a9788-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a9788-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9788-125">Authorization</span></span>  | <span data-ttu-id="a9788-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a9788-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a9788-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a9788-128">Request body</span></span>
<span data-ttu-id="a9788-129">此操作没有请求内容。</span><span class="sxs-lookup"><span data-stu-id="a9788-129">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="a9788-130">响应</span><span class="sxs-lookup"><span data-stu-id="a9788-130">Response</span></span>

<span data-ttu-id="a9788-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a9788-131">If successful, this method returns a `204 No Content` response code.</span></span>

>[!NOTE]
><span data-ttu-id="a9788-132">此 API 存在[已知问题](/graph/concepts/known-issues.md#revoke-sign-in-sessions-returns-wrong-HTTP-code)。</span><span class="sxs-lookup"><span data-stu-id="a9788-132">This API has a [known issue](/graph/concepts/known-issues.md#revoke-sign-in-sessions-returns-wrong-HTTP-code).</span></span> <span data-ttu-id="a9788-133">它返回不同的 HTTP 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a9788-133">It returns a different HTTP response code.</span></span>

## <a name="example"></a><span data-ttu-id="a9788-134">示例</span><span class="sxs-lookup"><span data-stu-id="a9788-134">Example</span></span>
<span data-ttu-id="a9788-135">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="a9788-135">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="a9788-136">请求</span><span class="sxs-lookup"><span data-stu-id="a9788-136">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a9788-137">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="a9788-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_revokesigninsessionss"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/revokeSignInSessions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a9788-138">C#</span><span class="sxs-lookup"><span data-stu-id="a9788-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-revokesigninsessionss-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a9788-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="a9788-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-revokesigninsessionss-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a9788-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="a9788-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-revokesigninsessionss-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a9788-141">Java</span><span class="sxs-lookup"><span data-stu-id="a9788-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-revokesigninsessionss-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a9788-142">响应</span><span class="sxs-lookup"><span data-stu-id="a9788-142">Response</span></span>
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
