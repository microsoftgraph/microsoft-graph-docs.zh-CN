---
title: 参与者： 邀请
description: 邀请参与者加入活动呼叫。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 50c9ebd30bf70290006d8c04ccfb29e09ce0d566
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510167"
---
# <a name="participant-invite"></a><span data-ttu-id="6c854-103">参与者： 邀请</span><span class="sxs-lookup"><span data-stu-id="6c854-103">participant: invite</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c854-104">邀请参与者加入活动呼叫。</span><span class="sxs-lookup"><span data-stu-id="6c854-104">Invite participants to the active call.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c854-105">权限</span><span class="sxs-lookup"><span data-stu-id="6c854-105">Permissions</span></span>
<span data-ttu-id="6c854-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6c854-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6c854-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6c854-108">Permission type</span></span> | <span data-ttu-id="6c854-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6c854-109">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="6c854-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6c854-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6c854-111">不支持</span><span class="sxs-lookup"><span data-stu-id="6c854-111">Not Supported</span></span>                       |
| <span data-ttu-id="6c854-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6c854-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c854-113">不支持</span><span class="sxs-lookup"><span data-stu-id="6c854-113">Not Supported</span></span>                       |
| <span data-ttu-id="6c854-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6c854-114">Application</span></span>     | <span data-ttu-id="6c854-115">Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="6c854-115">Calls.InitiateGroupCalls.All</span></span>                               |

## <a name="http-request"></a><span data-ttu-id="6c854-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6c854-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/invite
POST /applications/{id}/calls/{id}/participants/invite
```

## <a name="request-headers"></a><span data-ttu-id="6c854-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="6c854-117">Request headers</span></span>
| <span data-ttu-id="6c854-118">名称</span><span class="sxs-lookup"><span data-stu-id="6c854-118">Name</span></span>          | <span data-ttu-id="6c854-119">说明</span><span class="sxs-lookup"><span data-stu-id="6c854-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="6c854-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c854-120">Authorization</span></span> | <span data-ttu-id="6c854-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6c854-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c854-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="6c854-123">Request body</span></span>
<span data-ttu-id="6c854-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="6c854-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6c854-125">参数</span><span class="sxs-lookup"><span data-stu-id="6c854-125">Parameter</span></span>      | <span data-ttu-id="6c854-126">类型</span><span class="sxs-lookup"><span data-stu-id="6c854-126">Type</span></span>    |<span data-ttu-id="6c854-127">说明</span><span class="sxs-lookup"><span data-stu-id="6c854-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c854-128">participants</span><span class="sxs-lookup"><span data-stu-id="6c854-128">participants</span></span>|<span data-ttu-id="6c854-129">[invitationParticipantInfo](../resources/invitationparticipantinfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="6c854-129">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>| <span data-ttu-id="6c854-130">邀请参与者。</span><span class="sxs-lookup"><span data-stu-id="6c854-130">The participants to invite.</span></span>|
|<span data-ttu-id="6c854-131">ClientContext</span><span class="sxs-lookup"><span data-stu-id="6c854-131">clientContext</span></span>|<span data-ttu-id="6c854-132">String</span><span class="sxs-lookup"><span data-stu-id="6c854-132">String</span></span>|<span data-ttu-id="6c854-133">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="6c854-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="6c854-134">响应</span><span class="sxs-lookup"><span data-stu-id="6c854-134">Response</span></span>
<span data-ttu-id="6c854-135">返回`202 Accepted`响应代码和具有[commsOperation](../resources/commsoperation.md)创建的此请求 uri 中的位置标头。</span><span class="sxs-lookup"><span data-stu-id="6c854-135">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="examples"></a><span data-ttu-id="6c854-136">示例</span><span class="sxs-lookup"><span data-stu-id="6c854-136">Examples</span></span>
<span data-ttu-id="6c854-137">下面的示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="6c854-137">The following examples shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="6c854-138">请求</span><span class="sxs-lookup"><span data-stu-id="6c854-138">Request</span></span>
<span data-ttu-id="6c854-139">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="6c854-139">The following example shows the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="6c854-140">响应</span><span class="sxs-lookup"><span data-stu-id="6c854-140">Response</span></span>

> <span data-ttu-id="6c854-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6c854-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

```
<br/>

### <a name="invite-participants-in-existing-p2p-meeting"></a><span data-ttu-id="6c854-143">邀请中现有的 P2P 会议的参与者</span><span class="sxs-lookup"><span data-stu-id="6c854-143">Invite Participants in Existing P2P meeting</span></span>

##### <a name="request"></a><span data-ttu-id="6c854-144">请求</span><span class="sxs-lookup"><span data-stu-id="6c854-144">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="6c854-145">响应</span><span class="sxs-lookup"><span data-stu-id="6c854-145">Response</span></span>

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

##### <a name="notification---operation-completed"></a><span data-ttu-id="6c854-146">通知-完成的操作</span><span class="sxs-lookup"><span data-stu-id="6c854-146">Notification - operation completed</span></span>

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

##### <a name="notification---roster-updated-with-participant-added"></a><span data-ttu-id="6c854-147">通知-添加参与者使用更新的名单</span><span class="sxs-lookup"><span data-stu-id="6c854-147">Notification - roster updated with participant added</span></span>

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

### <a name="invite-participants-in-existing-p2p-meeting"></a><span data-ttu-id="6c854-148">邀请中现有的 P2P 会议的参与者</span><span class="sxs-lookup"><span data-stu-id="6c854-148">Invite Participants in Existing P2P meeting</span></span>

<span data-ttu-id="6c854-149">本示例在现有 P2P 会议[邀请](../api/participant-invite.md)参与者演示完整的 E2E 流。</span><span class="sxs-lookup"><span data-stu-id="6c854-149">This example shows a complete E2E flow for [Invite Participants](../api/participant-invite.md) in an existing P2P meeting.</span></span>

##### <a name="answer-incoming-voip-call-with-service-hosted-media"></a><span data-ttu-id="6c854-150">应答传入的 VOIP 呼叫与服务承载媒体</span><span class="sxs-lookup"><span data-stu-id="6c854-150">Answer Incoming VOIP call with service hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="6c854-151">通知-传入</span><span class="sxs-lookup"><span data-stu-id="6c854-151">Notification - Incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="6c854-152">请求</span><span class="sxs-lookup"><span data-stu-id="6c854-152">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="6c854-153">响应</span><span class="sxs-lookup"><span data-stu-id="6c854-153">Response</span></span>

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

##### <a name="notification---establishing"></a><span data-ttu-id="6c854-154">通知-建立</span><span class="sxs-lookup"><span data-stu-id="6c854-154">Notification - Establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="6c854-155">通知-建立</span><span class="sxs-lookup"><span data-stu-id="6c854-155">Notification - Established</span></span>

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

### <a name="join-channel-meeting-without-media"></a><span data-ttu-id="6c854-156">加入没有媒体通道会议</span><span class="sxs-lookup"><span data-stu-id="6c854-156">Join channel meeting without media</span></span>

> <span data-ttu-id="6c854-157">**重要说明**： 如果仅以促成转接中加入自动程序实例，它应避免媒体协商。</span><span class="sxs-lookup"><span data-stu-id="6c854-157">**IMPORTANT**: If the bot instance is joining only for the purpose of facilitating the transfer, it should avoid media negotiations.</span></span>  <span data-ttu-id="6c854-158">因此，最好将其添加没有任何`requestedModalities`或`mediaConfig`。</span><span class="sxs-lookup"><span data-stu-id="6c854-158">Therefore, it is best to add it without any `requestedModalities` or `mediaConfig`.</span></span>

##### <a name="request"></a><span data-ttu-id="6c854-159">请求</span><span class="sxs-lookup"><span data-stu-id="6c854-159">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="6c854-160">响应</span><span class="sxs-lookup"><span data-stu-id="6c854-160">Response</span></span>

``` http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/app/calls/90ED37DCD8E34E119DE330A955DDA06F
```

##### <a name="notification---establishing"></a><span data-ttu-id="6c854-161">通知-建立</span><span class="sxs-lookup"><span data-stu-id="6c854-161">Notification - Establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="6c854-162">通知-建立</span><span class="sxs-lookup"><span data-stu-id="6c854-162">Notification - Established</span></span>

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

### <a name="invite-participant-from-initial-incoming-call"></a><span data-ttu-id="6c854-163">邀请参与者从初始的传入呼叫</span><span class="sxs-lookup"><span data-stu-id="6c854-163">Invite participant from initial incoming call</span></span>

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

##### <a name="response"></a><span data-ttu-id="6c854-164">响应</span><span class="sxs-lookup"><span data-stu-id="6c854-164">Response</span></span>

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

##### <a name="notification---operation-completed"></a><span data-ttu-id="6c854-165">通知-完成的操作</span><span class="sxs-lookup"><span data-stu-id="6c854-165">Notification - Operation Completed</span></span>

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

##### <a name="notification---roster-updated-with-participant-added"></a><span data-ttu-id="6c854-166">通知-添加参与者使用更新的名单</span><span class="sxs-lookup"><span data-stu-id="6c854-166">Notification - Roster Updated With Participant Added</span></span>

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

##### <a name="notification---terminated-the-original-p2p-call"></a><span data-ttu-id="6c854-167">通知-终止原始 P2P 呼叫</span><span class="sxs-lookup"><span data-stu-id="6c854-167">Notification - terminated the original P2P call</span></span>

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

##### <a name="notification---deleted-the-original-p2p-call"></a><span data-ttu-id="6c854-168">通知-删除原始的 P2P 呼叫</span><span class="sxs-lookup"><span data-stu-id="6c854-168">Notification - Deleted the original P2P call</span></span>

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
    "Error: /api-reference/beta/api/participant-invite.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
