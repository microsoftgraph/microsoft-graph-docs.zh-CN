---
title: 参与者：邀请
description: 邀请参与者加入活动呼叫。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: aa463a7b300cfc4f3e6a8ad27bf2a7344b41c09d
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792518"
---
# <a name="participant-invite"></a><span data-ttu-id="8e64c-103">参与者：邀请</span><span class="sxs-lookup"><span data-stu-id="8e64c-103">participant: invite</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e64c-104">邀请参与者加入活动的多方呼叫。</span><span class="sxs-lookup"><span data-stu-id="8e64c-104">Invite participants to the active multiparty call.</span></span>

<span data-ttu-id="8e64c-105">有关如何处理长时间运行的参与者邀请操作的详细信息，请参阅[inviteParticipantsOperation](../resources/inviteparticipantsoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="8e64c-105">For more information about how to handle long-running participant invitation operations, see [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md).</span></span>

><span data-ttu-id="8e64c-106">**注意：** 此 API 仅支持多方调用。</span><span class="sxs-lookup"><span data-stu-id="8e64c-106">**Note:** This API is only supported for multiparty calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e64c-107">权限</span><span class="sxs-lookup"><span data-stu-id="8e64c-107">Permissions</span></span>
<span data-ttu-id="8e64c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8e64c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8e64c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8e64c-110">Permission type</span></span> | <span data-ttu-id="8e64c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8e64c-111">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="8e64c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8e64c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="8e64c-113">不支持</span><span class="sxs-lookup"><span data-stu-id="8e64c-113">Not Supported</span></span>                       |
| <span data-ttu-id="8e64c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8e64c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e64c-115">不支持</span><span class="sxs-lookup"><span data-stu-id="8e64c-115">Not Supported</span></span>                       |
| <span data-ttu-id="8e64c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8e64c-116">Application</span></span>     | <span data-ttu-id="8e64c-117">InitiateGroupCalls</span><span class="sxs-lookup"><span data-stu-id="8e64c-117">Calls.InitiateGroupCalls.All</span></span>                               |

## <a name="http-request"></a><span data-ttu-id="8e64c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8e64c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/invite
```

## <a name="request-headers"></a><span data-ttu-id="8e64c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8e64c-119">Request headers</span></span>
| <span data-ttu-id="8e64c-120">名称</span><span class="sxs-lookup"><span data-stu-id="8e64c-120">Name</span></span>          | <span data-ttu-id="8e64c-121">说明</span><span class="sxs-lookup"><span data-stu-id="8e64c-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8e64c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e64c-122">Authorization</span></span> | <span data-ttu-id="8e64c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8e64c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e64c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="8e64c-125">Request body</span></span>
<span data-ttu-id="8e64c-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="8e64c-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8e64c-127">参数</span><span class="sxs-lookup"><span data-stu-id="8e64c-127">Parameter</span></span>      | <span data-ttu-id="8e64c-128">类型</span><span class="sxs-lookup"><span data-stu-id="8e64c-128">Type</span></span>    |<span data-ttu-id="8e64c-129">说明</span><span class="sxs-lookup"><span data-stu-id="8e64c-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e64c-130">participants</span><span class="sxs-lookup"><span data-stu-id="8e64c-130">participants</span></span>|<span data-ttu-id="8e64c-131">[invitationParticipantInfo](../resources/invitationparticipantinfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="8e64c-131">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>| <span data-ttu-id="8e64c-132">要邀请的参与者。</span><span class="sxs-lookup"><span data-stu-id="8e64c-132">The participants to invite.</span></span>|
|<span data-ttu-id="8e64c-133">适用</span><span class="sxs-lookup"><span data-stu-id="8e64c-133">clientContext</span></span>|<span data-ttu-id="8e64c-134">String</span><span class="sxs-lookup"><span data-stu-id="8e64c-134">String</span></span>|<span data-ttu-id="8e64c-135">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="8e64c-135">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="8e64c-136">响应</span><span class="sxs-lookup"><span data-stu-id="8e64c-136">Response</span></span>
<span data-ttu-id="8e64c-137">如果成功，此 API 将返回`202 Accepted`响应代码和位置标头，其中包含为此请求创建的[INVITEPARTICIPANTSOPERATION](../resources/inviteparticipantsoperation.md)对象的 URI。</span><span class="sxs-lookup"><span data-stu-id="8e64c-137">If successful, this API returns a `202 Accepted` response code and a Location header with a URI to the [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) object created for this request.</span></span> <span data-ttu-id="8e64c-138">响应正文包含创建的[inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) 。</span><span class="sxs-lookup"><span data-stu-id="8e64c-138">The body of the response contains the [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) created.</span></span>

## <a name="examples"></a><span data-ttu-id="8e64c-139">示例</span><span class="sxs-lookup"><span data-stu-id="8e64c-139">Examples</span></span>
<span data-ttu-id="8e64c-140">下面的示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="8e64c-140">The following examples shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="8e64c-141">请求</span><span class="sxs-lookup"><span data-stu-id="8e64c-141">Request</span></span>
<span data-ttu-id="8e64c-142">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="8e64c-142">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8e64c-143">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="8e64c-143">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="8e64c-144">C#</span><span class="sxs-lookup"><span data-stu-id="8e64c-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8e64c-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e64c-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8e64c-146">目标-C</span><span class="sxs-lookup"><span data-stu-id="8e64c-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8e64c-147">响应</span><span class="sxs-lookup"><span data-stu-id="8e64c-147">Response</span></span>

> <span data-ttu-id="8e64c-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8e64c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inviteParticipantsOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
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
<br/>

## <a name="example---invite-participants-to-an-existing-multiparty-call"></a><span data-ttu-id="8e64c-150">示例-邀请参与者加入现有的多方呼叫</span><span class="sxs-lookup"><span data-stu-id="8e64c-150">Example - Invite participants to an existing multiparty call</span></span>

##### <a name="request"></a><span data-ttu-id="8e64c-151">请求</span><span class="sxs-lookup"><span data-stu-id="8e64c-151">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="8e64c-152">响应</span><span class="sxs-lookup"><span data-stu-id="8e64c-152">Response</span></span>

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

##### <a name="notification---operation-completed"></a><span data-ttu-id="8e64c-153">通知-操作已完成</span><span class="sxs-lookup"><span data-stu-id="8e64c-153">Notification - operation completed</span></span>

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
  "@odata.type": "microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.inviteParticipantsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"51\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "status": "completed"
      }
    }
  ]
}
```

##### <a name="notification---roster-updated-with-participant-added"></a><span data-ttu-id="8e64c-154">已添加参与者的通知-名单</span><span class="sxs-lookup"><span data-stu-id="8e64c-154">Notification - roster updated with participant added</span></span>

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
  "@odata.type": "microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "microsoft.graph.commsNotification",
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

## <a name="example---invite-participants-to-a-multiparty-call-replacing-an-existing-peer-to-peer-call"></a><span data-ttu-id="8e64c-155">示例-邀请参与者加入多方呼叫，替换现有的对等呼叫</span><span class="sxs-lookup"><span data-stu-id="8e64c-155">Example - Invite participants to a multiparty call, replacing an existing peer-to-peer call</span></span>

<span data-ttu-id="8e64c-156">本示例假定已在 bot 和 ID `8A34A46B-3D17-4ADC-8DCE-DC4E7D572698`为的用户之间建立了现有的对等呼叫，我们希望在结束对等呼叫时，机器人将用户邀请用户加入到现有的多方呼叫中。</span><span class="sxs-lookup"><span data-stu-id="8e64c-156">This example assumes an existing peer-to-peer call has been established between the bot and user with ID `8A34A46B-3D17-4ADC-8DCE-DC4E7D572698`, and we'd like the bot to invite the user into an existing multiparty call while ending the peer-to-peer call.</span></span>

<span data-ttu-id="8e64c-157">有关使用`replacesCallId`替换现有的对等呼叫的详细信息，请参阅[邀请参与者](../resources/invitationparticipantinfo.md)。</span><span class="sxs-lookup"><span data-stu-id="8e64c-157">For details on using `replacesCallId` to replace an existing peer-to-peer call, see [Invitation Participant](../resources/invitationparticipantinfo.md).</span></span>

##### <a name="request"></a><span data-ttu-id="8e64c-158">请求</span><span class="sxs-lookup"><span data-stu-id="8e64c-158">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="8e64c-159">响应</span><span class="sxs-lookup"><span data-stu-id="8e64c-159">Response</span></span>

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

##### <a name="notification---operation-completed"></a><span data-ttu-id="8e64c-160">通知-操作已完成</span><span class="sxs-lookup"><span data-stu-id="8e64c-160">Notification - Operation completed</span></span>

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
  "@odata.type": "microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "microsoft.graph.commsNotification",
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

##### <a name="notification---roster-updated-with-participant-added"></a><span data-ttu-id="8e64c-161">已添加参与者的通知-名单</span><span class="sxs-lookup"><span data-stu-id="8e64c-161">Notification - Roster updated with participant added</span></span>

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
  "@odata.type": "microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "microsoft.graph.commsNotification",
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

##### <a name="notification---terminated-the-original-peer-to-peer-call"></a><span data-ttu-id="8e64c-162">Notification-终止原始的对等呼叫</span><span class="sxs-lookup"><span data-stu-id="8e64c-162">Notification - Terminated the original peer-to-peer call</span></span>

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
  "@odata.type": "microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "microsoft.graph.commsNotification",
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

##### <a name="notification---deleted-the-original-peer-to-peer-call"></a><span data-ttu-id="8e64c-163">Notification-已删除原始的对等呼叫</span><span class="sxs-lookup"><span data-stu-id="8e64c-163">Notification - Deleted the original peer-to-peer call</span></span>

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
  "@odata.type": "microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "microsoft.graph.commsNotification",
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

## <a name="example---invite-participant-failure"></a><span data-ttu-id="8e64c-164">示例-邀请参与者失败</span><span class="sxs-lookup"><span data-stu-id="8e64c-164">Example - Invite Participant Failure</span></span>

<span data-ttu-id="8e64c-165">在邀请参与者操作失败的情况下，bot 将收到通知，并将[inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) `status`设置为`failed`。</span><span class="sxs-lookup"><span data-stu-id="8e64c-165">In the event the invite participant operation fails, the bot will receive a notification with the [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) with `status` set to `failed`.</span></span>

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
  "@odata.type": "microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resource": "/app/calls/90ED37DCD8E34E119DE330A955DDA06F/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.inviteParticipantsOperation",
        "@odata.id": "/app/calls/90ED37DCD8E34E119DE330A955DDA06F/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"51\"",
        "clientContext": "A904FBD5A31041E881E861877A3DE3CD",
        "status": "failed",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": 500,
          "subCode": 0,
          "message": "addParticipantsfailed for participants: 28:8A34A46B-3D17-4ADC-8DCE-DC4E7D572698 reason: Audio-video modality controller could not invite participant to this conversation., code=580 subcode=5201"
        },
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
  ]
}
-->
