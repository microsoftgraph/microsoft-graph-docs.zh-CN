---
title: 更新聊天
description: 更新聊天对象的属性。
author: bhartono
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b0b7fcccb3de2716aa30fdeb577ed3dc31ca99e6
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753916"
---
# <a name="update-chat"></a><span data-ttu-id="9200a-103">更新聊天</span><span class="sxs-lookup"><span data-stu-id="9200a-103">Update chat</span></span>
<span data-ttu-id="9200a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9200a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9200a-105">更新 [聊天对象的属性](../resources/chat.md) 。</span><span class="sxs-lookup"><span data-stu-id="9200a-105">Update the properties of a [chat](../resources/chat.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9200a-106">权限</span><span class="sxs-lookup"><span data-stu-id="9200a-106">Permissions</span></span>
<span data-ttu-id="9200a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9200a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9200a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9200a-109">Permission type</span></span>|<span data-ttu-id="9200a-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9200a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9200a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9200a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9200a-112">Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9200a-112">Chat.ReadWrite</span></span>|
|<span data-ttu-id="9200a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9200a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9200a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9200a-114">Not supported.</span></span> |
|<span data-ttu-id="9200a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9200a-115">Application</span></span> | <span data-ttu-id="9200a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9200a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9200a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9200a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /chats/{chat-id}
```

## <a name="request-headers"></a><span data-ttu-id="9200a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9200a-118">Request headers</span></span>
|<span data-ttu-id="9200a-119">名称</span><span class="sxs-lookup"><span data-stu-id="9200a-119">Name</span></span>|<span data-ttu-id="9200a-120">说明</span><span class="sxs-lookup"><span data-stu-id="9200a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9200a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9200a-121">Authorization</span></span>|<span data-ttu-id="9200a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9200a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9200a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9200a-124">Content-Type</span></span>|<span data-ttu-id="9200a-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="9200a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9200a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9200a-127">Request body</span></span>
<span data-ttu-id="9200a-128">在请求正文中，提供聊天对象的 JSON [表示形式](../resources/chat.md) 。</span><span class="sxs-lookup"><span data-stu-id="9200a-128">In the request body, supply a JSON representation of the [chat](../resources/chat.md) object.</span></span>

<span data-ttu-id="9200a-129">下表显示了可用于此操作的属性。</span><span class="sxs-lookup"><span data-stu-id="9200a-129">The following table shows the properties that can be used with this action.</span></span>

|<span data-ttu-id="9200a-130">属性</span><span class="sxs-lookup"><span data-stu-id="9200a-130">Property</span></span>|<span data-ttu-id="9200a-131">类型</span><span class="sxs-lookup"><span data-stu-id="9200a-131">Type</span></span>|<span data-ttu-id="9200a-132">说明</span><span class="sxs-lookup"><span data-stu-id="9200a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9200a-133">topic</span><span class="sxs-lookup"><span data-stu-id="9200a-133">topic</span></span>|<span data-ttu-id="9200a-134">String</span><span class="sxs-lookup"><span data-stu-id="9200a-134">String</span></span>|<span data-ttu-id="9200a-135">聊天的标题。</span><span class="sxs-lookup"><span data-stu-id="9200a-135">The title of the chat.</span></span> <span data-ttu-id="9200a-136">只能为 chatType 值为 **的聊天设置** `group` 此值。</span><span class="sxs-lookup"><span data-stu-id="9200a-136">This can only be set for a chat with a **chatType** value of `group`.</span></span>|


## <a name="response"></a><span data-ttu-id="9200a-137">响应</span><span class="sxs-lookup"><span data-stu-id="9200a-137">Response</span></span>

<span data-ttu-id="9200a-138">如果成功，此方法在响应正文中返回 `200 OK response` 代码和更新的聊天资源。</span><span class="sxs-lookup"><span data-stu-id="9200a-138">If successful, this method returns a `200 OK response` code and the updated **chat** resource in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9200a-139">示例</span><span class="sxs-lookup"><span data-stu-id="9200a-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9200a-140">请求</span><span class="sxs-lookup"><span data-stu-id="9200a-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9200a-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="9200a-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chat"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/chats/19:1c5b01696d2e4a179c292bc9cf04e63b@thread.v2
Content-Type: application/json

{
    "topic": "Group chat title update",
}
```
# <a name="c"></a>[<span data-ttu-id="9200a-142">C#</span><span class="sxs-lookup"><span data-stu-id="9200a-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9200a-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9200a-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9200a-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9200a-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9200a-145">Java</span><span class="sxs-lookup"><span data-stu-id="9200a-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="9200a-146">响应</span><span class="sxs-lookup"><span data-stu-id="9200a-146">Response</span></span>
><span data-ttu-id="9200a-147">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9200a-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats/$entity",
    "id": "19:1c5b01696d2e4a179c292bc9cf04e63b@thread.v2",
    "topic": "Group chat title update",
    "createdDateTime": "2020-12-04T23:11:16.175Z",
    "lastUpdatedDateTime": "2020-12-04T23:12:19.943Z",
    "chatType": "group"
}
```

