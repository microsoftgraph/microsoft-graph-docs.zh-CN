---
title: 呼叫：取消静音
description: 允许应用程序自行取消静音。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 7db831333982126b0edd24a5664388a89e8bc74d
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38005915"
---
# <a name="call-unmute"></a><span data-ttu-id="e109f-103">呼叫：取消静音</span><span class="sxs-lookup"><span data-stu-id="e109f-103">call: unmute</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e109f-104">允许应用程序自行取消静音。</span><span class="sxs-lookup"><span data-stu-id="e109f-104">Allow the application to unmute itself.</span></span>

<span data-ttu-id="e109f-105">这是一种服务器取消静音，这意味着服务器将再次开始将此参与者的音频数据包发送给其他参与者。</span><span class="sxs-lookup"><span data-stu-id="e109f-105">This is a server unmute, meaning that the server will start sending audio packets for this participant to other participants again.</span></span>

<span data-ttu-id="e109f-106">有关如何处理操作的详细信息，请参阅[commsOperation](../resources/commsOperation.md)。</span><span class="sxs-lookup"><span data-stu-id="e109f-106">For more information about how to handle operations, see [commsOperation](../resources/commsOperation.md).</span></span>

> <span data-ttu-id="e109f-107">**注意：** 这仅对组调用受支持。</span><span class="sxs-lookup"><span data-stu-id="e109f-107">**Note:** This is only supported for group calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="e109f-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="e109f-108">Permissions</span></span>

| <span data-ttu-id="e109f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e109f-109">Permission type</span></span>                        | <span data-ttu-id="e109f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e109f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e109f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e109f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e109f-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="e109f-112">Not supported.</span></span>                               |
| <span data-ttu-id="e109f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e109f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e109f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e109f-114">Not supported.</span></span>                               |
| <span data-ttu-id="e109f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e109f-115">Application</span></span>                            | <span data-ttu-id="e109f-116">无。</span><span class="sxs-lookup"><span data-stu-id="e109f-116">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="e109f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e109f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/unmute
POST /communications/calls/{id}/unmute
```
> <span data-ttu-id="e109f-118">**注意：**`/app`路径已被弃用。</span><span class="sxs-lookup"><span data-stu-id="e109f-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="e109f-119">接下来，请使用`/communications`路径。</span><span class="sxs-lookup"><span data-stu-id="e109f-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e109f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e109f-120">Request headers</span></span>
| <span data-ttu-id="e109f-121">名称</span><span class="sxs-lookup"><span data-stu-id="e109f-121">Name</span></span>          | <span data-ttu-id="e109f-122">说明</span><span class="sxs-lookup"><span data-stu-id="e109f-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e109f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e109f-123">Authorization</span></span> | <span data-ttu-id="e109f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e109f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e109f-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="e109f-126">Content-type</span></span> | <span data-ttu-id="e109f-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e109f-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e109f-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="e109f-129">Request body</span></span>
<span data-ttu-id="e109f-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="e109f-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e109f-131">参数</span><span class="sxs-lookup"><span data-stu-id="e109f-131">Parameter</span></span>      | <span data-ttu-id="e109f-132">类型</span><span class="sxs-lookup"><span data-stu-id="e109f-132">Type</span></span>    |<span data-ttu-id="e109f-133">说明</span><span class="sxs-lookup"><span data-stu-id="e109f-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e109f-134">适用</span><span class="sxs-lookup"><span data-stu-id="e109f-134">clientContext</span></span>|<span data-ttu-id="e109f-135">String</span><span class="sxs-lookup"><span data-stu-id="e109f-135">String</span></span>|<span data-ttu-id="e109f-136">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="e109f-136">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="e109f-137">响应</span><span class="sxs-lookup"><span data-stu-id="e109f-137">Response</span></span>
<span data-ttu-id="e109f-138">如果成功，此方法在响应`200 OK`正文中返回响应代码和[commsOperation](../resources/commsoperation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e109f-138">If successful, this method returns a `200 OK` response code and a [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

><span data-ttu-id="e109f-139">**注意：** 当此 API 返回成功响应时，所有参与者都将收到名单更新。</span><span class="sxs-lookup"><span data-stu-id="e109f-139">**Note:** When this API returns a successful response, all participants will receive a roster update.</span></span>

## <a name="example"></a><span data-ttu-id="e109f-140">示例</span><span class="sxs-lookup"><span data-stu-id="e109f-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e109f-141">请求</span><span class="sxs-lookup"><span data-stu-id="e109f-141">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e109f-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="e109f-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="e109f-143">C#</span><span class="sxs-lookup"><span data-stu-id="e109f-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-unmute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e109f-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e109f-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-unmute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e109f-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e109f-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-unmute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e109f-146">响应</span><span class="sxs-lookup"><span data-stu-id="e109f-146">Response</span></span>

> <span data-ttu-id="e109f-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e109f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

##### <a name="notification---roster-updated-with-participant-unmuted"></a><span data-ttu-id="e109f-149">通知名单使用参与者 unmuted 更新</span><span class="sxs-lookup"><span data-stu-id="e109f-149">Notification - roster updated with participant unmuted</span></span>

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
