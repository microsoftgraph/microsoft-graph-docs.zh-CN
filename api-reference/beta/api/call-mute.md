---
title: 呼叫：静音
description: 允许应用程序将其本身设为静音。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: d1c9093f6c86f11588b0758a80fdbe8682d6d216
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38005969"
---
# <a name="call-mute"></a><span data-ttu-id="9655a-103">呼叫：静音</span><span class="sxs-lookup"><span data-stu-id="9655a-103">call: mute</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9655a-104">允许应用程序将其本身设为静音。</span><span class="sxs-lookup"><span data-stu-id="9655a-104">Allows the application to mute itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="9655a-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="9655a-105">Permissions</span></span>
<span data-ttu-id="9655a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9655a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9655a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9655a-108">Permission type</span></span>                        | <span data-ttu-id="9655a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9655a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9655a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9655a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9655a-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="9655a-111">Not Supported.</span></span>                               |
| <span data-ttu-id="9655a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9655a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9655a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9655a-113">Not Supported.</span></span>                               |
| <span data-ttu-id="9655a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9655a-114">Application</span></span>                            | <span data-ttu-id="9655a-115">无。</span><span class="sxs-lookup"><span data-stu-id="9655a-115">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="9655a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9655a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/mute
POST /communications/calls/{id}/mute
```
> <span data-ttu-id="9655a-117">**注意：**`/app`路径已被弃用。</span><span class="sxs-lookup"><span data-stu-id="9655a-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="9655a-118">接下来，请使用`/communications`路径。</span><span class="sxs-lookup"><span data-stu-id="9655a-118">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9655a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9655a-119">Request headers</span></span>
| <span data-ttu-id="9655a-120">名称</span><span class="sxs-lookup"><span data-stu-id="9655a-120">Name</span></span>          | <span data-ttu-id="9655a-121">说明</span><span class="sxs-lookup"><span data-stu-id="9655a-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="9655a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9655a-122">Authorization</span></span> | <span data-ttu-id="9655a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9655a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9655a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9655a-125">Request body</span></span>
<span data-ttu-id="9655a-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="9655a-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9655a-127">参数</span><span class="sxs-lookup"><span data-stu-id="9655a-127">Parameter</span></span>      | <span data-ttu-id="9655a-128">类型</span><span class="sxs-lookup"><span data-stu-id="9655a-128">Type</span></span>    |<span data-ttu-id="9655a-129">说明</span><span class="sxs-lookup"><span data-stu-id="9655a-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9655a-130">适用</span><span class="sxs-lookup"><span data-stu-id="9655a-130">clientContext</span></span>|<span data-ttu-id="9655a-131">String</span><span class="sxs-lookup"><span data-stu-id="9655a-131">String</span></span>|<span data-ttu-id="9655a-132">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="9655a-132">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="9655a-133">响应</span><span class="sxs-lookup"><span data-stu-id="9655a-133">Response</span></span>
<span data-ttu-id="9655a-134">如果成功，此方法在`200 OK`响应正文中返回响应代码和[commsOperation](../resources/commsoperation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9655a-134">If successful, this method returns `200 OK` response code and a [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9655a-135">示例</span><span class="sxs-lookup"><span data-stu-id="9655a-135">Example</span></span>
<span data-ttu-id="9655a-136">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="9655a-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="9655a-137">请求</span><span class="sxs-lookup"><span data-stu-id="9655a-137">Request</span></span>
<span data-ttu-id="9655a-138">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="9655a-138">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9655a-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="9655a-139">HTTP</span></span>](#tab/http)
<!-- { 
  "blockType": "request", 
  "name": "call-mute" 
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/mute
Content-Type: application/json

{
  "clientContext": "clientContext-value"
}
```

# <a name="ctabcsharp"></a>[<span data-ttu-id="9655a-140">C#</span><span class="sxs-lookup"><span data-stu-id="9655a-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-mute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9655a-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9655a-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-mute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9655a-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9655a-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-mute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9655a-143">响应</span><span class="sxs-lookup"><span data-stu-id="9655a-143">Response</span></span>

> <span data-ttu-id="9655a-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9655a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span> 
 
<!-- { 
  "blockType": "response", 
  "truncated": true, 
  "@odata.type": "microsoft.graph.commsOperation" 
} --> 
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Content-Type: application/json
Content-Length: 259
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsOperation",
  "truncated": true
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsOperation",
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#commsOperation",
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "clientContext": "clientContext-value"
}
```

##### <a name="notification---roster-updated-with-participant-muted"></a><span data-ttu-id="9655a-146">通知-名单在参与者静音时更新</span><span class="sxs-lookup"><span data-stu-id="9655a-146">Notification - roster updated with participant muted</span></span>

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/participants",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "2765eb15-01f8-47c6-b12b-c32111a4a86f",
          "info": {
            "identity": {
              "user": {
                "displayName": "Bob",
                "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          },
          "mediaStreams": [
            {
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "1",
              "direction": "sendReceive"
            }
          ],
          "isMuted": true, // will be set to true on mute
          "isInLobby": false
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: mute",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
