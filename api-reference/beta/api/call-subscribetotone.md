---
title: '调用: subscribeToTone'
description: 订阅 DTMF (双音多频信号)。 这样, 当用户在 "按键电话" 上按下按键时, 您就会收到通知。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f3fe078965877204b767b689ace293c3d4f46a9d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461251"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="2bcb2-104">调用: subscribeToTone</span><span class="sxs-lookup"><span data-stu-id="2bcb2-104">call: subscribeToTone</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2bcb2-105">订阅 DTMF (双音多频信号)。</span><span class="sxs-lookup"><span data-stu-id="2bcb2-105">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="2bcb2-106">这样, 你就可以在用户按 "按键时" 电话上的键时收到通知。</span><span class="sxs-lookup"><span data-stu-id="2bcb2-106">This allows you to be notified when the user presses keys on a "touchtone" phone.</span></span>

## <a name="permissions"></a><span data-ttu-id="2bcb2-107">权限</span><span class="sxs-lookup"><span data-stu-id="2bcb2-107">Permissions</span></span>
<span data-ttu-id="2bcb2-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2bcb2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2bcb2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2bcb2-110">Permission type</span></span> | <span data-ttu-id="2bcb2-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2bcb2-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="2bcb2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2bcb2-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="2bcb2-113">不支持</span><span class="sxs-lookup"><span data-stu-id="2bcb2-113">Not Supported</span></span>        |
| <span data-ttu-id="2bcb2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2bcb2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2bcb2-115">不支持</span><span class="sxs-lookup"><span data-stu-id="2bcb2-115">Not Supported</span></span>        |
| <span data-ttu-id="2bcb2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2bcb2-116">Application</span></span>     | <span data-ttu-id="2bcb2-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="2bcb2-117">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="2bcb2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2bcb2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/subscribeToTone
POST /applications/{id}/calls/{id}/subscribeToTone
```

## <a name="request-headers"></a><span data-ttu-id="2bcb2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2bcb2-119">Request headers</span></span>
| <span data-ttu-id="2bcb2-120">名称</span><span class="sxs-lookup"><span data-stu-id="2bcb2-120">Name</span></span>          | <span data-ttu-id="2bcb2-121">说明</span><span class="sxs-lookup"><span data-stu-id="2bcb2-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="2bcb2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2bcb2-122">Authorization</span></span> | <span data-ttu-id="2bcb2-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2bcb2-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2bcb2-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="2bcb2-125">Request body</span></span>
<span data-ttu-id="2bcb2-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="2bcb2-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2bcb2-127">参数</span><span class="sxs-lookup"><span data-stu-id="2bcb2-127">Parameter</span></span>      | <span data-ttu-id="2bcb2-128">类型</span><span class="sxs-lookup"><span data-stu-id="2bcb2-128">Type</span></span>    | <span data-ttu-id="2bcb2-129">说明</span><span class="sxs-lookup"><span data-stu-id="2bcb2-129">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="2bcb2-130">适用</span><span class="sxs-lookup"><span data-stu-id="2bcb2-130">clientContext</span></span>  | <span data-ttu-id="2bcb2-131">字符串</span><span class="sxs-lookup"><span data-stu-id="2bcb2-131">String</span></span>  | <span data-ttu-id="2bcb2-132">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="2bcb2-132">The client context.</span></span> |

## <a name="response"></a><span data-ttu-id="2bcb2-133">响应</span><span class="sxs-lookup"><span data-stu-id="2bcb2-133">Response</span></span>
<span data-ttu-id="2bcb2-134">返回`202 Accepted`响应代码和位置标头, 其中包含为此请求创建的[commsOperation](../resources/commsoperation.md)的 uri。</span><span class="sxs-lookup"><span data-stu-id="2bcb2-134">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="2bcb2-135">示例</span><span class="sxs-lookup"><span data-stu-id="2bcb2-135">Example</span></span>
<span data-ttu-id="2bcb2-136">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="2bcb2-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="2bcb2-137">请求</span><span class="sxs-lookup"><span data-stu-id="2bcb2-137">Request</span></span>
<span data-ttu-id="2bcb2-138">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="2bcb2-138">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-subscribeToTone"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/subscribeToTone
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="response"></a><span data-ttu-id="2bcb2-139">响应</span><span class="sxs-lookup"><span data-stu-id="2bcb2-139">Response</span></span>

> <span data-ttu-id="2bcb2-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2bcb2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="2bcb2-142">通知-操作已完成</span><span class="sxs-lookup"><span data-stu-id="2bcb2-142">Notification - operation completed</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "status": "completed"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: subscribeToTone",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-subscribetotone.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
