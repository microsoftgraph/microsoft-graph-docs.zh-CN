---
title: 在通道中创建一条消息
description: 在指定的通道中创建一个新的邮件。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 891181c8797563fac6afb7862a27bd8b49628b5f
ms.sourcegitcommit: a4773239d8559899c3f9433b3073e250a56d2e04
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/13/2019
ms.locfileid: "30039552"
---
# <a name="create-a-message-in-a-channel"></a><span data-ttu-id="9cb19-103">在通道中创建一条消息</span><span class="sxs-lookup"><span data-stu-id="9cb19-103">Create a message in a channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cb19-104">在指定的[频道](../resources/channel.md)中创建一个新的[邮件](../resources/chatmessage.md)。</span><span class="sxs-lookup"><span data-stu-id="9cb19-104">Create a new [message](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9cb19-105">权限</span><span class="sxs-lookup"><span data-stu-id="9cb19-105">Permissions</span></span>
<span data-ttu-id="9cb19-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9cb19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cb19-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9cb19-108">Permission type</span></span>      | <span data-ttu-id="9cb19-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9cb19-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9cb19-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9cb19-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9cb19-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cb19-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9cb19-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9cb19-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9cb19-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9cb19-113">Not supported.</span></span>    |
|<span data-ttu-id="9cb19-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9cb19-114">Application</span></span> | <span data-ttu-id="9cb19-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9cb19-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9cb19-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9cb19-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="9cb19-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="9cb19-117">Request headers</span></span>
| <span data-ttu-id="9cb19-118">名称</span><span class="sxs-lookup"><span data-stu-id="9cb19-118">Name</span></span>       | <span data-ttu-id="9cb19-119">类型</span><span class="sxs-lookup"><span data-stu-id="9cb19-119">Type</span></span> | <span data-ttu-id="9cb19-120">说明</span><span class="sxs-lookup"><span data-stu-id="9cb19-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9cb19-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9cb19-121">Authorization</span></span>  | <span data-ttu-id="9cb19-122">string</span><span class="sxs-lookup"><span data-stu-id="9cb19-122">string</span></span>  | <span data-ttu-id="9cb19-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9cb19-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9cb19-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9cb19-125">Request body</span></span>
<span data-ttu-id="9cb19-126">在请求正文中，提供[message](../resources/chatmessage.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9cb19-126">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="9cb19-127">仅正文属性是必需的这是可选的其他属性。</span><span class="sxs-lookup"><span data-stu-id="9cb19-127">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="9cb19-128">响应</span><span class="sxs-lookup"><span data-stu-id="9cb19-128">Response</span></span>

<span data-ttu-id="9cb19-129">如果成功，此方法返回`201 Created`响应代码创建的[消息](../resources/chatmessage.md)。</span><span class="sxs-lookup"><span data-stu-id="9cb19-129">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="example"></a><span data-ttu-id="9cb19-130">示例</span><span class="sxs-lookup"><span data-stu-id="9cb19-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9cb19-131">请求</span><span class="sxs-lookup"><span data-stu-id="9cb19-131">Request</span></span>
<span data-ttu-id="9cb19-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9cb19-132">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="9cb19-133">响应</span><span class="sxs-lookup"><span data-stu-id="9cb19-133">Response</span></span>

<span data-ttu-id="9cb19-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9cb19-134">Here is an example of the response.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-post-chatmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
