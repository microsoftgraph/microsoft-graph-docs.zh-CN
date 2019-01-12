---
title: 参与者： 设为静音
description: 将呼叫中的特定参与者设为静音。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d41d97556aff7093660c0cdfb75a43f8b862c0d7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964471"
---
# <a name="participant-mute"></a><span data-ttu-id="01804-103">参与者： 设为静音</span><span class="sxs-lookup"><span data-stu-id="01804-103">participant: mute</span></span>

> <span data-ttu-id="01804-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="01804-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01804-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="01804-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="01804-106">将呼叫中的特定参与者设为静音。</span><span class="sxs-lookup"><span data-stu-id="01804-106">Mute a specific participant in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="01804-107">权限</span><span class="sxs-lookup"><span data-stu-id="01804-107">Permissions</span></span>
<span data-ttu-id="01804-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="01804-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="01804-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="01804-110">Permission type</span></span> | <span data-ttu-id="01804-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="01804-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="01804-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="01804-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="01804-113">不支持</span><span class="sxs-lookup"><span data-stu-id="01804-113">Not Supported</span></span>        |
| <span data-ttu-id="01804-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="01804-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01804-115">不支持</span><span class="sxs-lookup"><span data-stu-id="01804-115">Not Supported</span></span>        |
| <span data-ttu-id="01804-116">用途</span><span class="sxs-lookup"><span data-stu-id="01804-116">Application</span></span>     | <span data-ttu-id="01804-117">无</span><span class="sxs-lookup"><span data-stu-id="01804-117">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="01804-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="01804-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/{id}/mute
POST /applications/{id}/calls/{id}/participants/{id}/mute
```

## <a name="request-headers"></a><span data-ttu-id="01804-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="01804-119">Request headers</span></span>
| <span data-ttu-id="01804-120">名称</span><span class="sxs-lookup"><span data-stu-id="01804-120">Name</span></span>          | <span data-ttu-id="01804-121">说明</span><span class="sxs-lookup"><span data-stu-id="01804-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="01804-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="01804-122">Authorization</span></span> | <span data-ttu-id="01804-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="01804-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="01804-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="01804-125">Request body</span></span>
<span data-ttu-id="01804-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="01804-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="01804-127">参数</span><span class="sxs-lookup"><span data-stu-id="01804-127">Parameter</span></span>      | <span data-ttu-id="01804-128">类型</span><span class="sxs-lookup"><span data-stu-id="01804-128">Type</span></span>    |<span data-ttu-id="01804-129">说明</span><span class="sxs-lookup"><span data-stu-id="01804-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01804-130">clientContext</span><span class="sxs-lookup"><span data-stu-id="01804-130">clientContext</span></span>|<span data-ttu-id="01804-131">字符串</span><span class="sxs-lookup"><span data-stu-id="01804-131">String</span></span>|<span data-ttu-id="01804-132">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="01804-132">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="01804-133">响应</span><span class="sxs-lookup"><span data-stu-id="01804-133">Response</span></span>
<span data-ttu-id="01804-134">如果成功，此方法返回`200 OK`响应正文中的响应代码和[commsOperation](../resources/commsoperation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="01804-134">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01804-135">示例</span><span class="sxs-lookup"><span data-stu-id="01804-135">Example</span></span>
<span data-ttu-id="01804-136">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="01804-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="01804-137">请求</span><span class="sxs-lookup"><span data-stu-id="01804-137">Request</span></span>
<span data-ttu-id="01804-138">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="01804-138">The following example shows the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="01804-139">响应</span><span class="sxs-lookup"><span data-stu-id="01804-139">Response</span></span>

> <span data-ttu-id="01804-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="01804-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

## <a name="example---mute-specific-participant"></a><span data-ttu-id="01804-142">示例-静音特定参与者</span><span class="sxs-lookup"><span data-stu-id="01804-142">Example - Mute specific participant</span></span>

##### <a name="request"></a><span data-ttu-id="01804-143">请求</span><span class="sxs-lookup"><span data-stu-id="01804-143">Request</span></span>

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants/0698446E77E24E4D85F80597083CB830/mute
Authorization: Bearer <TOKEN>
Content-Type: application/json

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="response"></a><span data-ttu-id="01804-144">响应</span><span class="sxs-lookup"><span data-stu-id="01804-144">Response</span></span>

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

##### <a name="notification---roster-updated-with-participant-muted"></a><span data-ttu-id="01804-145">通知-更新与设为静音的参与者名单</span><span class="sxs-lookup"><span data-stu-id="01804-145">Notification - roster updated with participant muted</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "participant: mute",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
