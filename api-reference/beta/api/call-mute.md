---
title: 呼叫：静音
description: 允许应用程序将其本身设为静音。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 7e2e1252a34d6efc6004aa78873a11139fece83f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987342"
---
# <a name="call-mute"></a><span data-ttu-id="46b5e-103">呼叫：静音</span><span class="sxs-lookup"><span data-stu-id="46b5e-103">call: mute</span></span>

<span data-ttu-id="46b5e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46b5e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46b5e-105">允许应用程序将其本身设为静音。</span><span class="sxs-lookup"><span data-stu-id="46b5e-105">Allows the application to mute itself.</span></span>

<span data-ttu-id="46b5e-106">这是一种服务器静音，这意味着服务器将丢弃此参与者的所有音频数据包，即使参与者继续传输音频也是如此。</span><span class="sxs-lookup"><span data-stu-id="46b5e-106">This is a server mute, meaning that the server will drop all audio packets for this participant, even if the participant continues to stream audio.</span></span>

<span data-ttu-id="46b5e-107">有关如何处理静音操作的更多详细信息，请参阅 [muteParticipantOperation](../resources/muteparticipantoperation.md)</span><span class="sxs-lookup"><span data-stu-id="46b5e-107">For more details about how to handle mute operations, see [muteParticipantOperation](../resources/muteparticipantoperation.md)</span></span>

> <span data-ttu-id="46b5e-108">**注意：** 仅组调用支持此方法。</span><span class="sxs-lookup"><span data-stu-id="46b5e-108">**Note:** This method is only supported for group calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="46b5e-109">权限</span><span class="sxs-lookup"><span data-stu-id="46b5e-109">Permissions</span></span>
<span data-ttu-id="46b5e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="46b5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="46b5e-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="46b5e-112">Permission type</span></span>                        | <span data-ttu-id="46b5e-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="46b5e-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="46b5e-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="46b5e-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="46b5e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="46b5e-115">Not Supported.</span></span>                               |
| <span data-ttu-id="46b5e-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="46b5e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46b5e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="46b5e-117">Not Supported.</span></span>                               |
| <span data-ttu-id="46b5e-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="46b5e-118">Application</span></span>                            | <span data-ttu-id="46b5e-119">无。</span><span class="sxs-lookup"><span data-stu-id="46b5e-119">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="46b5e-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="46b5e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/mute
POST /communications/calls/{id}/mute
```
> <span data-ttu-id="46b5e-121">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="46b5e-121">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="46b5e-122">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="46b5e-122">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="46b5e-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="46b5e-123">Request headers</span></span>
| <span data-ttu-id="46b5e-124">名称</span><span class="sxs-lookup"><span data-stu-id="46b5e-124">Name</span></span>          | <span data-ttu-id="46b5e-125">说明</span><span class="sxs-lookup"><span data-stu-id="46b5e-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="46b5e-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="46b5e-126">Authorization</span></span> | <span data-ttu-id="46b5e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="46b5e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="46b5e-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="46b5e-129">Content-type</span></span> | <span data-ttu-id="46b5e-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="46b5e-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="46b5e-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="46b5e-132">Request body</span></span>
<span data-ttu-id="46b5e-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="46b5e-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="46b5e-134">参数</span><span class="sxs-lookup"><span data-stu-id="46b5e-134">Parameter</span></span>      | <span data-ttu-id="46b5e-135">类型</span><span class="sxs-lookup"><span data-stu-id="46b5e-135">Type</span></span>    |<span data-ttu-id="46b5e-136">说明</span><span class="sxs-lookup"><span data-stu-id="46b5e-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46b5e-137">适用</span><span class="sxs-lookup"><span data-stu-id="46b5e-137">clientContext</span></span>|<span data-ttu-id="46b5e-138">String</span><span class="sxs-lookup"><span data-stu-id="46b5e-138">String</span></span>|<span data-ttu-id="46b5e-139">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="46b5e-139">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="46b5e-140">响应</span><span class="sxs-lookup"><span data-stu-id="46b5e-140">Response</span></span>
<span data-ttu-id="46b5e-141">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [muteParticipantOperation](../resources/muteParticipantoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="46b5e-141">If successful, this method returns a `200 OK` response code and a [muteParticipantOperation](../resources/muteParticipantoperation.md) object in the response body.</span></span>

> <span data-ttu-id="46b5e-142">**注意：** 此操作返回成功响应后，所有参与者都将收到名单更新</span><span class="sxs-lookup"><span data-stu-id="46b5e-142">**Note:** After this operation returns a successful response, all participants will receive a roster update</span></span>

## <a name="example"></a><span data-ttu-id="46b5e-143">示例</span><span class="sxs-lookup"><span data-stu-id="46b5e-143">Example</span></span>
<span data-ttu-id="46b5e-144">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="46b5e-144">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="46b5e-145">请求</span><span class="sxs-lookup"><span data-stu-id="46b5e-145">Request</span></span>
<span data-ttu-id="46b5e-146">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="46b5e-146">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="46b5e-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="46b5e-147">HTTP</span></span>](#tab/http)
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

# <a name="c"></a>[<span data-ttu-id="46b5e-148">C#</span><span class="sxs-lookup"><span data-stu-id="46b5e-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-mute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="46b5e-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46b5e-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-mute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="46b5e-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46b5e-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-mute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="46b5e-151">响应</span><span class="sxs-lookup"><span data-stu-id="46b5e-151">Response</span></span>

> <span data-ttu-id="46b5e-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="46b5e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span> 
 
<!-- { 
  "blockType": "response", 
  "truncated": true, 
  "@odata.type": "microsoft.graph.muteParticipantOperation" 
} --> 
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Content-Type: application/json
Content-Length: 259
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.muteParticipantOperation",
  "truncated": true
}-->
```json
{
  "@odata.type": "#microsoft.graph.muteParticipantOperation",
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#muteParticipantOperation",
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "clientContext": "clientContext-value"
}
```

##### <a name="notification---roster-updated-with-participant-muted"></a><span data-ttu-id="46b5e-154">通知-名单在参与者静音时更新</span><span class="sxs-lookup"><span data-stu-id="46b5e-154">Notification - roster updated with participant muted</span></span>

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


