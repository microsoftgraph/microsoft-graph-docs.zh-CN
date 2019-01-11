---
title: 用户： invalidateAllRefreshTokens
description: 使所有用户的刷新令牌颁发给应用程序 （以及用户的浏览器中的会话 cookie） 到当前日期时间重置**refreshTokensValidFromDateTime**用户属性失效。 通常情况下，执行此操作 （按用户或管理员） 如果用户具有丢失或被盗的设备。  此操作将阻止对任何用户首先需要再次登录的情况下访问通过设备上的应用程序的组织的数据访问。 实际上，此操作会强制用户再次登录的所有应用程序的这些以前同意，独立于设备。
localization_priority: Normal
ms.openlocfilehash: 4ece9866e703d47ab8f7b024496f92f30a4a14b8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858077"
---
# <a name="user-invalidateallrefreshtokens"></a><span data-ttu-id="54505-106">用户： invalidateAllRefreshTokens</span><span class="sxs-lookup"><span data-stu-id="54505-106">user: invalidateAllRefreshTokens</span></span>

> <span data-ttu-id="54505-107">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="54505-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="54505-108">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="54505-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="54505-109">使所有用户的刷新令牌颁发给应用程序 （以及用户的浏览器中的会话 cookie） 到当前日期时间重置**refreshTokensValidFromDateTime**用户属性失效。</span><span class="sxs-lookup"><span data-stu-id="54505-109">Invalidates all of the user's refresh tokens issued to applications (as well as session cookies in a user's browser), by resetting the **refreshTokensValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="54505-110">通常情况下，执行此操作 （按用户或管理员） 如果用户具有丢失或被盗的设备。</span><span class="sxs-lookup"><span data-stu-id="54505-110">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span>  <span data-ttu-id="54505-111">此操作将阻止对任何用户首先需要再次登录的情况下访问通过设备上的应用程序的组织的数据访问。</span><span class="sxs-lookup"><span data-stu-id="54505-111">This operation would prevent access to any of the organization's data accessed through applications on the device without the user first being required to sign in again.</span></span> <span data-ttu-id="54505-112">实际上，此操作会强制用户再次登录的所有应用程序的这些以前同意，独立于设备。</span><span class="sxs-lookup"><span data-stu-id="54505-112">In fact, this operation would force the user to sign in again for all applications that they have previously consented to, independent of device.</span></span>

<span data-ttu-id="54505-113">面向开发人员，如果应用程序尝试使用无效的刷新令牌，兑换为此用户的委派的访问令牌的应用程序将收到错误。</span><span class="sxs-lookup"><span data-stu-id="54505-113">For developers, if the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="54505-114">如果发生这种情况，应用程序需要获取新刷新令牌的授权终结点，则会强制用户登录向发出请求。</span><span class="sxs-lookup"><span data-stu-id="54505-114">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

## <a name="permissions"></a><span data-ttu-id="54505-115">权限</span><span class="sxs-lookup"><span data-stu-id="54505-115">Permissions</span></span>
<span data-ttu-id="54505-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="54505-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

+ <span data-ttu-id="54505-118">应用程序，以便在用户以使应用程序无效签名他们已同意： User.ReadWrite，Directory.ReadWrite.All，Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="54505-118">For an application to allow the signed in user to invalidate applications they've consented to: User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>
+ <span data-ttu-id="54505-119">要允许管理员使失效应用程序的应用程序的用户已同意： Directory.ReadWrite.All、 Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="54505-119">For an application to allow an administrator to invalidate applications a user has consented to: Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="54505-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="54505-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/invalidateAllRefreshTokens
POST /users/{id | userPrincipalName}/invalidateAllRefreshTokens
```
## <a name="request-headers"></a><span data-ttu-id="54505-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="54505-121">Request headers</span></span>
| <span data-ttu-id="54505-122">标头</span><span class="sxs-lookup"><span data-stu-id="54505-122">Header</span></span>       | <span data-ttu-id="54505-123">值</span><span class="sxs-lookup"><span data-stu-id="54505-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="54505-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="54505-124">Authorization</span></span>  | <span data-ttu-id="54505-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="54505-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="54505-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="54505-127">Request body</span></span>
<span data-ttu-id="54505-128">此操作不包含任何请求内容。</span><span class="sxs-lookup"><span data-stu-id="54505-128">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="54505-129">响应</span><span class="sxs-lookup"><span data-stu-id="54505-129">Response</span></span>

<span data-ttu-id="54505-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="54505-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="54505-131">示例</span><span class="sxs-lookup"><span data-stu-id="54505-131">Example</span></span>
<span data-ttu-id="54505-132">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="54505-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="54505-133">请求</span><span class="sxs-lookup"><span data-stu-id="54505-133">Request</span></span>
<span data-ttu-id="54505-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="54505-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_invalidateallrefreshtokens"
}-->
```http
POST https://graph.microsoft.com/beta/me/invalidateAllRefreshTokens
```

##### <a name="response"></a><span data-ttu-id="54505-135">响应</span><span class="sxs-lookup"><span data-stu-id="54505-135">Response</span></span>
<span data-ttu-id="54505-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="54505-136">Here is an example of the response.</span></span> 
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
  "description": "user: invalidateAllRefreshTokens",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
