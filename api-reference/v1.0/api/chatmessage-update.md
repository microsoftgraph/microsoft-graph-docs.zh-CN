---
title: 更新了 chatmessage
description: 更新了 chatmessage 的 policyViolation 属性。
author: laujan
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b36f02ec2193bfc1eda1706265fa1392b04a4e70
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223939"
---
# <a name="update-chatmessage"></a><span data-ttu-id="4b754-103">更新了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="4b754-103">Update chatMessage</span></span>

<span data-ttu-id="4b754-104">更新 [了 chatmessage](../resources/chatMessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4b754-104">Update a [chatMessage](../resources/chatMessage.md) object.</span></span> <span data-ttu-id="4b754-105">仅**了 chatmessage**的**policyViolation**属性可以进行更新。</span><span class="sxs-lookup"><span data-stu-id="4b754-105">Only the **policyViolation** property of a **chatMessage** can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b754-106">权限</span><span class="sxs-lookup"><span data-stu-id="4b754-106">Permissions</span></span>

<span data-ttu-id="4b754-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4b754-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b754-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4b754-109">Permission type</span></span>      | <span data-ttu-id="4b754-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4b754-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b754-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4b754-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4b754-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b754-112">Not supported.</span></span>    |
|<span data-ttu-id="4b754-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4b754-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b754-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b754-114">Not supported.</span></span>    |
|<span data-ttu-id="4b754-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4b754-115">Application</span></span> | <span data-ttu-id="4b754-116">聊天消息的 UpdatePolicyViolation。</span><span class="sxs-lookup"><span data-stu-id="4b754-116">Chat.UpdatePolicyViolation.All for a chat message.</span></span></br><span data-ttu-id="4b754-117">ChannelMessage 通道邮件的所有 UpdatePolicyViolation。</span><span class="sxs-lookup"><span data-stu-id="4b754-117">ChannelMessage.UpdatePolicyViolation.All for a channel message.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b754-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4b754-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/(team-id)/channels/{channel-id}/chatMessages/{message-id}
PATCH /users/(user-id)/chats/{chatThread-id}/chatMessages/{message-id}
```

## <a name="request-headers"></a><span data-ttu-id="4b754-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4b754-119">Request headers</span></span>

| <span data-ttu-id="4b754-120">名称</span><span class="sxs-lookup"><span data-stu-id="4b754-120">Name</span></span>       | <span data-ttu-id="4b754-121">说明</span><span class="sxs-lookup"><span data-stu-id="4b754-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="4b754-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b754-122">Authorization</span></span>  | <span data-ttu-id="4b754-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4b754-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4b754-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4b754-125">Content-Type</span></span> | <span data-ttu-id="4b754-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="4b754-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b754-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="4b754-128">Request body</span></span>

<span data-ttu-id="4b754-129">在请求正文中，提供 [了 chatmessage](../resources/chatMessage.md) 对象的 JSON 表示形式，仅指定 **policyViolation** 属性。</span><span class="sxs-lookup"><span data-stu-id="4b754-129">In the request body, supply a JSON representation of a [chatMessage](../resources/chatMessage.md) object, specifying only the **policyViolation** property.</span></span>

## <a name="response"></a><span data-ttu-id="4b754-130">响应</span><span class="sxs-lookup"><span data-stu-id="4b754-130">Response</span></span>

<span data-ttu-id="4b754-131">如果成功，此方法将返回 `200 OK` 响应。</span><span class="sxs-lookup"><span data-stu-id="4b754-131">If successful, this method returns a `200 OK` response.</span></span>

## <a name="example"></a><span data-ttu-id="4b754-132">示例</span><span class="sxs-lookup"><span data-stu-id="4b754-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b754-133">请求</span><span class="sxs-lookup"><span data-stu-id="4b754-133">Request</span></span>

<span data-ttu-id="4b754-134">下面的示例演示了更新 Microsoft 团队频道消息上的 **policyViolation** 属性的请求。</span><span class="sxs-lookup"><span data-stu-id="4b754-134">The following is an example of the request to update the **policyViolation** property on a Microsoft Teams channel message.</span></span>

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

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="4b754-135">响应</span><span class="sxs-lookup"><span data-stu-id="4b754-135">Response</span></span>

<span data-ttu-id="4b754-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4b754-136">Here is an example of the response.</span></span>

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
