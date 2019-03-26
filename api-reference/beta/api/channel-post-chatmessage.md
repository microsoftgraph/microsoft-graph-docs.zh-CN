---
title: 在渠道中发送消息
description: 在指定的频道中发送新邮件。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 960c5d8164f2681b71bb2c3b46383bb210240bb2
ms.sourcegitcommit: 3410e1b8dcf62a7b0e4d6b11920912479f21feb2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/26/2019
ms.locfileid: "30799982"
---
# <a name="send-a-message-to-a-channel"></a><span data-ttu-id="16e3e-103">向渠道发送消息</span><span class="sxs-lookup"><span data-stu-id="16e3e-103">Send a message to a channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16e3e-104">在指定的[频道](../resources/channel.md)中创建新[邮件](../resources/chatmessage.md)。</span><span class="sxs-lookup"><span data-stu-id="16e3e-104">Create a new [message](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="16e3e-105">权限</span><span class="sxs-lookup"><span data-stu-id="16e3e-105">Permissions</span></span>
<span data-ttu-id="16e3e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="16e3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16e3e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="16e3e-108">Permission type</span></span>      | <span data-ttu-id="16e3e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="16e3e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16e3e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="16e3e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="16e3e-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16e3e-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="16e3e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="16e3e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16e3e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="16e3e-113">Not supported.</span></span>    |
|<span data-ttu-id="16e3e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="16e3e-114">Application</span></span> | <span data-ttu-id="16e3e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="16e3e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="16e3e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="16e3e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="16e3e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="16e3e-117">Request headers</span></span>
| <span data-ttu-id="16e3e-118">名称</span><span class="sxs-lookup"><span data-stu-id="16e3e-118">Name</span></span>       | <span data-ttu-id="16e3e-119">类型</span><span class="sxs-lookup"><span data-stu-id="16e3e-119">Type</span></span> | <span data-ttu-id="16e3e-120">说明</span><span class="sxs-lookup"><span data-stu-id="16e3e-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="16e3e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="16e3e-121">Authorization</span></span>  | <span data-ttu-id="16e3e-122">string</span><span class="sxs-lookup"><span data-stu-id="16e3e-122">string</span></span>  | <span data-ttu-id="16e3e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="16e3e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16e3e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="16e3e-125">Request body</span></span>
<span data-ttu-id="16e3e-126">在请求正文中, 提供[message](../resources/chatmessage.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="16e3e-126">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="16e3e-127">只有 body 属性是必需的, 其他属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="16e3e-127">Only the body property is mandatory, other properties are optional.</span></span>

> <span data-ttu-id="16e3e-128">注意: 不支持发送包含附件和图像的邮件。</span><span class="sxs-lookup"><span data-stu-id="16e3e-128">Note: Sending messages with attachments and images is not supported.</span></span>

## <a name="response"></a><span data-ttu-id="16e3e-129">响应</span><span class="sxs-lookup"><span data-stu-id="16e3e-129">Response</span></span>

<span data-ttu-id="16e3e-130">如果成功, 此方法将`201 Created`在已创建的[邮件](../resources/chatmessage.md)中返回响应代码。</span><span class="sxs-lookup"><span data-stu-id="16e3e-130">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="examples"></a><span data-ttu-id="16e3e-131">示例</span><span class="sxs-lookup"><span data-stu-id="16e3e-131">Examples</span></span> 

### <a name="example-1-hello-world"></a><span data-ttu-id="16e3e-132">示例 1: Hello World</span><span class="sxs-lookup"><span data-stu-id="16e3e-132">Example 1: Hello World</span></span>

##### <a name="request"></a><span data-ttu-id="16e3e-133">请求</span><span class="sxs-lookup"><span data-stu-id="16e3e-133">Request</span></span>
<span data-ttu-id="16e3e-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="16e3e-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World"
  }
}
```

##### <a name="response"></a><span data-ttu-id="16e3e-135">响应</span><span class="sxs-lookup"><span data-stu-id="16e3e-135">Response</span></span>

<span data-ttu-id="16e3e-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="16e3e-136">Here is an example of the response.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages/$entity",
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

### <a name="example-2-mentions"></a><span data-ttu-id="16e3e-137">示例 2: @mentions</span><span class="sxs-lookup"><span data-stu-id="16e3e-137">Example 2: @mentions</span></span>

##### <a name="request"></a><span data-ttu-id="16e3e-138">请求</span><span class="sxs-lookup"><span data-stu-id="16e3e-138">Request</span></span>
<span data-ttu-id="16e3e-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="16e3e-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World <at id=\"0\">Jane Smith</at>"
  },
  "mentions": [
    {
      "id": 0,
      "mentionText": "Jane Smith",
      "mentioned": {
        "user": {
          "displayName": "Jane Smith",
          "id": "ef1c916a-3135-4417-ba27-8eb7bd084193",
          "userIdentityType": "aadUser"
        }
      }
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="16e3e-140">响应</span><span class="sxs-lookup"><span data-stu-id="16e3e-140">Response</span></span>

<span data-ttu-id="16e3e-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="16e3e-141">Here is an example of the response.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages/$entity",
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
        "content": "Hello World <at id=\"0\">Jane Smith</at>"
    },
    "attachments": [],
    "mentions": [
        {
            "id": 0,
            "mentionText": "Jane Smith",
            "mentioned": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "ef1c916a-3135-4417-ba27-8eb7bd084193",
                    "displayName": "Jane Smith",
                    "userIdentityType": "aadUser"
                }
            }
        }
    ],
    "reactions": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Send message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-post-chatmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
