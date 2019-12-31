---
title: 参与者：静音
description: 将呼叫中的特定参与者静音。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 2c65bf06524b883ca4632a6127e50a13e4355054
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913420"
---
# <a name="participant-mute"></a><span data-ttu-id="f9fe2-103">参与者：静音</span><span class="sxs-lookup"><span data-stu-id="f9fe2-103">participant: mute</span></span>

<span data-ttu-id="f9fe2-104">将呼叫中的特定参与者静音。</span><span class="sxs-lookup"><span data-stu-id="f9fe2-104">Mute a specific participant in the call.</span></span>

<span data-ttu-id="f9fe2-105">这是一种服务器静音，这意味着服务器将丢弃此参与者的所有音频数据包，即使参与者继续传输音频也是如此。</span><span class="sxs-lookup"><span data-stu-id="f9fe2-105">This is a server mute, meaning that the server will drop all audio packets for this participant, even if the participant continues to stream audio.</span></span>

<span data-ttu-id="f9fe2-106">有关如何处理静音操作的详细信息，请参阅[muteParticipantOperation](../resources/muteParticipantoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="f9fe2-106">For more information about how to handle mute operations, see [muteParticipantOperation](../resources/muteParticipantoperation.md).</span></span>

> <span data-ttu-id="f9fe2-107">**注意：** 仅组调用支持此方法。</span><span class="sxs-lookup"><span data-stu-id="f9fe2-107">**Note:** This method is only supported for group calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9fe2-108">权限</span><span class="sxs-lookup"><span data-stu-id="f9fe2-108">Permissions</span></span>

| <span data-ttu-id="f9fe2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f9fe2-109">Permission type</span></span> | <span data-ttu-id="f9fe2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f9fe2-110">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="f9fe2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f9fe2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f9fe2-112">不支持</span><span class="sxs-lookup"><span data-stu-id="f9fe2-112">Not Supported</span></span>        |
| <span data-ttu-id="f9fe2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f9fe2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9fe2-114">不支持</span><span class="sxs-lookup"><span data-stu-id="f9fe2-114">Not Supported</span></span>        |
| <span data-ttu-id="f9fe2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f9fe2-115">Application</span></span>     | <span data-ttu-id="f9fe2-116">无</span><span class="sxs-lookup"><span data-stu-id="f9fe2-116">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="f9fe2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f9fe2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/participants/{id}/mute
```

## <a name="request-headers"></a><span data-ttu-id="f9fe2-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f9fe2-118">Request headers</span></span>
| <span data-ttu-id="f9fe2-119">名称</span><span class="sxs-lookup"><span data-stu-id="f9fe2-119">Name</span></span>          | <span data-ttu-id="f9fe2-120">说明</span><span class="sxs-lookup"><span data-stu-id="f9fe2-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f9fe2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9fe2-121">Authorization</span></span> | <span data-ttu-id="f9fe2-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f9fe2-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f9fe2-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="f9fe2-124">Content-type</span></span>  | <span data-ttu-id="f9fe2-p102">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f9fe2-p102">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9fe2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f9fe2-127">Request body</span></span>
<span data-ttu-id="f9fe2-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f9fe2-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f9fe2-129">参数</span><span class="sxs-lookup"><span data-stu-id="f9fe2-129">Parameter</span></span>      | <span data-ttu-id="f9fe2-130">类型</span><span class="sxs-lookup"><span data-stu-id="f9fe2-130">Type</span></span>    |<span data-ttu-id="f9fe2-131">说明</span><span class="sxs-lookup"><span data-stu-id="f9fe2-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9fe2-132">适用</span><span class="sxs-lookup"><span data-stu-id="f9fe2-132">clientContext</span></span>|<span data-ttu-id="f9fe2-133">String</span><span class="sxs-lookup"><span data-stu-id="f9fe2-133">String</span></span>|<span data-ttu-id="f9fe2-134">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="f9fe2-134">Unique Client Context string.</span></span> <span data-ttu-id="f9fe2-135">最大限制为256个字符。</span><span class="sxs-lookup"><span data-stu-id="f9fe2-135">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="f9fe2-136">响应</span><span class="sxs-lookup"><span data-stu-id="f9fe2-136">Response</span></span>
<span data-ttu-id="f9fe2-137">如果成功，此方法在响应`200 OK`正文中返回响应代码和[muteParticipantOperation](../resources/muteParticipantoperation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f9fe2-137">If successful, this method returns a `200 OK` response code and a [muteParticipantOperation](../resources/muteParticipantoperation.md) object in the response body.</span></span>

><span data-ttu-id="f9fe2-138">**注意：** 当此 API 返回成功响应时，所有参与者都将收到名单更新。</span><span class="sxs-lookup"><span data-stu-id="f9fe2-138">**Note:** When this API returns a successful response, all participants will receive a roster update.</span></span>

## <a name="example---mute-specific-participant"></a><span data-ttu-id="f9fe2-139">示例-特定参与者的静音</span><span class="sxs-lookup"><span data-stu-id="f9fe2-139">Example - Mute specific participant</span></span>
<span data-ttu-id="f9fe2-140">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="f9fe2-140">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="f9fe2-141">请求</span><span class="sxs-lookup"><span data-stu-id="f9fe2-141">Request</span></span>
<span data-ttu-id="f9fe2-142">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="f9fe2-142">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f9fe2-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9fe2-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-mute"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/participants/2765eb15-01f8-47c6-b12b-c32111a4a86f/mute
Content-Type: application/json

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f9fe2-144">C#</span><span class="sxs-lookup"><span data-stu-id="f9fe2-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-mute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f9fe2-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9fe2-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-mute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f9fe2-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9fe2-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-mute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f9fe2-147">Java</span><span class="sxs-lookup"><span data-stu-id="f9fe2-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/participant-mute-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f9fe2-148">响应</span><span class="sxs-lookup"><span data-stu-id="f9fe2-148">Response</span></span>

> <span data-ttu-id="f9fe2-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f9fe2-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span> 


<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.muteParticipantOperation",
  "truncated": true
}-->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.muteParticipantOperation",
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#muteParticipantOperation",
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="notification---roster-updated-with-participant-muted"></a><span data-ttu-id="f9fe2-151">通知-名单在参与者静音时更新</span><span class="sxs-lookup"><span data-stu-id="f9fe2-151">Notification - roster updated with participant muted</span></span>

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
