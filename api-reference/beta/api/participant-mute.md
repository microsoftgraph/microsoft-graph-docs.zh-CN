---
title: participant： mute
description: 将呼叫中的特定参与者静音。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 0399807f7cd962b508b10cc5dd0cd3ed8d3378ff
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049189"
---
# <a name="participant-mute"></a><span data-ttu-id="11979-103">participant： mute</span><span class="sxs-lookup"><span data-stu-id="11979-103">participant: mute</span></span>

<span data-ttu-id="11979-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11979-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11979-105">将呼叫中的特定参与者静音。</span><span class="sxs-lookup"><span data-stu-id="11979-105">Mute a specific participant in the call.</span></span>

<span data-ttu-id="11979-106">这是服务器静音，这意味着服务器将删除此参与者的所有音频数据包，即使参与者继续流式传输音频。</span><span class="sxs-lookup"><span data-stu-id="11979-106">This is a server mute, meaning that the server will drop all audio packets for this participant, even if the participant continues to stream audio.</span></span>

<span data-ttu-id="11979-107">若要详细了解如何处理静音操作，请参阅 [muteParticipantOperation](../resources/muteParticipantoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="11979-107">For more information about how to handle mute operations, see [muteParticipantOperation](../resources/muteParticipantoperation.md).</span></span>

> <span data-ttu-id="11979-108">**注意：** 此方法仅支持组调用。</span><span class="sxs-lookup"><span data-stu-id="11979-108">**Note:** This method is only supported for group calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="11979-109">权限</span><span class="sxs-lookup"><span data-stu-id="11979-109">Permissions</span></span>

| <span data-ttu-id="11979-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="11979-110">Permission type</span></span> | <span data-ttu-id="11979-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="11979-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="11979-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="11979-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="11979-113">不支持</span><span class="sxs-lookup"><span data-stu-id="11979-113">Not Supported</span></span>        |
| <span data-ttu-id="11979-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="11979-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11979-115">不支持</span><span class="sxs-lookup"><span data-stu-id="11979-115">Not Supported</span></span>        |
| <span data-ttu-id="11979-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="11979-116">Application</span></span>     | <span data-ttu-id="11979-117">无</span><span class="sxs-lookup"><span data-stu-id="11979-117">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="11979-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="11979-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/{id}/mute
POST /communications/calls/{id}/participants/{id}/mute
```
> <span data-ttu-id="11979-119">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="11979-119">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="11979-120">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="11979-120">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="11979-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="11979-121">Request headers</span></span>
| <span data-ttu-id="11979-122">名称</span><span class="sxs-lookup"><span data-stu-id="11979-122">Name</span></span>          | <span data-ttu-id="11979-123">说明</span><span class="sxs-lookup"><span data-stu-id="11979-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="11979-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="11979-124">Authorization</span></span> | <span data-ttu-id="11979-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="11979-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="11979-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="11979-127">Content-type</span></span>  | <span data-ttu-id="11979-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="11979-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="11979-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="11979-130">Request body</span></span>
<span data-ttu-id="11979-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="11979-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="11979-132">参数</span><span class="sxs-lookup"><span data-stu-id="11979-132">Parameter</span></span>      | <span data-ttu-id="11979-133">类型</span><span class="sxs-lookup"><span data-stu-id="11979-133">Type</span></span>    |<span data-ttu-id="11979-134">说明</span><span class="sxs-lookup"><span data-stu-id="11979-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11979-135">clientContext</span><span class="sxs-lookup"><span data-stu-id="11979-135">clientContext</span></span>|<span data-ttu-id="11979-136">String</span><span class="sxs-lookup"><span data-stu-id="11979-136">String</span></span>|<span data-ttu-id="11979-137">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="11979-137">Unique Client Context string.</span></span> <span data-ttu-id="11979-138">最大限制为 256 个字符。</span><span class="sxs-lookup"><span data-stu-id="11979-138">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="11979-139">响应</span><span class="sxs-lookup"><span data-stu-id="11979-139">Response</span></span>
<span data-ttu-id="11979-140">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [muteParticipantOperation](../resources/muteParticipantoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="11979-140">If successful, this method returns a `200 OK` response code and a [muteParticipantOperation](../resources/muteParticipantoperation.md) object in the response body.</span></span>

><span data-ttu-id="11979-141">**注意：** 当此 API 返回成功响应时，所有参与者都将收到名单更新。</span><span class="sxs-lookup"><span data-stu-id="11979-141">**Note:** When this API returns a successful response, all participants will receive a roster update.</span></span>

## <a name="example---mute-specific-participant"></a><span data-ttu-id="11979-142">示例 - 将特定参与者设为静音</span><span class="sxs-lookup"><span data-stu-id="11979-142">Example - Mute specific participant</span></span>
<span data-ttu-id="11979-143">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="11979-143">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="11979-144">请求</span><span class="sxs-lookup"><span data-stu-id="11979-144">Request</span></span>
<span data-ttu-id="11979-145">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="11979-145">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="11979-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="11979-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-mute"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/participants/2765eb15-01f8-47c6-b12b-c32111a4a86f/mute
Content-Type: application/json

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```
# <a name="c"></a>[<span data-ttu-id="11979-147">C#</span><span class="sxs-lookup"><span data-stu-id="11979-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-mute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11979-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11979-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-mute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11979-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11979-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-mute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="11979-150">Java</span><span class="sxs-lookup"><span data-stu-id="11979-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/participant-mute-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="11979-151">响应</span><span class="sxs-lookup"><span data-stu-id="11979-151">Response</span></span>

> <span data-ttu-id="11979-152">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="11979-152">**Note:** The response object shown here might be shortened for readability.</span></span> 


<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.muteParticipantOperation",
  "truncated": true
}-->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.muteParticipantOperation",
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#muteParticipantOperation",
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="notification---roster-updated-with-participant-muted"></a><span data-ttu-id="11979-153">通知 - 参与者静音更新名单</span><span class="sxs-lookup"><span data-stu-id="11979-153">Notification - roster updated with participant muted</span></span>

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
  "description": "participant: mute",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


