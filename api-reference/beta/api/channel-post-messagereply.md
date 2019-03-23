---
title: 在渠道中回复消息
description: 在渠道中回复现有消息。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 15e1bfffe7d7634092937a0605debfd5294b142b
ms.sourcegitcommit: 3615f9475d57bfbb3a8c4402af863897f592dfbd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2019
ms.locfileid: "30789674"
---
# <a name="reply-to-a-message-in-a-channel"></a><span data-ttu-id="5e657-103">在渠道中回复消息</span><span class="sxs-lookup"><span data-stu-id="5e657-103">Reply to a message in a channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e657-104">在指定的[频道](../resources/channel.md)中创建对[邮件](../resources/chatmessage.md)的新答复。</span><span class="sxs-lookup"><span data-stu-id="5e657-104">Create a new reply to a [message](../resources/chatmessage.md) in a specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5e657-105">权限</span><span class="sxs-lookup"><span data-stu-id="5e657-105">Permissions</span></span>
<span data-ttu-id="5e657-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5e657-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e657-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5e657-108">Permission type</span></span>      | <span data-ttu-id="5e657-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5e657-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e657-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5e657-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5e657-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e657-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5e657-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5e657-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e657-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e657-113">Not supported.</span></span>    |
|<span data-ttu-id="5e657-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="5e657-114">Application</span></span> | <span data-ttu-id="5e657-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e657-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e657-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5e657-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages/{id}/replies
```
## <a name="request-headers"></a><span data-ttu-id="5e657-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="5e657-117">Request headers</span></span>
| <span data-ttu-id="5e657-118">名称</span><span class="sxs-lookup"><span data-stu-id="5e657-118">Name</span></span>       | <span data-ttu-id="5e657-119">类型</span><span class="sxs-lookup"><span data-stu-id="5e657-119">Type</span></span> | <span data-ttu-id="5e657-120">说明</span><span class="sxs-lookup"><span data-stu-id="5e657-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5e657-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e657-121">Authorization</span></span>  | <span data-ttu-id="5e657-122">string</span><span class="sxs-lookup"><span data-stu-id="5e657-122">string</span></span>  | <span data-ttu-id="5e657-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5e657-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5e657-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="5e657-125">Request body</span></span>
<span data-ttu-id="5e657-126">在请求正文中, 提供[message](../resources/chatmessage.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e657-126">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="5e657-127">只有 body 属性是必需的, 其他属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="5e657-127">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="5e657-128">响应</span><span class="sxs-lookup"><span data-stu-id="5e657-128">Response</span></span>

<span data-ttu-id="5e657-129">如果成功, 此方法将`201 Created`在已创建的[邮件](../resources/chatmessage.md)中返回响应代码。</span><span class="sxs-lookup"><span data-stu-id="5e657-129">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="example"></a><span data-ttu-id="5e657-130">示例</span><span class="sxs-lookup"><span data-stu-id="5e657-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5e657-131">请求</span><span class="sxs-lookup"><span data-stu-id="5e657-131">Request</span></span>
<span data-ttu-id="5e657-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5e657-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_reply_message"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}/replies
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World"
  }
}
```

##### <a name="response"></a><span data-ttu-id="5e657-133">响应</span><span class="sxs-lookup"><span data-stu-id="5e657-133">Response</span></span>

<span data-ttu-id="5e657-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5e657-134">Here is an example of the response.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages('id-value')/replies/$entity",
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
    "Error: /api-reference/beta/api/channel-post-reply_chatmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
