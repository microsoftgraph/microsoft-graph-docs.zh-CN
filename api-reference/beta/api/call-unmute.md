---
title: call： unmute
description: 允许应用程序自行取消静音。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 1e995e17bfd98b26ae4680c1215a56d231e0116c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047600"
---
# <a name="call-unmute"></a><span data-ttu-id="e40b6-103">call： unmute</span><span class="sxs-lookup"><span data-stu-id="e40b6-103">call: unmute</span></span>

<span data-ttu-id="e40b6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e40b6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e40b6-105">允许应用程序自行取消静音。</span><span class="sxs-lookup"><span data-stu-id="e40b6-105">Allow the application to unmute itself.</span></span>

<span data-ttu-id="e40b6-106">这是服务器取消静音，这意味着服务器将开始向其他参与者发送此参与者的音频数据包。</span><span class="sxs-lookup"><span data-stu-id="e40b6-106">This is a server unmute, meaning that the server will start sending audio packets for this participant to other participants again.</span></span>

<span data-ttu-id="e40b6-107">若要详细了解如何处理取消静音操作，请参阅 [unmuteParticipantOperation](../resources/unmuteParticipantoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="e40b6-107">For more information about how to handle unmute operations, see [unmuteParticipantOperation](../resources/unmuteParticipantoperation.md).</span></span>

> <span data-ttu-id="e40b6-108">**注意：** 此方法仅支持组调用。</span><span class="sxs-lookup"><span data-stu-id="e40b6-108">**Note:** This method is only supported for group calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="e40b6-109">权限</span><span class="sxs-lookup"><span data-stu-id="e40b6-109">Permissions</span></span>

| <span data-ttu-id="e40b6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e40b6-110">Permission type</span></span>                        | <span data-ttu-id="e40b6-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e40b6-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e40b6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e40b6-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e40b6-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e40b6-113">Not supported.</span></span>                               |
| <span data-ttu-id="e40b6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e40b6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e40b6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e40b6-115">Not supported.</span></span>                               |
| <span data-ttu-id="e40b6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e40b6-116">Application</span></span>                            | <span data-ttu-id="e40b6-117">无。</span><span class="sxs-lookup"><span data-stu-id="e40b6-117">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="e40b6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e40b6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/unmute
POST /communications/calls/{id}/unmute
```
> <span data-ttu-id="e40b6-119">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="e40b6-119">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="e40b6-120">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="e40b6-120">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e40b6-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e40b6-121">Request headers</span></span>
| <span data-ttu-id="e40b6-122">名称</span><span class="sxs-lookup"><span data-stu-id="e40b6-122">Name</span></span>          | <span data-ttu-id="e40b6-123">说明</span><span class="sxs-lookup"><span data-stu-id="e40b6-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e40b6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e40b6-124">Authorization</span></span> | <span data-ttu-id="e40b6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e40b6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e40b6-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="e40b6-127">Content-type</span></span> | <span data-ttu-id="e40b6-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e40b6-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e40b6-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="e40b6-130">Request body</span></span>
<span data-ttu-id="e40b6-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="e40b6-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e40b6-132">参数</span><span class="sxs-lookup"><span data-stu-id="e40b6-132">Parameter</span></span>      | <span data-ttu-id="e40b6-133">类型</span><span class="sxs-lookup"><span data-stu-id="e40b6-133">Type</span></span>    |<span data-ttu-id="e40b6-134">说明</span><span class="sxs-lookup"><span data-stu-id="e40b6-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e40b6-135">clientContext</span><span class="sxs-lookup"><span data-stu-id="e40b6-135">clientContext</span></span>|<span data-ttu-id="e40b6-136">String</span><span class="sxs-lookup"><span data-stu-id="e40b6-136">String</span></span>|<span data-ttu-id="e40b6-137">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="e40b6-137">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="e40b6-138">响应</span><span class="sxs-lookup"><span data-stu-id="e40b6-138">Response</span></span>
<span data-ttu-id="e40b6-139">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [unmuteParticipantOperation](../resources/unmuteParticipantoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e40b6-139">If successful, this method returns a `200 OK` response code and a [unmuteParticipantOperation](../resources/unmuteParticipantoperation.md) object in the response body.</span></span>

><span data-ttu-id="e40b6-140">**注意：** 当此 API 返回成功响应时，所有参与者都将收到名单更新。</span><span class="sxs-lookup"><span data-stu-id="e40b6-140">**Note:** When this API returns a successful response, all participants will receive a roster update.</span></span>

## <a name="example"></a><span data-ttu-id="e40b6-141">示例</span><span class="sxs-lookup"><span data-stu-id="e40b6-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e40b6-142">请求</span><span class="sxs-lookup"><span data-stu-id="e40b6-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e40b6-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="e40b6-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-unmute"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/unmute
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "clientContext-value"
}
```
# <a name="c"></a>[<span data-ttu-id="e40b6-144">C#</span><span class="sxs-lookup"><span data-stu-id="e40b6-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-unmute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e40b6-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e40b6-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-unmute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e40b6-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e40b6-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-unmute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e40b6-147">Java</span><span class="sxs-lookup"><span data-stu-id="e40b6-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-unmute-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e40b6-148">响应</span><span class="sxs-lookup"><span data-stu-id="e40b6-148">Response</span></span>

> <span data-ttu-id="e40b6-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e40b6-149">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unmuteParticipantOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Content-Type: application/json
Content-Length: 259
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.unmuteParticipantOperation",
  "truncated": true
}-->
```json
{
  "@odata.type": "#microsoft.graph.unmuteParticipantOperation",
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#unmuteParticipantOperation",
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "clientContext": "clientContext-value"
}
```

##### <a name="notification---roster-updated-with-participant-unmuted"></a><span data-ttu-id="e40b6-150">通知 - 使用参与者取消静音更新名单</span><span class="sxs-lookup"><span data-stu-id="e40b6-150">Notification - roster updated with participant unmuted</span></span>

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
          "isMuted": false, // will be set to false on unmute
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
  "description": "call: unmute",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


