---
title: 呼叫：取消静音
description: 允许应用程序自行取消静音。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 51ad26211208934599feb65d4f932d8654fd170e
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913630"
---
# <a name="call-unmute"></a><span data-ttu-id="3f22c-103">呼叫：取消静音</span><span class="sxs-lookup"><span data-stu-id="3f22c-103">call: unmute</span></span>

<span data-ttu-id="3f22c-104">允许应用程序自行取消静音。</span><span class="sxs-lookup"><span data-stu-id="3f22c-104">Allow the application to unmute itself.</span></span>

<span data-ttu-id="3f22c-105">这是一种服务器取消静音，这意味着服务器将再次开始将此参与者的音频数据包发送给其他参与者。</span><span class="sxs-lookup"><span data-stu-id="3f22c-105">This is a server unmute, meaning that the server will start sending audio packets for this participant to other participants again.</span></span>

<span data-ttu-id="3f22c-106">有关如何处理静音操作的详细信息，请参阅[unmuteParticipantOperation](../resources/unmuteParticipantoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="3f22c-106">For more information about how to handle unmute operations, see [unmuteParticipantOperation](../resources/unmuteParticipantoperation.md).</span></span>

> <span data-ttu-id="3f22c-107">**注意：** 仅组调用支持此方法。</span><span class="sxs-lookup"><span data-stu-id="3f22c-107">**Note:** This method is only supported for group calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="3f22c-108">权限</span><span class="sxs-lookup"><span data-stu-id="3f22c-108">Permissions</span></span>

| <span data-ttu-id="3f22c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3f22c-109">Permission type</span></span>                        | <span data-ttu-id="3f22c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3f22c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3f22c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3f22c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3f22c-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="3f22c-112">Not supported.</span></span>                               |
| <span data-ttu-id="3f22c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3f22c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f22c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3f22c-114">Not supported.</span></span>                               |
| <span data-ttu-id="3f22c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3f22c-115">Application</span></span>                            | <span data-ttu-id="3f22c-116">无。</span><span class="sxs-lookup"><span data-stu-id="3f22c-116">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="3f22c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3f22c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/unmute
```

## <a name="request-headers"></a><span data-ttu-id="3f22c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3f22c-118">Request headers</span></span>
| <span data-ttu-id="3f22c-119">名称</span><span class="sxs-lookup"><span data-stu-id="3f22c-119">Name</span></span>          | <span data-ttu-id="3f22c-120">说明</span><span class="sxs-lookup"><span data-stu-id="3f22c-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="3f22c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f22c-121">Authorization</span></span> | <span data-ttu-id="3f22c-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3f22c-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3f22c-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="3f22c-124">Content-type</span></span> | <span data-ttu-id="3f22c-p102">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="3f22c-p102">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f22c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3f22c-127">Request body</span></span>
<span data-ttu-id="3f22c-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="3f22c-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3f22c-129">参数</span><span class="sxs-lookup"><span data-stu-id="3f22c-129">Parameter</span></span>      | <span data-ttu-id="3f22c-130">类型</span><span class="sxs-lookup"><span data-stu-id="3f22c-130">Type</span></span>    |<span data-ttu-id="3f22c-131">说明</span><span class="sxs-lookup"><span data-stu-id="3f22c-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3f22c-132">适用</span><span class="sxs-lookup"><span data-stu-id="3f22c-132">clientContext</span></span>|<span data-ttu-id="3f22c-133">String</span><span class="sxs-lookup"><span data-stu-id="3f22c-133">String</span></span>|<span data-ttu-id="3f22c-134">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="3f22c-134">Unique Client Context string.</span></span> <span data-ttu-id="3f22c-135">最大限制为256个字符。</span><span class="sxs-lookup"><span data-stu-id="3f22c-135">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="3f22c-136">响应</span><span class="sxs-lookup"><span data-stu-id="3f22c-136">Response</span></span>
<span data-ttu-id="3f22c-137">如果成功，此方法在响应`200 OK`正文中返回响应代码和[unmuteParticipantOperation](../resources/unmuteParticipantoperation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3f22c-137">If successful, this method returns a `200 OK` response code and a [unmuteParticipantOperation](../resources/unmuteParticipantoperation.md) object in the response body.</span></span>

><span data-ttu-id="3f22c-138">**注意：** 当此 API 返回成功响应时，所有参与者都将收到名单更新。</span><span class="sxs-lookup"><span data-stu-id="3f22c-138">**Note:** When this API returns a successful response, all participants will receive a roster update.</span></span>

## <a name="example"></a><span data-ttu-id="3f22c-139">示例</span><span class="sxs-lookup"><span data-stu-id="3f22c-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3f22c-140">请求</span><span class="sxs-lookup"><span data-stu-id="3f22c-140">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3f22c-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f22c-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-unmute"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/unmute
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "clientContext-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3f22c-142">C#</span><span class="sxs-lookup"><span data-stu-id="3f22c-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-unmute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3f22c-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f22c-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-unmute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3f22c-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f22c-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-unmute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3f22c-145">Java</span><span class="sxs-lookup"><span data-stu-id="3f22c-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-unmute-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3f22c-146">响应</span><span class="sxs-lookup"><span data-stu-id="3f22c-146">Response</span></span>

> <span data-ttu-id="3f22c-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3f22c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unmuteParticipantOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#unmuteParticipantOperation",
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "clientContext": "clientContext-value"
}
```

##### <a name="notification---roster-updated-with-participant-unmuted"></a><span data-ttu-id="3f22c-149">通知名单使用参与者 unmuted 更新</span><span class="sxs-lookup"><span data-stu-id="3f22c-149">Notification - roster updated with participant unmuted</span></span>

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
