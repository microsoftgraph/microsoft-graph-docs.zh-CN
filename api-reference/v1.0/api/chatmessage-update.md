---
title: 更新 chatMessage
description: 更新 chatMessage 的 policyViolation 属性。
author: laujan
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 06ceb5aae99955062c9d409eb69dac5fdef0d6d9
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515602"
---
# <a name="update-chatmessage"></a><span data-ttu-id="0668f-103">更新 chatMessage</span><span class="sxs-lookup"><span data-stu-id="0668f-103">Update chatMessage</span></span>

<span data-ttu-id="0668f-104">更新 [chatMessage](../resources/chatMessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0668f-104">Update a [chatMessage](../resources/chatMessage.md) object.</span></span> <span data-ttu-id="0668f-105">只能 **更新 chatMessage** 的 **policyViolation** 属性。</span><span class="sxs-lookup"><span data-stu-id="0668f-105">Only the **policyViolation** property of a **chatMessage** can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="0668f-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="0668f-106">Permissions</span></span>

<span data-ttu-id="0668f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0668f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0668f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0668f-109">Permission type</span></span>      | <span data-ttu-id="0668f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0668f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0668f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0668f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0668f-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="0668f-112">Not supported.</span></span> |
|<span data-ttu-id="0668f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0668f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0668f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0668f-114">Not supported.</span></span>    |
|<span data-ttu-id="0668f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0668f-115">Application</span></span> | <span data-ttu-id="0668f-116">Chat.UpdatePolicyViolation.All 用于聊天消息。</span><span class="sxs-lookup"><span data-stu-id="0668f-116">Chat.UpdatePolicyViolation.All for a chat message.</span></span></br><span data-ttu-id="0668f-117">ChannelMessage.UpdatePolicyViolation.All 用于频道消息。</span><span class="sxs-lookup"><span data-stu-id="0668f-117">ChannelMessage.UpdatePolicyViolation.All for a channel message.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0668f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0668f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/(team-id)/channels/{channel-id}/messages/{message-id}
```

## <a name="request-headers"></a><span data-ttu-id="0668f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0668f-119">Request headers</span></span>

| <span data-ttu-id="0668f-120">名称</span><span class="sxs-lookup"><span data-stu-id="0668f-120">Name</span></span>       | <span data-ttu-id="0668f-121">说明</span><span class="sxs-lookup"><span data-stu-id="0668f-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="0668f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0668f-122">Authorization</span></span>  | <span data-ttu-id="0668f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0668f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0668f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0668f-125">Content-Type</span></span> | <span data-ttu-id="0668f-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0668f-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0668f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="0668f-128">Request body</span></span>

<span data-ttu-id="0668f-129">在请求正文中，提供 [chatMessage](../resources/chatMessage.md) 对象的 JSON 表示形式，仅指定 **policyViolation** 属性。</span><span class="sxs-lookup"><span data-stu-id="0668f-129">In the request body, supply a JSON representation of a [chatMessage](../resources/chatMessage.md) object, specifying only the **policyViolation** property.</span></span>

## <a name="response"></a><span data-ttu-id="0668f-130">响应</span><span class="sxs-lookup"><span data-stu-id="0668f-130">Response</span></span>

<span data-ttu-id="0668f-131">如果成功，此方法将返回 `200 OK` 响应。</span><span class="sxs-lookup"><span data-stu-id="0668f-131">If successful, this method returns a `200 OK` response.</span></span>

## <a name="example"></a><span data-ttu-id="0668f-132">示例</span><span class="sxs-lookup"><span data-stu-id="0668f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="0668f-133">请求</span><span class="sxs-lookup"><span data-stu-id="0668f-133">Request</span></span>

<span data-ttu-id="0668f-134">下面是请求更新 Microsoft Teams 频道消息中的 **policyViolation** 属性的示例。</span><span class="sxs-lookup"><span data-stu-id="0668f-134">The following is an example of the request to update the **policyViolation** property on a Microsoft Teams channel message.</span></span>


# <a name="http"></a>[<span data-ttu-id="0668f-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="0668f-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chatMessage.PatchPolicyViolation.All"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/teams/e1234567-e123-4276-55555-6232b0e3a89a/channels/a7654321-e321-0000-0000-123b0e3a00a/messages/19%3Aa21b0b0c05194ebc9e30000000000f61%40thread.skype
Content-Type: application/json
Content-Length: 248

{
  "policyViolation": {
    "policyTip": {
      "generalText" : "This item has been blocked by the administrator.",
      "complianceUrl" : "https://contoso.com/dlp-policy-page",
      "matchedConditionDescriptions" : ["Credit Card Number"]
    },
    "verdictDetails" : "AllowOverrideWithoutJustification,AllowFalsePositiveOverride",
    "dlpAction" : "BlockAccess"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="0668f-136">C#</span><span class="sxs-lookup"><span data-stu-id="0668f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chatmessagepatchpolicyviolationall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0668f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0668f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chatmessagepatchpolicyviolationall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0668f-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0668f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chatmessagepatchpolicyviolationall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0668f-139">Java</span><span class="sxs-lookup"><span data-stu-id="0668f-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chatmessagepatchpolicyviolationall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="0668f-140">响应</span><span class="sxs-lookup"><span data-stu-id="0668f-140">Response</span></span>

<span data-ttu-id="0668f-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0668f-141">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatMessage.UpdatePolicyViolation.All",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
