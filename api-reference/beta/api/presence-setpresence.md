---
title: presence： setPresence
description: 设置用户的应用程序状态会话状态信息。
author: jsandoval-msft
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 1e7e90b90ad92ca62327ad9c356fa1d870c7ecbd
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208280"
---
# <a name="presence-setpresence"></a><span data-ttu-id="62a66-103">presence： setPresence</span><span class="sxs-lookup"><span data-stu-id="62a66-103">presence: setPresence</span></span>

<span data-ttu-id="62a66-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62a66-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62a66-105">将用户的状态设置为应用程序状态。</span><span class="sxs-lookup"><span data-stu-id="62a66-105">Set the state of a user's presence session as an application.</span></span>

### <a name="presence-sessions"></a><span data-ttu-id="62a66-106">状态会话</span><span class="sxs-lookup"><span data-stu-id="62a66-106">Presence sessions</span></span>
<span data-ttu-id="62a66-107">用户可以具有多个状态会话，因为用户可以使用桌面、Teams和 web (多个) 。</span><span class="sxs-lookup"><span data-stu-id="62a66-107">A user can have multiple presence sessions because the user can be on multiple Teams clients (desktop, mobile, and web).</span></span> <span data-ttu-id="62a66-108">每个Teams客户端都有一个独立的状态会话，并且用户的状态是来自所有隐藏会话的聚合状态。</span><span class="sxs-lookup"><span data-stu-id="62a66-108">Each Teams client has an independent presence session and the user's presence is an aggregated state from all the sessions behind.</span></span>

<span data-ttu-id="62a66-109">同样，应用程序可以具有其自己的用户状态会话，并能够更新状态。</span><span class="sxs-lookup"><span data-stu-id="62a66-109">Similarly, an application can have its own presence session for a user and be able to update the state.</span></span>

<span data-ttu-id="62a66-110">以下是会话状态聚合方式的优先级：</span><span class="sxs-lookup"><span data-stu-id="62a66-110">The following is the precedence for how session states are aggregated:</span></span>
* <span data-ttu-id="62a66-111">用户配置>应用配置 (状态会覆盖其他用户) </span><span class="sxs-lookup"><span data-stu-id="62a66-111">User-configured > app-configured (user-configured state overrides others)</span></span>
* <span data-ttu-id="62a66-112">在已配置应用之间： (状态设置状态设置) >忙碌状态> DoNotDisturb >离开</span><span class="sxs-lookup"><span data-stu-id="62a66-112">Among app-configured: DoNotDisturb (currently not supported for set presence) > Busy > Available > Away</span></span>

### <a name="timeout-expiration-and-keep-alive"></a><span data-ttu-id="62a66-113">超时、到期并保持活动状态</span><span class="sxs-lookup"><span data-stu-id="62a66-113">Timeout, expiration, and keep alive</span></span>
<span data-ttu-id="62a66-114">状态会话 **可能会超时且\*\*\*\*过期**，因此应用程序需要在超时前调用此 API，以维护会话的状态;或过期 **之前，** 使会话保持活动状态。</span><span class="sxs-lookup"><span data-stu-id="62a66-114">A presence session may **time out** and **expire**, so the application needs to call this API before the **timeout**, to maintain the state for the session; or before the **expiration**, to keep the session alive.</span></span>

<span data-ttu-id="62a66-115">如果状态会话可用且超时为 5 分钟， `Available` 则状态会话可能会超时。</span><span class="sxs-lookup"><span data-stu-id="62a66-115">A presence session can time out if the availability is `Available` and the timeout is 5 minutes.</span></span> <span data-ttu-id="62a66-116">当状态淡出时，状态将逐渐淡出。</span><span class="sxs-lookup"><span data-stu-id="62a66-116">When it times out, the presence state fades in stages.</span></span> <span data-ttu-id="62a66-117">例如，如果应用程序将状态会话设置为 ，状态将在 5 分钟内更改为第一个超时，然后在另外 5 分钟（第二个超时） `Available/Available` `Available/AvailableInactive` `Away/Away` 中更改。</span><span class="sxs-lookup"><span data-stu-id="62a66-117">For example, if an application sets the presence session as `Available/Available`, the state would change to `Available/AvailableInactive` in 5 minutes with the first timeout, then `Away/Away` in another 5 minutes with the second timeout.</span></span>

<span data-ttu-id="62a66-118">状态会话的过期时间可用 参数 `expirationDuration` 进行配置。</span><span class="sxs-lookup"><span data-stu-id="62a66-118">The expiration of a presence session is configurable with the `expirationDuration` parameter.</span></span> <span data-ttu-id="62a66-119">当会话过期时，它将变为 `Offline` 。</span><span class="sxs-lookup"><span data-stu-id="62a66-119">When a session expires it becomes `Offline`.</span></span>

## <a name="permissions"></a><span data-ttu-id="62a66-120">权限</span><span class="sxs-lookup"><span data-stu-id="62a66-120">Permissions</span></span>
<span data-ttu-id="62a66-121">调用 API 需要以下权限。</span><span class="sxs-lookup"><span data-stu-id="62a66-121">The following permission is required to call the API.</span></span> <span data-ttu-id="62a66-122">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="62a66-122">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="62a66-123">权限类型</span><span class="sxs-lookup"><span data-stu-id="62a66-123">Permission type</span></span>                        | <span data-ttu-id="62a66-124">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="62a66-124">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="62a66-125">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="62a66-125">Delegated (work or school account)</span></span>     | <span data-ttu-id="62a66-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="62a66-126">Not Supported.</span></span>                              |
| <span data-ttu-id="62a66-127">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="62a66-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62a66-128">不支持。</span><span class="sxs-lookup"><span data-stu-id="62a66-128">Not Supported.</span></span>                              |
| <span data-ttu-id="62a66-129">应用程序</span><span class="sxs-lookup"><span data-stu-id="62a66-129">Application</span></span>                            | <span data-ttu-id="62a66-130">Presence.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62a66-130">Presence.ReadWrite.All</span></span>                      |

## <a name="http-request"></a><span data-ttu-id="62a66-131">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="62a66-131">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{userId}/presence/setPresence
```
## <a name="request-headers"></a><span data-ttu-id="62a66-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="62a66-132">Request headers</span></span>
| <span data-ttu-id="62a66-133">名称</span><span class="sxs-lookup"><span data-stu-id="62a66-133">Name</span></span>          | <span data-ttu-id="62a66-134">说明</span><span class="sxs-lookup"><span data-stu-id="62a66-134">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="62a66-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="62a66-135">Authorization</span></span> | <span data-ttu-id="62a66-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="62a66-p105">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="62a66-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="62a66-138">Content-Type</span></span>  | <span data-ttu-id="62a66-p106">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="62a66-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="62a66-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="62a66-141">Request body</span></span>

<span data-ttu-id="62a66-142">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="62a66-142">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="62a66-143">参数</span><span class="sxs-lookup"><span data-stu-id="62a66-143">Parameter</span></span>          | <span data-ttu-id="62a66-144">类型</span><span class="sxs-lookup"><span data-stu-id="62a66-144">Type</span></span>     | <span data-ttu-id="62a66-145">说明</span><span class="sxs-lookup"><span data-stu-id="62a66-145">Description</span></span>                                                                                            |
| :----------------- | :------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="62a66-146">sessionId</span><span class="sxs-lookup"><span data-stu-id="62a66-146">sessionId</span></span>          | <span data-ttu-id="62a66-147">字符串</span><span class="sxs-lookup"><span data-stu-id="62a66-147">string</span></span>   | <span data-ttu-id="62a66-148">应用程序状态会话的 ID。</span><span class="sxs-lookup"><span data-stu-id="62a66-148">The ID of the application's presence session.</span></span>                                                          |
| <span data-ttu-id="62a66-149">availability</span><span class="sxs-lookup"><span data-stu-id="62a66-149">availability</span></span>       | <span data-ttu-id="62a66-150">字符串</span><span class="sxs-lookup"><span data-stu-id="62a66-150">string</span></span>   | <span data-ttu-id="62a66-151">基本状态信息。</span><span class="sxs-lookup"><span data-stu-id="62a66-151">The base presence information.</span></span>                                                                         |
| <span data-ttu-id="62a66-152">活动</span><span class="sxs-lookup"><span data-stu-id="62a66-152">activity</span></span>           | <span data-ttu-id="62a66-153">字符串</span><span class="sxs-lookup"><span data-stu-id="62a66-153">string</span></span>   | <span data-ttu-id="62a66-154">可用性的补充信息。</span><span class="sxs-lookup"><span data-stu-id="62a66-154">The supplemental information to availability.</span></span>                                                          |
| <span data-ttu-id="62a66-155">expirationDuration</span><span class="sxs-lookup"><span data-stu-id="62a66-155">expirationDuration</span></span> | <span data-ttu-id="62a66-156">duration</span><span class="sxs-lookup"><span data-stu-id="62a66-156">duration</span></span> | <span data-ttu-id="62a66-157">应用状态会话的过期时间。</span><span class="sxs-lookup"><span data-stu-id="62a66-157">The expiration of the app presence session.</span></span> <span data-ttu-id="62a66-158">该值以 ISO 8601 格式表示持续时间。</span><span class="sxs-lookup"><span data-stu-id="62a66-158">The value is represented in ISO 8601 format for durations.</span></span> |

> [!IMPORTANT]
>
> <span data-ttu-id="62a66-159">提供请求中应用程序 `sessionId` ID。</span><span class="sxs-lookup"><span data-stu-id="62a66-159">Provide the ID of the application as `sessionId` in the request.</span></span>

<span data-ttu-id="62a66-160">支持的 和 `availability` `activity` 的组合包括：</span><span class="sxs-lookup"><span data-stu-id="62a66-160">Supported combinations of `availability` and `activity` are:</span></span>

| <span data-ttu-id="62a66-161">availability</span><span class="sxs-lookup"><span data-stu-id="62a66-161">availability</span></span> | <span data-ttu-id="62a66-162">活动</span><span class="sxs-lookup"><span data-stu-id="62a66-162">activity</span></span>          | <span data-ttu-id="62a66-163">说明</span><span class="sxs-lookup"><span data-stu-id="62a66-163">Description</span></span>                                              |
| :----------- | :---------------- | :------------------------------------------------------- |
| <span data-ttu-id="62a66-164">可用</span><span class="sxs-lookup"><span data-stu-id="62a66-164">Available</span></span>    | <span data-ttu-id="62a66-165">可用</span><span class="sxs-lookup"><span data-stu-id="62a66-165">Available</span></span>         | <span data-ttu-id="62a66-166">将状态会话更新为"可用"。</span><span class="sxs-lookup"><span data-stu-id="62a66-166">Updates the presence session as Available.</span></span>               |
| <span data-ttu-id="62a66-167">忙碌</span><span class="sxs-lookup"><span data-stu-id="62a66-167">Busy</span></span>         | <span data-ttu-id="62a66-168">InACall</span><span class="sxs-lookup"><span data-stu-id="62a66-168">InACall</span></span>           | <span data-ttu-id="62a66-169">将状态会话更新为 Busy、InACall。</span><span class="sxs-lookup"><span data-stu-id="62a66-169">Updates the presence session as Busy, InACall.</span></span>           |
| <span data-ttu-id="62a66-170">忙碌</span><span class="sxs-lookup"><span data-stu-id="62a66-170">Busy</span></span>         | <span data-ttu-id="62a66-171">InAConferenceCall</span><span class="sxs-lookup"><span data-stu-id="62a66-171">InAConferenceCall</span></span> | <span data-ttu-id="62a66-172">将状态会话更新为 Busy、InAConferenceCall。</span><span class="sxs-lookup"><span data-stu-id="62a66-172">Updates the presence session as Busy, InAConferenceCall.</span></span> |
| <span data-ttu-id="62a66-173">离开</span><span class="sxs-lookup"><span data-stu-id="62a66-173">Away</span></span>         | <span data-ttu-id="62a66-174">离开</span><span class="sxs-lookup"><span data-stu-id="62a66-174">Away</span></span>              | <span data-ttu-id="62a66-175">将状态会话更新为离开。</span><span class="sxs-lookup"><span data-stu-id="62a66-175">Updates the presence session as Away.</span></span>                    |

## <a name="response"></a><span data-ttu-id="62a66-176">响应</span><span class="sxs-lookup"><span data-stu-id="62a66-176">Response</span></span>
<span data-ttu-id="62a66-177">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="62a66-177">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="62a66-178">示例</span><span class="sxs-lookup"><span data-stu-id="62a66-178">Examples</span></span>
<span data-ttu-id="62a66-179">以下请求显示 ID 为 `22553876-f5ab-4529-bffb-cfe50aa89f87` 用户设置其状态会话的应用程序 `fa8bf3dc-eca7-46b7-bad1-db199b62afc3` 。</span><span class="sxs-lookup"><span data-stu-id="62a66-179">The following request shows the application with ID `22553876-f5ab-4529-bffb-cfe50aa89f87` that sets its presence session for user `fa8bf3dc-eca7-46b7-bad1-db199b62afc3`.</span></span>

### <a name="request"></a><span data-ttu-id="62a66-180">请求</span><span class="sxs-lookup"><span data-stu-id="62a66-180">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="62a66-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="62a66-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "set-presence"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/users/fa8bf3dc-eca7-46b7-bad1-db199b62afc3/presence/setPresence
Content-Type: application/json

{
  "sessionId": "22553876-f5ab-4529-bffb-cfe50aa89f87",
  "availability": "Available",
  "activity": "Available",
  "expirationDuration": "PT1H"
}
```
# <a name="c"></a>[<span data-ttu-id="62a66-182">C#</span><span class="sxs-lookup"><span data-stu-id="62a66-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/set-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="62a66-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62a66-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/set-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="62a66-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62a66-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/set-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="62a66-185">Java</span><span class="sxs-lookup"><span data-stu-id="62a66-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/set-presence-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="62a66-186">响应</span><span class="sxs-lookup"><span data-stu-id="62a66-186">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
