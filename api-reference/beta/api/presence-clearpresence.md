---
title: presence： clearPresence
description: 清除用户的应用程序状态会话状态信息。
author: jsandoval-msft
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 984c7667ceb2a28de189230952e5333f273cce24
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208249"
---
# <a name="presence-clearpresence"></a><span data-ttu-id="110be-103">presence： clearPresence</span><span class="sxs-lookup"><span data-stu-id="110be-103">presence: clearPresence</span></span>

<span data-ttu-id="110be-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="110be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="110be-105">清除用户的应用程序状态会话。</span><span class="sxs-lookup"><span data-stu-id="110be-105">Clear the application's presence session for a user.</span></span> <span data-ttu-id="110be-106">如果它是用户的唯一状态会话，则用户状态将更改为 `Offline/Offline` 。</span><span class="sxs-lookup"><span data-stu-id="110be-106">If it is the user's only presence session, the user's presence will change to `Offline/Offline`.</span></span>

<span data-ttu-id="110be-107">有关状态会话的详细信息，请参阅 [状态：setPresence](presence-setpresence.md#presence-sessions)。</span><span class="sxs-lookup"><span data-stu-id="110be-107">For details about presences sessions, see [presence: setPresence](presence-setpresence.md#presence-sessions).</span></span>

## <a name="permissions"></a><span data-ttu-id="110be-108">权限</span><span class="sxs-lookup"><span data-stu-id="110be-108">Permissions</span></span>
<span data-ttu-id="110be-109">调用 API 需要以下权限。</span><span class="sxs-lookup"><span data-stu-id="110be-109">The following permission is required to call the API.</span></span> <span data-ttu-id="110be-110">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="110be-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="110be-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="110be-111">Permission type</span></span>                        | <span data-ttu-id="110be-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="110be-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="110be-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="110be-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="110be-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="110be-114">Not Supported.</span></span>                              |
| <span data-ttu-id="110be-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="110be-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="110be-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="110be-116">Not Supported.</span></span>                              |
| <span data-ttu-id="110be-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="110be-117">Application</span></span>                            | <span data-ttu-id="110be-118">Presence.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="110be-118">Presence.ReadWrite.All</span></span>                      |

## <a name="http-request"></a><span data-ttu-id="110be-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="110be-119">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{userId}/presence/clearPresence
```

## <a name="request-headers"></a><span data-ttu-id="110be-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="110be-120">Request headers</span></span>
| <span data-ttu-id="110be-121">名称</span><span class="sxs-lookup"><span data-stu-id="110be-121">Name</span></span>          | <span data-ttu-id="110be-122">说明</span><span class="sxs-lookup"><span data-stu-id="110be-122">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="110be-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="110be-123">Authorization</span></span> | <span data-ttu-id="110be-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="110be-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="110be-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="110be-126">Content-Type</span></span>  | <span data-ttu-id="110be-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="110be-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="110be-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="110be-129">Request body</span></span>

<span data-ttu-id="110be-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="110be-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="110be-131">参数</span><span class="sxs-lookup"><span data-stu-id="110be-131">Parameter</span></span> | <span data-ttu-id="110be-132">类型</span><span class="sxs-lookup"><span data-stu-id="110be-132">Type</span></span>   | <span data-ttu-id="110be-133">说明</span><span class="sxs-lookup"><span data-stu-id="110be-133">Description</span></span>                                   |
| :-------- | :----- | :-------------------------------------------- |
| <span data-ttu-id="110be-134">sessionId</span><span class="sxs-lookup"><span data-stu-id="110be-134">sessionId</span></span> | <span data-ttu-id="110be-135">字符串</span><span class="sxs-lookup"><span data-stu-id="110be-135">string</span></span> | <span data-ttu-id="110be-136">应用程序状态会话的 ID。</span><span class="sxs-lookup"><span data-stu-id="110be-136">The ID of the application's presence session.</span></span> |


> [!IMPORTANT]
> 
> <span data-ttu-id="110be-137">提供请求中应用程序 `sessionId` ID。</span><span class="sxs-lookup"><span data-stu-id="110be-137">Provide the ID of the application as `sessionId` in the request.</span></span>

## <a name="response"></a><span data-ttu-id="110be-138">响应</span><span class="sxs-lookup"><span data-stu-id="110be-138">Response</span></span>
<span data-ttu-id="110be-139">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="110be-139">If successful, this method returns a `200 OK` response code.</span></span>

<span data-ttu-id="110be-140">如果状态会话不存在，此方法将返回 响应 `404 NotFound` 代码。</span><span class="sxs-lookup"><span data-stu-id="110be-140">If the presence session doesn't exist, this method returns a `404 NotFound` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="110be-141">示例</span><span class="sxs-lookup"><span data-stu-id="110be-141">Examples</span></span>
<span data-ttu-id="110be-142">以下请求显示 ID 为 `22553876-f5ab-4529-bffb-cfe50aa89f87` 的用户清除其状态会话的应用程序 `fa8bf3dc-eca7-46b7-bad1-db199b62afc3` 。</span><span class="sxs-lookup"><span data-stu-id="110be-142">The following request shows the application with ID `22553876-f5ab-4529-bffb-cfe50aa89f87` that clears its presence session for user `fa8bf3dc-eca7-46b7-bad1-db199b62afc3`.</span></span>

### <a name="request"></a><span data-ttu-id="110be-143">请求</span><span class="sxs-lookup"><span data-stu-id="110be-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="110be-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="110be-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "clear--presence"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/users/fa8bf3dc-eca7-46b7-bad1-db199b62afc3/presence/clearPresence
Content-Type: application/json

{
  "sessionId": "22553876-f5ab-4529-bffb-cfe50aa89f87"
}
```
# <a name="c"></a>[<span data-ttu-id="110be-145">C#</span><span class="sxs-lookup"><span data-stu-id="110be-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/clear--presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="110be-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="110be-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/clear--presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="110be-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="110be-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/clear--presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="110be-148">Java</span><span class="sxs-lookup"><span data-stu-id="110be-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/clear--presence-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="110be-149">响应</span><span class="sxs-lookup"><span data-stu-id="110be-149">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
