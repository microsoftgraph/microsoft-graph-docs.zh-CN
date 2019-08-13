---
title: '参与者: 静音'
description: 将呼叫中的特定参与者静音。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 22d8fc973a181b6c569fbc6738882e4e89b147be
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349570"
---
# <a name="participant-mute"></a><span data-ttu-id="4f172-103">参与者: 静音</span><span class="sxs-lookup"><span data-stu-id="4f172-103">participant: mute</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f172-104">将呼叫中的特定参与者静音。</span><span class="sxs-lookup"><span data-stu-id="4f172-104">Mute a specific participant in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f172-105">权限</span><span class="sxs-lookup"><span data-stu-id="4f172-105">Permissions</span></span>
<span data-ttu-id="4f172-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4f172-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4f172-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4f172-108">Permission type</span></span> | <span data-ttu-id="4f172-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4f172-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="4f172-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4f172-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4f172-111">不支持</span><span class="sxs-lookup"><span data-stu-id="4f172-111">Not Supported</span></span>        |
| <span data-ttu-id="4f172-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4f172-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f172-113">不支持</span><span class="sxs-lookup"><span data-stu-id="4f172-113">Not Supported</span></span>        |
| <span data-ttu-id="4f172-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4f172-114">Application</span></span>     | <span data-ttu-id="4f172-115">无</span><span class="sxs-lookup"><span data-stu-id="4f172-115">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="4f172-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4f172-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/{id}/mute
POST /applications/{id}/calls/{id}/participants/{id}/mute
```

## <a name="request-headers"></a><span data-ttu-id="4f172-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="4f172-117">Request headers</span></span>
| <span data-ttu-id="4f172-118">名称</span><span class="sxs-lookup"><span data-stu-id="4f172-118">Name</span></span>          | <span data-ttu-id="4f172-119">说明</span><span class="sxs-lookup"><span data-stu-id="4f172-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="4f172-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f172-120">Authorization</span></span> | <span data-ttu-id="4f172-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4f172-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f172-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="4f172-123">Request body</span></span>
<span data-ttu-id="4f172-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="4f172-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4f172-125">参数</span><span class="sxs-lookup"><span data-stu-id="4f172-125">Parameter</span></span>      | <span data-ttu-id="4f172-126">类型</span><span class="sxs-lookup"><span data-stu-id="4f172-126">Type</span></span>    |<span data-ttu-id="4f172-127">说明</span><span class="sxs-lookup"><span data-stu-id="4f172-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4f172-128">适用</span><span class="sxs-lookup"><span data-stu-id="4f172-128">clientContext</span></span>|<span data-ttu-id="4f172-129">String</span><span class="sxs-lookup"><span data-stu-id="4f172-129">String</span></span>|<span data-ttu-id="4f172-130">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="4f172-130">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="4f172-131">响应</span><span class="sxs-lookup"><span data-stu-id="4f172-131">Response</span></span>
<span data-ttu-id="4f172-132">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[commsOperation](../resources/commsoperation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4f172-132">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f172-133">示例</span><span class="sxs-lookup"><span data-stu-id="4f172-133">Example</span></span>
<span data-ttu-id="4f172-134">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="4f172-134">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="4f172-135">请求</span><span class="sxs-lookup"><span data-stu-id="4f172-135">Request</span></span>
<span data-ttu-id="4f172-136">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="4f172-136">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4f172-137">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="4f172-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-mute"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/participants/{id}/mute
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "clientContext-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4f172-138">C#</span><span class="sxs-lookup"><span data-stu-id="4f172-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-mute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4f172-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f172-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-mute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4f172-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="4f172-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-mute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4f172-141">Java</span><span class="sxs-lookup"><span data-stu-id="4f172-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/participant-mute-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4f172-142">响应</span><span class="sxs-lookup"><span data-stu-id="4f172-142">Response</span></span>

> <span data-ttu-id="4f172-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4f172-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.commsOperation",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

## <a name="example---mute-specific-participant"></a><span data-ttu-id="4f172-145">示例-特定参与者的静音</span><span class="sxs-lookup"><span data-stu-id="4f172-145">Example - Mute specific participant</span></span>

##### <a name="request"></a><span data-ttu-id="4f172-146">请求</span><span class="sxs-lookup"><span data-stu-id="4f172-146">Request</span></span>

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants/0698446E77E24E4D85F80597083CB830/mute
Authorization: Bearer <TOKEN>
Content-Type: application/json

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="response"></a><span data-ttu-id="4f172-147">响应</span><span class="sxs-lookup"><span data-stu-id="4f172-147">Response</span></span>

```http
HTTP/1.1 200 OK
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
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="notification---roster-updated-with-participant-muted"></a><span data-ttu-id="4f172-148">通知-名单在参与者静音时更新</span><span class="sxs-lookup"><span data-stu-id="4f172-148">Notification - roster updated with participant muted</span></span>

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
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "0698446E77E24E4D85F80597083CB830",
          "info": {
            "identity": {
              "user": {
                "displayName": "Test User",
                "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
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
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isMuted": true,
          "isInLobby": false
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "123456W77E24E4D85F80597083CB830",
          "info": {
            "identity": {
              "application": {
                "displayName": "Test Bot",
                "id": "1234A46B-3D17-4ADC-8DCE-DC4E7D556789"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          },
          "mediaStreams": [
            {
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "2",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
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
