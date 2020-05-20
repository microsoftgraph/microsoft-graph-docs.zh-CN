---
title: 答复频道中的邮件
description: 在渠道中回复现有消息。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 42ca21f34dac869a8686e0f14beb13ee8df17db1
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289726"
---
# <a name="reply-to-a-message-in-a-channel"></a><span data-ttu-id="aae36-103">答复频道中的邮件</span><span class="sxs-lookup"><span data-stu-id="aae36-103">Reply to a message in a channel</span></span>

<span data-ttu-id="aae36-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aae36-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aae36-105">在指定的[频道](../resources/channel.md)中创建对[邮件](../resources/chatmessage.md)的新答复。</span><span class="sxs-lookup"><span data-stu-id="aae36-105">Create a new reply to a [message](../resources/chatmessage.md) in a specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="aae36-106">**注意**：我们建议您不要使用此 API 进行数据迁移。</span><span class="sxs-lookup"><span data-stu-id="aae36-106">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="aae36-107">它不具有典型迁移所需的吞吐量。</span><span class="sxs-lookup"><span data-stu-id="aae36-107">It does not have the throughput necessary for a typical migration.</span></span>

## <a name="permissions"></a><span data-ttu-id="aae36-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="aae36-108">Permissions</span></span>

<span data-ttu-id="aae36-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aae36-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aae36-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="aae36-111">Permission type</span></span>      | <span data-ttu-id="aae36-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aae36-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aae36-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aae36-113">Delegated (work or school account)</span></span> | <span data-ttu-id="aae36-114">ChannelMessage、Group、Group 写。 All</span><span class="sxs-lookup"><span data-stu-id="aae36-114">ChannelMessage.Send, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="aae36-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aae36-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aae36-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="aae36-116">Not supported.</span></span>    |
|<span data-ttu-id="aae36-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="aae36-117">Application</span></span> | <span data-ttu-id="aae36-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aae36-118">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aae36-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aae36-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages/{id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="aae36-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="aae36-120">Request headers</span></span>

| <span data-ttu-id="aae36-121">名称</span><span class="sxs-lookup"><span data-stu-id="aae36-121">Name</span></span>       | <span data-ttu-id="aae36-122">类型</span><span class="sxs-lookup"><span data-stu-id="aae36-122">Type</span></span> | <span data-ttu-id="aae36-123">说明</span><span class="sxs-lookup"><span data-stu-id="aae36-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="aae36-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="aae36-124">Authorization</span></span>  | <span data-ttu-id="aae36-125">string</span><span class="sxs-lookup"><span data-stu-id="aae36-125">string</span></span>  | <span data-ttu-id="aae36-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aae36-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aae36-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="aae36-128">Request body</span></span>

<span data-ttu-id="aae36-129">在请求正文中，提供[message](../resources/chatmessage.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aae36-129">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="aae36-130">只有 body 属性是必需的，其他属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="aae36-130">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="aae36-131">响应</span><span class="sxs-lookup"><span data-stu-id="aae36-131">Response</span></span>

<span data-ttu-id="aae36-132">如果成功，此方法 `201 Created` 将在已创建的[邮件](../resources/chatmessage.md)中返回响应代码。</span><span class="sxs-lookup"><span data-stu-id="aae36-132">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="example"></a><span data-ttu-id="aae36-133">示例</span><span class="sxs-lookup"><span data-stu-id="aae36-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="aae36-134">请求</span><span class="sxs-lookup"><span data-stu-id="aae36-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "post_reply_message"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/messages/{id}/replies
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World"
  }
}
```
### <a name="response"></a><span data-ttu-id="aae36-135">响应</span><span class="sxs-lookup"><span data-stu-id="aae36-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 160

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages('id-value')/replies/$entity",
    "id": "id-value",
    "replyToId": null,
    "etag": "id-value",
    "messageType": "message",
    "createdDateTime": "2019-02-04T19:58:15.511Z",
    "lastModifiedDateTime": null,
    "deleted": false,
    "subject": null,
    "summary": null,
    "importance": "normal",
    "locale": "en-us",
    "policyViolation": null,
    "from": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "id-value",
            "displayName": "Joh Doe",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "html",
        "content": "Hello World"
    },
    "attachments": [],
    "mentions": [],
    "reactions": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create a reply message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
