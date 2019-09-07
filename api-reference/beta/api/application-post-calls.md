---
title: 创建调用
description: 创建新呼叫。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 28496a8ed236c3dc5ef43b5a592caf953e8b2d6c
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791141"
---
# <a name="create-call"></a><span data-ttu-id="78008-103">创建调用</span><span class="sxs-lookup"><span data-stu-id="78008-103">Create call</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78008-104">"创建[呼叫](../resources/call.md)" 使你的 bot 能够创建新的传出呼叫或加入现有会议。</span><span class="sxs-lookup"><span data-stu-id="78008-104">Create [call](../resources/call.md) enables your bot to create a new outgoing call or join an existing meeting.</span></span> <span data-ttu-id="78008-105">你需要[注册呼叫机器人](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot)并查看所需的权限列表，如下所述。</span><span class="sxs-lookup"><span data-stu-id="78008-105">You will need to [register the calling bot](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot) and go through the list of permissions needed as mentioned below.</span></span>


## <a name="permissions"></a><span data-ttu-id="78008-106">权限</span><span class="sxs-lookup"><span data-stu-id="78008-106">Permissions</span></span>
<span data-ttu-id="78008-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot#add-microsoft-graph-permissions)。</span><span class="sxs-lookup"><span data-stu-id="78008-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot#add-microsoft-graph-permissions).</span></span>

| <span data-ttu-id="78008-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="78008-109">Permission type</span></span>                        | <span data-ttu-id="78008-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="78008-110">Permissions (from least to most privileged)</span></span>                                             |
|:---------------------------------------|:----------------------------------------------------------------------------------------|
| <span data-ttu-id="78008-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="78008-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="78008-112">不支持</span><span class="sxs-lookup"><span data-stu-id="78008-112">Not Supported</span></span>                                                                           |
| <span data-ttu-id="78008-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="78008-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78008-114">不支持</span><span class="sxs-lookup"><span data-stu-id="78008-114">Not Supported</span></span>                                                                           |
| <span data-ttu-id="78008-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="78008-115">Application</span></span>                            | <span data-ttu-id="78008-116">JoinGroupCallsasGuest、JoinGroupCalls、calls、InitiateGroupCalls、All、和。</span><span class="sxs-lookup"><span data-stu-id="78008-116">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All</span></span> |

> <span data-ttu-id="78008-117">**注意：** 此外，对于具有应用托管媒体的呼叫，您需要 AccessMedia 权限。</span><span class="sxs-lookup"><span data-stu-id="78008-117">**Note:** In addition, for a call with app hosted media, you need the Calls.AccessMedia.All permission.</span></span>

## <a name="http-request"></a><span data-ttu-id="78008-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="78008-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls
```

## <a name="request-headers"></a><span data-ttu-id="78008-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="78008-119">Request headers</span></span>
| <span data-ttu-id="78008-120">名称</span><span class="sxs-lookup"><span data-stu-id="78008-120">Name</span></span>          | <span data-ttu-id="78008-121">说明</span><span class="sxs-lookup"><span data-stu-id="78008-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="78008-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="78008-122">Authorization</span></span> | <span data-ttu-id="78008-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="78008-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="78008-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="78008-125">Request body</span></span>
<span data-ttu-id="78008-126">在请求正文中，提供[call](../resources/call.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="78008-126">In the request body, supply a JSON representation of a [call](../resources/call.md) object.</span></span>

> <span data-ttu-id="78008-127">**注意：** 在`Server generated` `app/calls`处理`POST`时，被标记为的属性将被忽略。</span><span class="sxs-lookup"><span data-stu-id="78008-127">**Note:** Properties marked as `Server generated` are ignored when processing `POST` on `app/calls`.</span></span>

## <a name="response"></a><span data-ttu-id="78008-128">响应</span><span class="sxs-lookup"><span data-stu-id="78008-128">Response</span></span>
<span data-ttu-id="78008-129">如果成功，此方法在响应`201 Created`正文中返回响应代码和[call](../resources/call.md)对象。</span><span class="sxs-lookup"><span data-stu-id="78008-129">If successful, this method returns a `201 Created` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="78008-130">示例</span><span class="sxs-lookup"><span data-stu-id="78008-130">Examples</span></span>

### <a name="create-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="78008-131">使用服务托管媒体创建对等 VOIP 呼叫</span><span class="sxs-lookup"><span data-stu-id="78008-131">Create peer to peer VOIP call with service hosted media</span></span>

> <span data-ttu-id="78008-132">**注意：** 此调用需要调用. Initiate。 All 权限。</span><span class="sxs-lookup"><span data-stu-id="78008-132">**Note:** This call needs the Calls.Initiate.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="78008-133">请求</span><span class="sxs-lookup"><span data-stu-id="78008-133">Request</span></span>
<span data-ttu-id="78008-134">以下示例显示了在 bot 和指定用户之间建立对等呼叫的请求。</span><span class="sxs-lookup"><span data-stu-id="78008-134">The following example shows the request which makes a peer to peer call between the bot and the specified user.</span></span> <span data-ttu-id="78008-135">在此示例中，媒体由服务托管。</span><span class="sxs-lookup"><span data-stu-id="78008-135">In this example the media is hosted by the service.</span></span> <span data-ttu-id="78008-136">必须使用实际值替换授权令牌、回调 url、应用程序 id、应用程序名称、用户 id、用户名和租户 id 的值，以使示例正常工作。</span><span class="sxs-lookup"><span data-stu-id="78008-136">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced with actual values to make the example work.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="78008-137">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="78008-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-call-from-application"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
Authorization: Bearer <Token>

{
  "@odata.type": "#microsoft.graph.call",
  "callbackUri": "https://bot.contoso.com/callback",
  "targets": [
    {
      "@odata.type": "#microsoft.graph.participantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "John",
          "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
        }
      }
    }
  ],
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
  }
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="78008-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="78008-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-call-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="78008-139">响应</span><span class="sxs-lookup"><span data-stu-id="78008-139">Response</span></span>

> <span data-ttu-id="78008-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="78008-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/app/calls/2e1a0b00-2db4-4022-9570-243709c565ab
Content-Type: application/json


{
  "@odata.type": "#microsoft.graph.call",
  "state": "establishing",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "callRoutes": [],
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "application": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "2891555a-92ff-42e6-80fa-6e1300c6b5c6",
      }
    },
    "region": null,
    "languageId": null
  },
  "targets": [
    {
      "@odata.type": "#microsoft.graph.participantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "John",
          "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
        }
      },
      "region": null,
      "languageId": null
    }
  ],
  "requestedModalities": [
    "audio"
  ],
  "activeModalities": [],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
     {
       "uri": "https://cdn.contoso.com/beep.wav",
       "resourceId": "f8971b04-b53e-418c-9222-c82ce681a582"
     },
     {
       "uri": "https://cdn.contoso.com/cool.wav",
       "resourceId": "86dc814b-c172-4428-9112-60f8ecae1edb"
     }
    ],
  },
  "routingPolicies": [],
  "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
  "myParticipantId": "499ff390-7a72-40e8-83a0-8fac6295ae7e",
  "id": "2e1a0b00-2db4-4022-9570-243709c565ab",
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#app/calls/$entity",
  "subject": null,
  "terminationReason": null,
  "ringingTimeoutInSeconds": null,
  "mediaState": null,
  "resultInfo": null,
  "answeredBy": null,
  "chatInfo": null,
  "meetingInfo": null,
  "meetingCapability": null,
  "toneInfo": null
}
```

##### <a name="notification---establishing"></a><span data-ttu-id="78008-142">通知-建立</span><span class="sxs-lookup"><span data-stu-id="78008-142">Notification - establishing</span></span>

```http
POST https://bot.contoso.com/callback
Authorization: Bearer <TOKEN>
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
      "resource": "/app/calls/2e1a0b00-2db4-4022-9570-243709c565ab",
      "callbackUri": "https://bot.contoso.com/callback",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "establishing",
        "id": "2e1a0b00-2db4-4022-9570-243709c565ab"
      }
    }
  ]
}
```
##### <a name="notification---established"></a><span data-ttu-id="78008-143">已建立通知</span><span class="sxs-lookup"><span data-stu-id="78008-143">Notification - established</span></span>

```http
POST https://bot.contoso.com/callback
Authorization: Bearer <TOKEN>
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
      "resource": "/app/calls/2e1a0b00-b3c5-4b0f-99b3-c133bc1e6116",
      "callbackUri": "https://bot.contoso.com/callback",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "established",
        "direction": "outgoing",
        "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
        "id": "2e1a0b00-b3c5-4b0f-99b3-c133bc1e6116"
      }
    }
  ]
}
```

### <a name="create-peer-to-peer-voip-call-with-application-hosted-media"></a><span data-ttu-id="78008-144">使用应用程序托管媒体创建对等 VOIP 呼叫</span><span class="sxs-lookup"><span data-stu-id="78008-144">Create peer to peer VOIP call with application hosted media</span></span>

> <span data-ttu-id="78008-145">注意：需要调用. Initiate. All 和 AccessMedia 权限。</span><span class="sxs-lookup"><span data-stu-id="78008-145">Note: Needs Calls.Initiate.All and Calls.AccessMedia.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="78008-146">请求</span><span class="sxs-lookup"><span data-stu-id="78008-146">Request</span></span>
<span data-ttu-id="78008-147">以下示例显示了在 bot 和指定用户之间建立对等呼叫的请求。</span><span class="sxs-lookup"><span data-stu-id="78008-147">The following example shows the request which makes a peer to peer call between the bot and the specified user.</span></span> <span data-ttu-id="78008-148">在此示例中，媒体由应用程序本地承载。</span><span class="sxs-lookup"><span data-stu-id="78008-148">In this example the media is hosted locally by the application.</span></span> <span data-ttu-id="78008-149">必须使用实际值替换授权令牌、回调 url、应用程序 id、应用程序名称、用户 id、用户名和租户 id 的值，以使示例正常工作。</span><span class="sxs-lookup"><span data-stu-id="78008-149">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced with actual values to make the example work.</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
Authorization: Bearer <Token>
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "@odata.type": "#microsoft.graph.call",
  "callbackUri": "https://bot.contoso.com/callback",
  "targets": [
    {
      "@odata.type": "#microsoft.graph.participantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "John",
          "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
        }
      }
    }
  ],
  "requestedModalities": [
    "audio"
  ],
 "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<Media Session Configuration>",
  }
}
```
<span data-ttu-id="78008-150">`<Media Session Configuration>`是序列化的媒体会话配置，其中包含媒体堆栈的会话信息。</span><span class="sxs-lookup"><span data-stu-id="78008-150">`<Media Session Configuration>` is the serialized media session configuration which contains the session information of the media stack.</span></span> <span data-ttu-id="78008-151">应在此处传递有关音频、视频、VBSS ssession 信息的特定信息。</span><span class="sxs-lookup"><span data-stu-id="78008-151">Specific information about audio, video, VBSS ssession information should be passed here.</span></span>

<span data-ttu-id="78008-152">示例音频媒体会话 blob 如下所示</span><span class="sxs-lookup"><span data-stu-id="78008-152">Sample audio media session blob is shown below</span></span>
```json
{\"mpUri\":\"net.tcp://bot.contoso.com:18732/MediaProcessor\",\"audioRenderContexts\":[\"14778cc4-f54c-43c7-989f-9092e34ef784\"],\"videoRenderContexts\":[],\"audioSourceContexts\":[\"a5dcfc9b-5a54-48ef-86f5-1fdd8508741a\"],\"videoSourceContexts\":[],\"dataRenderContexts\":null,\"dataSourceContexts\":null,\"supportedAudioFormat\":\"Pcm16K\",\"videoSinkEncodingFormats\":[],\"mpMediaSessionId\":\"2379cf46-acf3-4fef-a914-be9627075320\",\"regionAffinity\":null,\"skypeMediaBotsVersion\":\"1.11.1.0086\",\"mediaStackVersion\":\"2018.53.1.1\",\"mpVersion\":\"7.2.0.3881\",\"callId\":\"1b69b141-7f1a-4033-9c34-202737190a20\"}
```

><span data-ttu-id="78008-153">**注意：** 对于点对点呼叫，预期的通知仅适用于呼叫状态更改。</span><span class="sxs-lookup"><span data-stu-id="78008-153">**Note:** For peer to peer calls, the expected notifications are for call state changes only.</span></span>

### <a name="join-scheduled-meeting-with-service-hosted-media"></a><span data-ttu-id="78008-154">加入服务托管媒体的计划会议</span><span class="sxs-lookup"><span data-stu-id="78008-154">Join scheduled meeting with service hosted media</span></span>
<span data-ttu-id="78008-155">若要加入计划的会议，我们需要获取线程 id、邮件 id、组织者 id 以及在其中安排会议的租户 id。</span><span class="sxs-lookup"><span data-stu-id="78008-155">To join the scheduled meeting we will need to get the thread id, message id, organizer id and the tenant id in which the meeting is scheduled.</span></span>
<span data-ttu-id="78008-156">可以从[获取联机会议 API](../api/onlinemeeting-get.md)获取此信息。</span><span class="sxs-lookup"><span data-stu-id="78008-156">This information can be obtained from [Get Online Meetings API](../api/onlinemeeting-get.md).</span></span>

<span data-ttu-id="78008-157">授权令牌、回调 url、应用程序 id、应用程序名称、用户 id、用户名和租户 id 的值必须替换为通过获取具有实际值的[联机会议 API](../api/onlinemeeting-get.md)获取的详细信息，以使示例正常工作。</span><span class="sxs-lookup"><span data-stu-id="78008-157">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced along with the details obtained from  [Get Online Meetings API](../api/onlinemeeting-get.md) with actual values to make the example work.</span></span>
> <span data-ttu-id="78008-158">**注意：** 此示例需要该`Calls.JoinGroupCalls.All`权限。</span><span class="sxs-lookup"><span data-stu-id="78008-158">**Note:** This example needs the `Calls.JoinGroupCalls.All` permission.</span></span>

##### <a name="request"></a><span data-ttu-id="78008-159">请求</span><span class="sxs-lookup"><span data-stu-id="78008-159">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
Authorization: Bearer <Token>
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "@odata.type": "#microsoft.graph.call",
  "callbackUri": "https://bot.contoso.com/callback",
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
     {
       "uri": "https://cdn.contoso.com/beep.wav",
       "resourceId": "f8971b04-b53e-418c-9222-c82ce681a582"
     },
     {
       "uri": "https://cdn.contoso.com/cool.wav",
       "resourceId": "86dc814b-c172-4428-9112-60f8ecae1edb"
     }
    ],
  },
  "chatInfo": {
    "@odata.type": "#microsoft.graph.chatInfo",
    "threadId": "19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2",
    "messageId": "0"
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "@odata.type": "#microsoft.graph.identitySet",
      "user": {
        "@odata.type": "#microsoft.graph.identity",
        "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
        "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
        "displayName": "Bob"
      }
    },
    "allowConversationWithoutHost": true
  }
}
```
##### <a name="response"></a><span data-ttu-id="78008-160">响应</span><span class="sxs-lookup"><span data-stu-id="78008-160">Response</span></span>

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/app/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "truncated": "true",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "@odata.type": "#microsoft.graph.call",
  "state": "establishing",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "callRoutes": [],
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "application": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "2891555a-92ff-42e6-80fa-6e1300c6b5c6",
      }
    },
    "region": null,
    "languageId": null
  },
  "targets": [],
  "requestedModalities": [
    "audio"
  ],
  "activeModalities": [],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
     {
       "uri": "https://cdn.contoso.com/beep.wav",
       "resourceId": "f8971b04-b53e-418c-9222-c82ce681a582"
     },
     {
       "uri": "https://cdn.contoso.com/cool.wav",
       "resourceId": "86dc814b-c172-4428-9112-60f8ecae1edb"
     }
    ],
  },
  "chatInfo": {
    "@odata.type": "#microsoft.graph.chatInfo",
    "threadId": "19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2",
    "messageId": "0",
    "replyChainMessageId": null
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "@odata.type": "#microsoft.graph.identitySet",
      "user": {
        "@odata.type": "#microsoft.graph.identity",
        "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
        "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
        "displayName": "Bob"
      }
    },
    "allowConversationWithoutHost": true
  },
  "routingPolicies": [],
  "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
  "myParticipantId": "05491616-385f-44a8-9974-18cc5f9933c1",
  "id": "2f1a1100-b174-40a0-aba7-0b405e01ed92",
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#app/calls/$entity",
  "terminationReason": null,
  "ringingTimeoutInSeconds": null,
  "mediaState": null,
  "subject": null,
  "resultInfo": null,
  "answeredBy": null,
  "meetingCapability": null,
  "toneInfo": null
}
```

##### <a name="notification---establishing"></a><span data-ttu-id="78008-161">通知-建立</span><span class="sxs-lookup"><span data-stu-id="78008-161">Notification - establishing</span></span>

```http
POST https://bot.contoso.com/callback
Authorization: Bearer <TOKEN>
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
      "resource": "/app/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92",
        "callbackUri": "https://bot.contoso.com/callback",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "establishing",
        "chatInfo": {
          "@odata.type": "#microsoft.graph.chatInfo",
          "threadId": "19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2",
          "messageId": "0"
        },
        "meetingInfo": {
          "@odata.type": "#microsoft.graph.organizerMeetingInfo",
          "organizer": {
            "@odata.type": "#microsoft.graph.identitySet",
            "user": {
              "@odata.type": "#microsoft.graph.identity",
              "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
              "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
              "displayName": "Bob"
            }
          },
          "allowConversationWithoutHost": true
        },
        "id": "2f1a1100-b174-40a0-aba7-0b405e01ed92"
      }
    }
  ]
}

```
##### <a name="notification---established"></a><span data-ttu-id="78008-162">已建立通知</span><span class="sxs-lookup"><span data-stu-id="78008-162">Notification - established</span></span>

```http
POST https://bot.contoso.com/callback
Authorization: Bearer <TOKEN>
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
      "resource": "/app/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92",
      "callbackUri": "https://bot.contoso.com/callback",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "established",
        "chatInfo": {
          "@odata.type": "#microsoft.graph.chatInfo",
          "threadId": "19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2",
          "messageId": "0"
        },
        "meetingInfo": {
          "@odata.type": "#microsoft.graph.organizerMeetingInfo",
          "organizer": {
            "@odata.type": "#microsoft.graph.identitySet",
            "user": {
              "@odata.type": "#microsoft.graph.identity",
              "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
              "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
              "displayName": "Bob"
            }
          },
          "allowConversationWithoutHost": true
        },
        "id": "2f1a1100-b174-40a0-aba7-0b405e01ed92"
      }
    }
  ]
}
```
##### <a name="notification---roster"></a><span data-ttu-id="78008-163">通知-名单</span><span class="sxs-lookup"><span data-stu-id="78008-163">Notification - Roster</span></span>

```http
POST https://bot.contoso.com/callback
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications",
  "truncated": true
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resource": "/app/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92/participants",
      "callbackUri": "https://bot.contoso.com/callback",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "info": {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "user": {
                "@odata.type": "#microsoft.graph.identity",
                "displayName": "John",
                "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
              }
            },
            "languageId": "en-US"
          },
          "mediaStreams": [
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "audio",
              "sourceId": "1",
              "direction": "sendReceive",
              "serverMuted": false
            },
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "video",
              "sourceId": "2",
              "direction": "receiveOnly",
              "serverMuted": false
            },
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "videoBasedScreenSharing",
              "sourceId": "8",
              "direction": "receiveOnly",
              "serverMuted": false
            }
          ],
          "isMuted": true,
          "isInLobby": false,
          "id": "0d7664b6-6432-43ed-8d27-d9e7adec188c"
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "info": {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "application": {
                "@odata.type": "#microsoft.graph.identity",
                "displayName": "Calling Bot",
                "id": "2891555a-92ff-42e6-80fa-6e1300c6b5c6"
              }
            }
          },
          "mediaStreams": [
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "audio",
              "sourceId": "10",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isMuted": false,
          "isInLobby": false,
          "id": "05491616-385f-44a8-9974-18cc5f9933c1"
        }
      ]
    }
  ]
}
```

><span data-ttu-id="78008-164">**注意：** 除了呼叫状态通知之外，对于加入会议方案，我们会收到名单通知。</span><span class="sxs-lookup"><span data-stu-id="78008-164">**Note:** For join meeting scenarios apart from call state notifications, we receive roster notifications.</span></span>

### <a name="join-scheduled-meeting-with-app-hosted-media"></a><span data-ttu-id="78008-165">加入包含应用托管媒体的计划会议</span><span class="sxs-lookup"><span data-stu-id="78008-165">Join scheduled meeting with app hosted media</span></span>
<span data-ttu-id="78008-166">若要使用应用程序托管媒体加入会议，请按照上面提供的示例中所示的[AppHostedMediaConfig](../resources/apphostedmediaconfig.md)更新媒体配置。</span><span class="sxs-lookup"><span data-stu-id="78008-166">To join the meeting with application hosted media update the media config with the [AppHostedMediaConfig](../resources/apphostedmediaconfig.md) as shown below, In the sample provided above.</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
Authorization: Bearer <Token>
```
<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "@odata.type": "#microsoft.graph.call",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<Media Session Configuration>",
  },
  "chatInfo": {
    "@odata.type": "#microsoft.graph.chatInfo",
    "threadId": "19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2",
    "messageId": "0"
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "@odata.type": "#microsoft.graph.identitySet",
      "user": {
        "@odata.type": "#microsoft.graph.identity",
        "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
        "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
        "displayName": "Bob"
      }
    },
    "allowConversationWithoutHost": true
  },
  "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a"
}
```


### <a name="join-channel-meeting-with-service-hosted-media"></a><span data-ttu-id="78008-167">加入使用服务托管媒体的渠道会议</span><span class="sxs-lookup"><span data-stu-id="78008-167">Join channel meeting with service hosted media</span></span>
<span data-ttu-id="78008-168">频道内的会议需要特定的详细信息，例如，可以使用[获取联机会议 API](../api/onlinemeeting-get.md)获取的线程 id、messageid 和组织者详细信息。</span><span class="sxs-lookup"><span data-stu-id="78008-168">Meeting inside a channel requires specific details like thread id, messageid, and organizer details that can be obtained using the [Get Online Meetings API](../api/onlinemeeting-get.md).</span></span>

<span data-ttu-id="78008-169">授权令牌、回调 url、应用程序 id、应用程序名称、用户 id、用户名和租户 id 的值必须替换为通过获取具有实际值的[联机会议 API](../api/onlinemeeting-get.md)获取的详细信息，以使示例正常工作。</span><span class="sxs-lookup"><span data-stu-id="78008-169">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced along with the details obtained from  [Get Online Meetings API](../api/onlinemeeting-get.md) with actual values to make the example work.</span></span>

> <span data-ttu-id="78008-170">**注意：** 此示例需要该`Calls.JoinGroupCalls.All`权限。</span><span class="sxs-lookup"><span data-stu-id="78008-170">**Note:** This example needs the `Calls.JoinGroupCalls.All` permission.</span></span>

##### <a name="request"></a><span data-ttu-id="78008-171">请求</span><span class="sxs-lookup"><span data-stu-id="78008-171">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
Authorization: Bearer <Token>
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "@odata.type": "#microsoft.graph.call",
  "callbackUri": "https://bot.contoso.com/callback",
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
     {
       "uri": "https://cdn.contoso.com/beep.wav",
       "resourceId": "f8971b04-b53e-418c-9222-c82ce681a582"
     },
     {
       "uri": "https://cdn.contoso.com/cool.wav",
       "resourceId": "86dc814b-c172-4428-9112-60f8ecae1edb"
     }
    ],
  },
  "chatInfo": {
    "@odata.type": "#microsoft.graph.chatInfo",
    "threadId": "19:cbee7c1c860e465f8258e3cebf7bee0d@thread.skype",
    "messageId": "1533758867081"
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "@odata.type": "#microsoft.graph.identitySet",
      "user": {
        "@odata.type": "#microsoft.graph.identity",
        "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
        "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
        "displayName": "Bob"
      }
    },
    "allowConversationWithoutHost": true
  }
}
```

### <a name="join-channel-meeting-as-a-guest-with-service-hosted-media"></a><span data-ttu-id="78008-172">以具有服务托管媒体的来宾身份加入频道会议</span><span class="sxs-lookup"><span data-stu-id="78008-172">Join channel meeting as a guest with service hosted media</span></span>
<span data-ttu-id="78008-173">若要将渠道会议作为来宾加入，您需要创建一个来宾[标识](../resources/identityset.md)，并将其添加为加入会议请求中的呼叫源。</span><span class="sxs-lookup"><span data-stu-id="78008-173">For joining a channel meeting as a guest you will need to create a guest [identity](../resources/identityset.md) and add it as the call source in the join meeting request.</span></span>
<span data-ttu-id="78008-174">显示名称是您希望在会议中为您的来宾标识显示的名称。</span><span class="sxs-lookup"><span data-stu-id="78008-174">The display name is the name you want to be displayed in the meeting for your guest identity.</span></span> <span data-ttu-id="78008-175">Id 可以是标识来宾标识的唯一 id。</span><span class="sxs-lookup"><span data-stu-id="78008-175">The id may be a unique id identifying the guest identity.</span></span>

> <span data-ttu-id="78008-176">**注意：** 此示例需要该`Calls.JoinGroupCallsAsGuest.All`权限。</span><span class="sxs-lookup"><span data-stu-id="78008-176">**Note:** This example needs the `Calls.JoinGroupCallsAsGuest.All` permission.</span></span>

##### <a name="request"></a><span data-ttu-id="78008-177">请求</span><span class="sxs-lookup"><span data-stu-id="78008-177">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
Authorization: Bearer <Token>
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "@odata.type": "#microsoft.graph.call",
  "callbackUri": "https://bot.contoso.com/callback",
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "guest": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Guest User",
        "id": "d7a3b999-17ac-4bca-9e77-e6a730d2ec2e"
      }
    }
  },
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
     {
       "uri": "https://cdn.contoso.com/beep.wav",
       "resourceId": "f8971b04-b53e-418c-9222-c82ce681a582"
     },
     {
       "uri": "https://cdn.contoso.com/cool.wav",
       "resourceId": "86dc814b-c172-4428-9112-60f8ecae1edb"
     }
    ],
  },
  "chatInfo": {
    "@odata.type": "#microsoft.graph.chatInfo",
    "threadId": "19:cbee7c1c860e465f8258e3cebf7bee0d@thread.skype",
    "messageId": "1533758867081"
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "@odata.type": "#microsoft.graph.identitySet",
      "user": {
        "@odata.type": "#microsoft.graph.identity",
        "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
        "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
        "displayName": "Bob"
      }
    },
    "allowConversationWithoutHost": true
  }
}
```
> <span data-ttu-id="78008-178">**注意：** 来宾加入取决于会议的租户设置。</span><span class="sxs-lookup"><span data-stu-id="78008-178">**Note:** The guest join depends on the tenant settings for meeting.</span></span> <span data-ttu-id="78008-179">应用程序可能放置在等待用户承认的大厅中。</span><span class="sxs-lookup"><span data-stu-id="78008-179">The application might be put in lobby waiting to be admitted by a user.</span></span> <span data-ttu-id="78008-180">此`isInLobby`属性由属性定义</span><span class="sxs-lookup"><span data-stu-id="78008-180">This is defined by the `isInLobby` property</span></span>

##### <a name="notification---roster"></a><span data-ttu-id="78008-181">通知-名单</span><span class="sxs-lookup"><span data-stu-id="78008-181">Notification - Roster</span></span>

```http
POST https://bot.contoso.com/callback
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications",
  "truncated": true
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resource": "/app/calls/2f1a1100-726f-4705-a071-30fb8f6b568f/participants",
      "callbackUri": "https://bot.contoso.com/callback",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "info": {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "guest": {
                "@odata.type": "#microsoft.graph.identity",
                "displayName": "Guest User",
                "id": "d7a3b999-17ac-4bca-9e77-e6a730d2ec2e"
              }
            }
          },
          "mediaStreams": [
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "audio",
              "sourceId": "10",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isMuted": false,
          "isInLobby": true,
          "id": "05491616-385f-44a8-9974-18cc5f9933c1"
        }
      ]
    }
  ]
}
```
> <span data-ttu-id="78008-182">**注意：** 应用程序将不会在会议厅中收到参与者的名单，除非其获准来自会议厅</span><span class="sxs-lookup"><span data-stu-id="78008-182">**Note:** The application will not receive the roster for participants in the meeting until its admitted from lobby</span></span>
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create call",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
