---
title: '参与者: 邀请'
description: 邀请参与者加入活动呼叫。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 10e23f825f48b75dad1f2cb42e422d66feb8daf9
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34537328"
---
# <a name="participant-invite"></a><span data-ttu-id="a4b6e-103">参与者: 邀请</span><span class="sxs-lookup"><span data-stu-id="a4b6e-103">participant: invite</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4b6e-104">邀请参与者加入活动呼叫。</span><span class="sxs-lookup"><span data-stu-id="a4b6e-104">Invite participants to the active call.</span></span>

## <a name="permissions"></a><span data-ttu-id="a4b6e-105">权限</span><span class="sxs-lookup"><span data-stu-id="a4b6e-105">Permissions</span></span>
<span data-ttu-id="a4b6e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a4b6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a4b6e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4b6e-108">Permission type</span></span> | <span data-ttu-id="a4b6e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a4b6e-109">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="a4b6e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4b6e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a4b6e-111">不支持</span><span class="sxs-lookup"><span data-stu-id="a4b6e-111">Not Supported</span></span>                       |
| <span data-ttu-id="a4b6e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4b6e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4b6e-113">不支持</span><span class="sxs-lookup"><span data-stu-id="a4b6e-113">Not Supported</span></span>                       |
| <span data-ttu-id="a4b6e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4b6e-114">Application</span></span>     | <span data-ttu-id="a4b6e-115">InitiateGroupCalls</span><span class="sxs-lookup"><span data-stu-id="a4b6e-115">Calls.InitiateGroupCalls.All</span></span>                               |

## <a name="http-request"></a><span data-ttu-id="a4b6e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4b6e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/invite
POST /applications/{id}/calls/{id}/participants/invite
```

## <a name="request-headers"></a><span data-ttu-id="a4b6e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4b6e-117">Request headers</span></span>
| <span data-ttu-id="a4b6e-118">名称</span><span class="sxs-lookup"><span data-stu-id="a4b6e-118">Name</span></span>          | <span data-ttu-id="a4b6e-119">说明</span><span class="sxs-lookup"><span data-stu-id="a4b6e-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="a4b6e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4b6e-120">Authorization</span></span> | <span data-ttu-id="a4b6e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a4b6e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a4b6e-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4b6e-123">Request body</span></span>
<span data-ttu-id="a4b6e-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a4b6e-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a4b6e-125">参数</span><span class="sxs-lookup"><span data-stu-id="a4b6e-125">Parameter</span></span>      | <span data-ttu-id="a4b6e-126">类型</span><span class="sxs-lookup"><span data-stu-id="a4b6e-126">Type</span></span>    |<span data-ttu-id="a4b6e-127">说明</span><span class="sxs-lookup"><span data-stu-id="a4b6e-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4b6e-128">participants</span><span class="sxs-lookup"><span data-stu-id="a4b6e-128">participants</span></span>|<span data-ttu-id="a4b6e-129">[invitationParticipantInfo](../resources/invitationparticipantinfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="a4b6e-129">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>| <span data-ttu-id="a4b6e-130">要邀请的参与者。</span><span class="sxs-lookup"><span data-stu-id="a4b6e-130">The participants to invite.</span></span>|
|<span data-ttu-id="a4b6e-131">适用</span><span class="sxs-lookup"><span data-stu-id="a4b6e-131">clientContext</span></span>|<span data-ttu-id="a4b6e-132">String</span><span class="sxs-lookup"><span data-stu-id="a4b6e-132">String</span></span>|<span data-ttu-id="a4b6e-133">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="a4b6e-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="a4b6e-134">响应</span><span class="sxs-lookup"><span data-stu-id="a4b6e-134">Response</span></span>
<span data-ttu-id="a4b6e-135">返回`202 Accepted`响应代码和位置标头, 其中包含为此请求创建的[commsOperation](../resources/commsoperation.md)的 uri。</span><span class="sxs-lookup"><span data-stu-id="a4b6e-135">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="examples"></a><span data-ttu-id="a4b6e-136">示例</span><span class="sxs-lookup"><span data-stu-id="a4b6e-136">Examples</span></span>
<span data-ttu-id="a4b6e-137">下面的示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="a4b6e-137">The following examples shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="a4b6e-138">请求</span><span class="sxs-lookup"><span data-stu-id="a4b6e-138">Request</span></span>
<span data-ttu-id="a4b6e-139">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="a4b6e-139">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "participant-invite"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/participants/invite
Content-Type: application/json
Content-Length: 464

{
  "participants": [
    {
      "endpointType": "default",
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "languageId": "languageId-value",
      "region": "region-value",
      "replacesCallId": "replacesCallId-value"
    }
  ],
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="a4b6e-140">响应</span><span class="sxs-lookup"><span data-stu-id="a4b6e-140">Response</span></span>

> <span data-ttu-id="a4b6e-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a4b6e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a4b6e-143">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="a4b6e-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a4b6e-144">C#</span><span class="sxs-lookup"><span data-stu-id="a4b6e-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/participant-invite-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a4b6e-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="a4b6e-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/participant-invite-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<br/>

### <a name="invite-participants-in-existing-p2p-meeting"></a><span data-ttu-id="a4b6e-146">邀请现有 P2P 会议中的参与者</span><span class="sxs-lookup"><span data-stu-id="a4b6e-146">Invite Participants in Existing P2P meeting</span></span>

##### <a name="request"></a><span data-ttu-id="a4b6e-147">请求</span><span class="sxs-lookup"><span data-stu-id="a4b6e-147">Request</span></span>

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants/invite
Content-Type: application/json

{
  "participants": [
    {
      "endpointType": "default",
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "languageId": "en-US",
      "region": "westus"
    }
  ],
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="response"></a><span data-ttu-id="a4b6e-148">响应</span><span class="sxs-lookup"><span data-stu-id="a4b6e-148">Response</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "running",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="a4b6e-149">通知-操作已完成</span><span class="sxs-lookup"><span data-stu-id="a4b6e-149">Notification - operation completed</span></span>

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
        "@odata.etag": "W/\"51\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "status": "completed"
      }
    }
  ]
}
```

##### <a name="notification---roster-updated-with-participant-added"></a><span data-ttu-id="a4b6e-150">已添加参与者的通知-名单</span><span class="sxs-lookup"><span data-stu-id="a4b6e-150">Notification - roster updated with participant added</span></span>

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
          "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants/8A34A46B3D174ADC8DCEDC4E7D572698",
          "@odata.etag": "W/\"51\"",
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
          ]
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants/123456W77E24E4D85F80597083CB830",
          "@odata.etag": "W/\"55\"",
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
          ]
        }
      ]
    }
  ]
}
```

### <a name="invite-participants-in-existing-p2p-meeting"></a><span data-ttu-id="a4b6e-151">邀请现有 P2P 会议中的参与者</span><span class="sxs-lookup"><span data-stu-id="a4b6e-151">Invite Participants in Existing P2P meeting</span></span>

<span data-ttu-id="a4b6e-152">本示例显示现有 P2P 会议中的[邀请参与者](../api/participant-invite.md)的完整 E2E 流。</span><span class="sxs-lookup"><span data-stu-id="a4b6e-152">This example shows a complete E2E flow for [Invite Participants](../api/participant-invite.md) in an existing P2P meeting.</span></span>

##### <a name="answer-incoming-voip-call-with-service-hosted-media"></a><span data-ttu-id="a4b6e-153">使用服务托管媒体应答传入 VOIP 呼叫</span><span class="sxs-lookup"><span data-stu-id="a4b6e-153">Answer Incoming VOIP call with service hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="a4b6e-154">通知传入</span><span class="sxs-lookup"><span data-stu-id="a4b6e-154">Notification - Incoming</span></span>

``` http
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
      "changeType": "created",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "incoming",
        "direction": "incoming",
        "source": {
          "@odata.type": "#microsoft.graph.participantInfo",
          "identity": {
            "user": {
              "displayName": "Test User",
              "language": "en-US",
              "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
            }
          }
        },
        "targets": [
          {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "application": {
                "displayName": "Test BOT",
                "language": "en-US",
                "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
              }
            }
          }
        ],
        "requestedModalities": [ "audio", "video" ]
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="a4b6e-155">请求</span><span class="sxs-lookup"><span data-stu-id="a4b6e-155">Request</span></span>

``` http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/answer
Authorization: Bearer <TOKEN>
Content-Type: application/json

{
  "callback": "https://bot.contoso.com/api/calls",
  "acceptModalities": [ "audio", "video" ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
      {
        "url": "https://cdn.contoso.com/beep.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      },
      {
        "url": "https://cdn.contoso.com/cool.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088F"
      }
    ]
  }
}
```

##### <a name="response"></a><span data-ttu-id="a4b6e-156">响应</span><span class="sxs-lookup"><span data-stu-id="a4b6e-156">Response</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 306

{
  "clientContext": "clientContext-value",
  "createdDateTime": "2018-03-19T09:46:02Z",
  "id": "id-value",
  "lastActionDateTime": "2018-03-19T09:46:02Z",
  "status": "Running"
}
```

##### <a name="notification---establishing"></a><span data-ttu-id="a4b6e-157">通知-建立</span><span class="sxs-lookup"><span data-stu-id="a4b6e-157">Notification - Establishing</span></span>

``` http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
``` json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "establishing"
      }
    }
  ]
}
```

##### <a name="notification---established"></a><span data-ttu-id="a4b6e-158">已建立通知</span><span class="sxs-lookup"><span data-stu-id="a4b6e-158">Notification - Established</span></span>

``` http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
``` json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "established",
        "activeModalities": [ "audio", "video" ],
        "requestedModalities": []
      }
    }
  ]
}
```

### <a name="join-channel-meeting-without-media"></a><span data-ttu-id="a4b6e-159">不带媒体的加入频道会议</span><span class="sxs-lookup"><span data-stu-id="a4b6e-159">Join channel meeting without media</span></span>

> <span data-ttu-id="a4b6e-160">**重要说明**: 如果 bot 实例只是为了便于传输而加入, 它应避免媒体协商。</span><span class="sxs-lookup"><span data-stu-id="a4b6e-160">**IMPORTANT**: If the bot instance is joining only for the purpose of facilitating the transfer, it should avoid media negotiations.</span></span>  <span data-ttu-id="a4b6e-161">因此, 最好在不添加任何`requestedModalities`或`mediaConfig`的情况下添加它。</span><span class="sxs-lookup"><span data-stu-id="a4b6e-161">Therefore, it is best to add it without any `requestedModalities` or `mediaConfig`.</span></span>

##### <a name="request"></a><span data-ttu-id="a4b6e-162">请求</span><span class="sxs-lookup"><span data-stu-id="a4b6e-162">Request</span></span>

``` http
POST /app/calls
Content-Type: application/json

{
  "subject": "Test Call",
  "callback": "https://bot.contoso.com/api/calls",
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "application": {
        "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
      }
    }
  },
  "targetDisposition": "default",
  "requestedModalities": [],
  "chatInfo": {
    "threadId": "90ED37DC-D8E3-4E11-9DE3-30A955DDA06F",
    "messageId": "1507228578052",
    "replyChainMessageId": "1507228578052"
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "user": {
        "id": "90ED37DC-D8E3-4E11-9DE3-30A955DDA06F",
        "tenantId": "49BFC225-8482-4AB8-94E7-76B48FDB9849"
      }
    }
  }
}
```

##### <a name="response"></a><span data-ttu-id="a4b6e-163">响应</span><span class="sxs-lookup"><span data-stu-id="a4b6e-163">Response</span></span>

``` http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/app/calls/90ED37DCD8E34E119DE330A955DDA06F
```

##### <a name="notification---establishing"></a><span data-ttu-id="a4b6e-164">通知-建立</span><span class="sxs-lookup"><span data-stu-id="a4b6e-164">Notification - Establishing</span></span>

``` http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
``` json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/90ED37DCD8E34E119DE330A955DDA06F",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/90ED37DCD8E34E119DE330A955DDA06F",
        "@odata.etag": "W/\"5445\"",
        "state": "establishing",
        "direction": "outgoing"
      }
    }
  ]
}
```

##### <a name="notification---established"></a><span data-ttu-id="a4b6e-165">已建立通知</span><span class="sxs-lookup"><span data-stu-id="a4b6e-165">Notification - Established</span></span>

``` http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
``` json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/90ED37DCD8E34E119DE330A955DDA06F",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/90ED37DCD8E34E119DE330A955DDA06F",
        "@odata.etag": "W/\"5445\"",
        "state": "established",
        "activeModalities": []
      }
    }
  ]
}
```

### <a name="invite-participant-from-initial-incoming-call"></a><span data-ttu-id="a4b6e-166">邀请参与者进入初始传入呼叫</span><span class="sxs-lookup"><span data-stu-id="a4b6e-166">Invite participant from initial incoming call</span></span>

``` http
POST /app/calls/90ED37DCD8E34E119DE330A955DDA06F/participants/invite
Authorization: Bearer <TOKEN>
Content-Type: application/json

{
  "participants": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "user": {
          "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
        }
      },
      "replacesCallId": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896"
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="a4b6e-167">响应</span><span class="sxs-lookup"><span data-stu-id="a4b6e-167">Response</span></span>

``` http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/app/calls/90ED37DCD8E34E119DE330A955DDA06F/operations/0FE0623FD62842EDB4BD8AC290072CC5
Content-Type: application/json
Content-Length: 306

{
  "clientContext": "clientContext-value",
  "createdDateTime": "2018-03-19T09:46:02Z",
  "id": "id-value",
  "lastActionDateTime": "2018-03-19T09:46:02Z",
  "status": "Running"
}
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="a4b6e-168">通知-操作已完成</span><span class="sxs-lookup"><span data-stu-id="a4b6e-168">Notification - Operation Completed</span></span>

``` http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
``` json
{
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/90ED37DCD8E34E119DE330A955DDA06F/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.inviteParticipantsOperation",
        "@odata.id": "/app/calls/90ED37DCD8E34E119DE330A955DDA06F/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"51\"",
        "clientContext": "A904FBD5A31041E881E861877A3DE3CD",
        "status": "completed"
      }
    }
  ]
}
```

##### <a name="notification---roster-updated-with-participant-added"></a><span data-ttu-id="a4b6e-169">已添加参与者的通知-名单</span><span class="sxs-lookup"><span data-stu-id="a4b6e-169">Notification - Roster Updated With Participant Added</span></span>

``` http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
``` json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants/8A34A46B3D174ADC8DCEDC4E7D572698",
          "@odata.etag": "W/\"51\"",
          "info": {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "user": {
                "region": "westus",
                "languageId": "en-US",
                "displayName": "Test User",
                "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
              }
            }
          },
          "mediaStreams": [
            {
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "1",
              "direction": "sendReceive"
            }
          ]
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants/123456W77E24E4D85F80597083CB830",
          "@odata.etag": "W/\"55\"",
          "info": {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "application": {
                "region": "westus",
                "languageId": "en-US",
                "displayName": "Test Bot",
                "id": "1234A46B-3D17-4ADC-8DCE-DC4E7D556789"
              }
            }
          },
          "mediaStreams": [
            {
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "2",
              "direction": "sendReceive"
            }
          ]
        }
      ]
    }
  ]
}
```

##### <a name="notification---terminated-the-original-p2p-call"></a><span data-ttu-id="a4b6e-170">通知-终止原始 P2P 呼叫</span><span class="sxs-lookup"><span data-stu-id="a4b6e-170">Notification - terminated the original P2P call</span></span>

``` http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
``` json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "terminated",
        "terminationReason": "AppInitiated"
      }
    }
  ]
}
```

##### <a name="notification---deleted-the-original-p2p-call"></a><span data-ttu-id="a4b6e-171">通知-已删除原始 P2P 呼叫</span><span class="sxs-lookup"><span data-stu-id="a4b6e-171">Notification - Deleted the original P2P call</span></span>

``` http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
``` json
{
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\""
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
  "description": "participant: invite",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/participant-invite.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/participant-invite.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
