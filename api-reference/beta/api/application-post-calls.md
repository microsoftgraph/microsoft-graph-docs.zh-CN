---
title: 创建调用
description: 创建新呼叫。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 056ec5a26c8eb38809acbbe56f5097137d265fbb
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289307"
---
# <a name="create-call"></a><span data-ttu-id="1fd52-103">创建调用</span><span class="sxs-lookup"><span data-stu-id="1fd52-103">Create call</span></span>

<span data-ttu-id="1fd52-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fd52-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1fd52-105">创建[呼叫](../resources/call.md)使你的 bot 能够创建新的传出对等或组呼叫，或加入现有会议。</span><span class="sxs-lookup"><span data-stu-id="1fd52-105">Create [call](../resources/call.md) enables your bot to create a new outgoing peer-to-peer or group call, or join an existing meeting.</span></span> <span data-ttu-id="1fd52-106">你需要[注册呼叫机器人](https://docs.microsoft.com/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot)并查看所需的权限列表，如下所述。</span><span class="sxs-lookup"><span data-stu-id="1fd52-106">You will need to [register the calling bot](https://docs.microsoft.com/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot) and go through the list of permissions needed as mentioned below.</span></span>

> <span data-ttu-id="1fd52-107">**注意：** 目前，仅支持 VoIP 呼叫。</span><span class="sxs-lookup"><span data-stu-id="1fd52-107">**Note:** Currently, only VoIP calls are supported.</span></span> 

## <a name="permissions"></a><span data-ttu-id="1fd52-108">权限</span><span class="sxs-lookup"><span data-stu-id="1fd52-108">Permissions</span></span>

<span data-ttu-id="1fd52-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](https://docs.microsoft.com/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot#add-microsoft-graph-permissions)。</span><span class="sxs-lookup"><span data-stu-id="1fd52-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://docs.microsoft.com/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot#add-microsoft-graph-permissions).</span></span>

| <span data-ttu-id="1fd52-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1fd52-111">Permission type</span></span>                        | <span data-ttu-id="1fd52-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1fd52-112">Permissions (from least to most privileged)</span></span>                                             |
|:---------------------------------------|:----------------------------------------------------------------------------------------|
| <span data-ttu-id="1fd52-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1fd52-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="1fd52-114">不支持</span><span class="sxs-lookup"><span data-stu-id="1fd52-114">Not Supported</span></span>                                                                           |
| <span data-ttu-id="1fd52-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1fd52-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1fd52-116">不支持</span><span class="sxs-lookup"><span data-stu-id="1fd52-116">Not Supported</span></span>                                                                           |
| <span data-ttu-id="1fd52-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1fd52-117">Application</span></span>                            | <span data-ttu-id="1fd52-118">JoinGroupCallsasGuest、JoinGroupCalls、calls、InitiateGroupCalls、All、和。</span><span class="sxs-lookup"><span data-stu-id="1fd52-118">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All</span></span> |

> <span data-ttu-id="1fd52-119">**注意：** 对于包含应用托管媒体的呼叫，除了列出的权限之一之外，还需要 AccessMedia 权限。</span><span class="sxs-lookup"><span data-stu-id="1fd52-119">**Note:** For a call with app-hosted media, you need the Calls.AccessMedia.All permission in addition to one of the permissions listed.</span></span>

## <a name="http-request"></a><span data-ttu-id="1fd52-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1fd52-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls
POST /communications/calls
```
> <span data-ttu-id="1fd52-121">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="1fd52-121">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="1fd52-122">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="1fd52-122">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1fd52-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="1fd52-123">Request headers</span></span>
| <span data-ttu-id="1fd52-124">名称</span><span class="sxs-lookup"><span data-stu-id="1fd52-124">Name</span></span>          | <span data-ttu-id="1fd52-125">说明</span><span class="sxs-lookup"><span data-stu-id="1fd52-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="1fd52-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="1fd52-126">Authorization</span></span> | <span data-ttu-id="1fd52-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1fd52-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1fd52-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="1fd52-129">Content-type</span></span>  | <span data-ttu-id="1fd52-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="1fd52-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fd52-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="1fd52-132">Request body</span></span>
<span data-ttu-id="1fd52-133">在请求正文中，提供[call](../resources/call.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1fd52-133">In the request body, supply a JSON representation of a [call](../resources/call.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1fd52-134">响应</span><span class="sxs-lookup"><span data-stu-id="1fd52-134">Response</span></span>
<span data-ttu-id="1fd52-135">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[call](../resources/call.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1fd52-135">If successful, this method returns a `201 Created` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1fd52-136">示例</span><span class="sxs-lookup"><span data-stu-id="1fd52-136">Examples</span></span>

### <a name="example-1-create-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="1fd52-137">示例1：使用服务托管媒体创建对等 VoIP 呼叫</span><span class="sxs-lookup"><span data-stu-id="1fd52-137">Example 1: Create peer-to-peer VoIP call with service hosted media</span></span>

> <span data-ttu-id="1fd52-138">**注意：** 此调用需要调用. Initiate。 All 权限。</span><span class="sxs-lookup"><span data-stu-id="1fd52-138">**Note:** This call needs the Calls.Initiate.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="1fd52-139">请求</span><span class="sxs-lookup"><span data-stu-id="1fd52-139">Request</span></span>
<span data-ttu-id="1fd52-140">以下示例显示了在 bot 和指定用户之间进行对等呼叫的请求。</span><span class="sxs-lookup"><span data-stu-id="1fd52-140">The following example shows the request which makes a peer-to-peer call between the bot and the specified user.</span></span> <span data-ttu-id="1fd52-141">在此示例中，媒体由服务托管。</span><span class="sxs-lookup"><span data-stu-id="1fd52-141">In this example, the media is hosted by the service.</span></span> <span data-ttu-id="1fd52-142">必须使用实际值替换授权令牌、回调 URL、应用程序 ID、应用程序名称、用户 ID、用户名和租户 ID 的值，以使示例正常工作。</span><span class="sxs-lookup"><span data-stu-id="1fd52-142">The values of authorization token, callback URL, application ID, application name, user ID, user name, and tenant ID must be replaced with actual values to make the example work.</span></span>


# <a name="http"></a>[<span data-ttu-id="1fd52-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="1fd52-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-call-service-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "callbackUri": "https://bot.contoso.com/callback",
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
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
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig"
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="1fd52-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1fd52-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-call-service-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="1fd52-145">C#</span><span class="sxs-lookup"><span data-stu-id="1fd52-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-call-service-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1fd52-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1fd52-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-call-service-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1fd52-147">响应</span><span class="sxs-lookup"><span data-stu-id="1fd52-147">Response</span></span>

> <span data-ttu-id="1fd52-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1fd52-148">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "state": "establishing",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "callChainId": "d8217646-3110-40b1-bae6-e9ac6c3a9f74",
  "callRoutes": [],
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "application": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "2891555a-92ff-42e6-80fa-6e1300c6b5c6"
      }
    },
    "countryCode": null,
    "endpointType": null,
    "region": null,
    "languageId": null
  },
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "John",
          "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
        }
      },
      "endpointType": null,
      "region": null,
      "replacesCallId": null,
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

##### <a name="notification---establishing"></a><span data-ttu-id="1fd52-149">通知-建立</span><span class="sxs-lookup"><span data-stu-id="1fd52-149">Notification - establishing</span></span>

```http
POST https://bot.contoso.com/callback
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
      "resourceUrl": "/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab",
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
##### <a name="notification---established"></a><span data-ttu-id="1fd52-150">已建立通知</span><span class="sxs-lookup"><span data-stu-id="1fd52-150">Notification - established</span></span>

```http
POST https://bot.contoso.com/callback
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
      "resourceUrl": "/communications/calls/2e1a0b00-b3c5-4b0f-99b3-c133bc1e6116",
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

### <a name="example-2-create-peer-to-peer-voip-call-with-application-hosted-media"></a><span data-ttu-id="1fd52-151">示例2：使用应用程序托管媒体创建对等 VoIP 呼叫</span><span class="sxs-lookup"><span data-stu-id="1fd52-151">Example 2: Create peer-to-peer VoIP call with application hosted media</span></span>

> <span data-ttu-id="1fd52-152">**注意**：此示例需要调用 AccessMedia 所有权限。</span><span class="sxs-lookup"><span data-stu-id="1fd52-152">**Note**: This example needs Calls.Initiate.All and Calls.AccessMedia.All permissions.</span></span>

##### <a name="request"></a><span data-ttu-id="1fd52-153">请求</span><span class="sxs-lookup"><span data-stu-id="1fd52-153">Request</span></span>
<span data-ttu-id="1fd52-154">以下示例显示了在 bot 和指定用户之间进行对等呼叫的请求。</span><span class="sxs-lookup"><span data-stu-id="1fd52-154">The following example shows the request which makes a peer-to-peer call between the bot and the specified user.</span></span> <span data-ttu-id="1fd52-155">在此示例中，媒体由应用程序本地承载。</span><span class="sxs-lookup"><span data-stu-id="1fd52-155">In this example the media is hosted locally by the application.</span></span> <span data-ttu-id="1fd52-156">必须使用实际值替换授权令牌、回调 url、应用程序 id、应用程序名称、用户 id、用户名和租户 id 的值，以使示例正常工作。</span><span class="sxs-lookup"><span data-stu-id="1fd52-156">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced with actual values to make the example work.</span></span>


# <a name="http"></a>[<span data-ttu-id="1fd52-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="1fd52-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-call-app-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "callbackUri": "https://bot.contoso.com/callback",
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "application": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "2891555a-92ff-42e6-80fa-6e1300c6b5c6"
      }
    },
    "region": null,
    "languageId": null
  },
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
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
    "blob": "<Media Session Configuration>"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="1fd52-158">C#</span><span class="sxs-lookup"><span data-stu-id="1fd52-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-call-app-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1fd52-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1fd52-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-call-app-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1fd52-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1fd52-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-call-app-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="1fd52-161">`<Media Session Configuration>`是序列化的媒体会话配置，其中包含媒体堆栈的会话信息。</span><span class="sxs-lookup"><span data-stu-id="1fd52-161">`<Media Session Configuration>` is the serialized media session configuration which contains the session information of the media stack.</span></span> <span data-ttu-id="1fd52-162">应在此处传递有关音频、视频、VBSS ssession 信息的特定信息。</span><span class="sxs-lookup"><span data-stu-id="1fd52-162">Specific information about audio, video, VBSS ssession information should be passed here.</span></span>

<span data-ttu-id="1fd52-163">示例音频媒体会话 blob 如下所示</span><span class="sxs-lookup"><span data-stu-id="1fd52-163">Sample audio media session blob is shown below</span></span>
```json
{\"mpUri\":\"net.tcp://bot.contoso.com:18732/MediaProcessor\",\"audioRenderContexts\":[\"14778cc4-f54c-43c7-989f-9092e34ef784\"],\"videoRenderContexts\":[],\"audioSourceContexts\":[\"a5dcfc9b-5a54-48ef-86f5-1fdd8508741a\"],\"videoSourceContexts\":[],\"dataRenderContexts\":null,\"dataSourceContexts\":null,\"supportedAudioFormat\":\"Pcm16K\",\"videoSinkEncodingFormats\":[],\"mpMediaSessionId\":\"2379cf46-acf3-4fef-a914-be9627075320\",\"regionAffinity\":null,\"skypeMediaBotsVersion\":\"1.11.1.0086\",\"mediaStackVersion\":\"2018.53.1.1\",\"mpVersion\":\"7.2.0.3881\",\"callId\":\"1b69b141-7f1a-4033-9c34-202737190a20\"}
```

><span data-ttu-id="1fd52-164">**注意：** 对于点对点呼叫，预期的通知仅适用于呼叫状态更改。</span><span class="sxs-lookup"><span data-stu-id="1fd52-164">**Note:** For peer-to-peer calls, the expected notifications are for call state changes only.</span></span>

##### <a name="response"></a><span data-ttu-id="1fd52-165">响应</span><span class="sxs-lookup"><span data-stu-id="1fd52-165">Response</span></span>

> <span data-ttu-id="1fd52-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1fd52-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "state": "establishing",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "callChainId": "d8217646-3110-40b1-bae6-e9ac6c3a9f74",
  "callRoutes": [],
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "application": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "2891555a-92ff-42e6-80fa-6e1300c6b5c6"
      }
    },
    "region": null,
    "languageId": null
  },
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
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
  "activeModalities": [],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<Media Session Configuration>",
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

### <a name="example-3-create-a-group-call-with-service-hosted-media"></a><span data-ttu-id="1fd52-168">示例3：使用服务托管媒体创建组呼叫</span><span class="sxs-lookup"><span data-stu-id="1fd52-168">Example 3: Create a group call with service hosted media</span></span>

<span data-ttu-id="1fd52-169">这最高支持5个 VoIP 用户。</span><span class="sxs-lookup"><span data-stu-id="1fd52-169">This supports up to 5 VoIP users.</span></span> <span data-ttu-id="1fd52-170">此示例演示如何使用两个 VoIP 用户创建组呼叫。</span><span class="sxs-lookup"><span data-stu-id="1fd52-170">The example shows how to create a group call with two VoIP users.</span></span>
> <span data-ttu-id="1fd52-171">**注意：** 此示例调用需要该 `Calls.InitiateGroupCalls.All` 权限。</span><span class="sxs-lookup"><span data-stu-id="1fd52-171">**Note:** This example call needs the `Calls.InitiateGroupCalls.All` permission.</span></span> <span data-ttu-id="1fd52-172">创建的组呼叫不支持聊天或录制。</span><span class="sxs-lookup"><span data-stu-id="1fd52-172">The group call created doesn't support chat or recording.</span></span>

##### <a name="request"></a><span data-ttu-id="1fd52-173">请求</span><span class="sxs-lookup"><span data-stu-id="1fd52-173">Request</span></span>
```http
POST https://graph.microsoft.com/beta/communications/calls
Content-Type: application/json
```
<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "@odata.type": "#microsoft.graph.call",
  "direction": "outgoing",
  "subject": "Create a group call with service hosted media",
  "callbackUri": "https://bot.contoso.com/callback",
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "application": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "TestBot",
        "id": "dd3885da-f9ab-486b-bfae-85de3d445555"
      }
    }
  },
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "user1",
          "id": "98da8a1a-1b87-452c-a713-65d3f10b5555"
        }
      }
    },
    {
      "@odata.type": "#microsoft.graph.participantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "user2",
          "id": "bf5aae9a-d11d-47a8-93b1-782504c95555"
        }
      }
    }
  ],
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "removeFromDefaultAudioGroup": false
  },
  "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a"
}
```

### <a name="example-4-create-a-group-call-with-application-hosted-media"></a><span data-ttu-id="1fd52-174">示例4：使用应用程序托管媒体创建组调用</span><span class="sxs-lookup"><span data-stu-id="1fd52-174">Example 4: Create a group call with application hosted media</span></span>

<span data-ttu-id="1fd52-175">这最高支持5个 VoIP 用户。</span><span class="sxs-lookup"><span data-stu-id="1fd52-175">This supports up to 5 VoIP users.</span></span> <span data-ttu-id="1fd52-176">此示例演示如何使用两个 VoIP 用户创建组呼叫。</span><span class="sxs-lookup"><span data-stu-id="1fd52-176">The example shows how to create a group call with two VoIP users.</span></span>
> <span data-ttu-id="1fd52-177">**注意：** 此示例调用需要该 `Calls.InitiateGroupCalls.All` 权限。</span><span class="sxs-lookup"><span data-stu-id="1fd52-177">**Note:** This example call needs the `Calls.InitiateGroupCalls.All` permission.</span></span> <span data-ttu-id="1fd52-178">创建的组呼叫不支持聊天或录制。</span><span class="sxs-lookup"><span data-stu-id="1fd52-178">The group call created doesn't support chat or recording.</span></span>

##### <a name="request"></a><span data-ttu-id="1fd52-179">请求</span><span class="sxs-lookup"><span data-stu-id="1fd52-179">Request</span></span>
```http
POST https://graph.microsoft.com/beta/communications/calls
Content-Type: application/json
```
<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "@odata.type": "#microsoft.graph.call",
  "direction": "outgoing",
  "subject": "Create a group call with service hosted media",
  "callbackUri": "https://bot.contoso.com/callback",
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "application": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "TestBot",
        "id": "dd3885da-f9ab-486b-bfae-85de3d445555"
      }
    }
  },
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "user1",
          "id": "98da8a1a-1b87-452c-a713-65d3f10b5555"
        }
      }
    },
    {
      "@odata.type": "#microsoft.graph.participantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "user2",
          "id": "bf5aae9a-d11d-47a8-93b1-782504c95555"
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
    "removeFromDefaultAudioGroup": false
  },
  "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a"
}
```

### <a name="example-5-join-scheduled-meeting-with-service-hosted-media"></a><span data-ttu-id="1fd52-180">示例5：加入服务托管媒体的计划会议</span><span class="sxs-lookup"><span data-stu-id="1fd52-180">Example 5: Join scheduled meeting with service hosted media</span></span>
<span data-ttu-id="1fd52-181">若要加入计划的会议，我们需要获取线程 id、邮件 id、组织者 id 以及在其中安排会议的租户 id。</span><span class="sxs-lookup"><span data-stu-id="1fd52-181">To join the scheduled meeting we will need to get the thread id, message id, organizer id and the tenant id in which the meeting is scheduled.</span></span>
<span data-ttu-id="1fd52-182">可以从[获取联机会议 API](../api/onlinemeeting-get.md)获取此信息。</span><span class="sxs-lookup"><span data-stu-id="1fd52-182">This information can be obtained from [Get Online Meetings API](../api/onlinemeeting-get.md).</span></span>

<span data-ttu-id="1fd52-183">授权令牌、回调 url、应用程序 id、应用程序名称、用户 id、用户名和租户 id 的值必须替换为通过获取具有实际值的[联机会议 API](../api/onlinemeeting-get.md)获取的详细信息，以使示例正常工作。</span><span class="sxs-lookup"><span data-stu-id="1fd52-183">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced along with the details obtained from  [Get Online Meetings API](../api/onlinemeeting-get.md) with actual values to make the example work.</span></span>
> <span data-ttu-id="1fd52-184">**注意：** 此示例需要该 `Calls.JoinGroupCalls.All` 权限。</span><span class="sxs-lookup"><span data-stu-id="1fd52-184">**Note:** This example needs the `Calls.JoinGroupCalls.All` permission.</span></span>

##### <a name="request"></a><span data-ttu-id="1fd52-185">请求</span><span class="sxs-lookup"><span data-stu-id="1fd52-185">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "join-meeting-service-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls
Content-Type: application/json

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
##### <a name="response"></a><span data-ttu-id="1fd52-186">响应</span><span class="sxs-lookup"><span data-stu-id="1fd52-186">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": "true",
  "@odata.type": "microsoft.graph.call"
}-->
```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/communications/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "state": "establishing",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "callChainId": "d8217646-3110-40b1-bae6-e9ac6c3a9f74",
  "callRoutes": [],
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "application": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "2891555a-92ff-42e6-80fa-6e1300c6b5c6"
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

##### <a name="notification---establishing"></a><span data-ttu-id="1fd52-187">通知-建立</span><span class="sxs-lookup"><span data-stu-id="1fd52-187">Notification - establishing</span></span>

```http
POST https://bot.contoso.com/callback
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
      "resourceUrl": "/communications/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92",
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
##### <a name="notification---established"></a><span data-ttu-id="1fd52-188">已建立通知</span><span class="sxs-lookup"><span data-stu-id="1fd52-188">Notification - established</span></span>

```http
POST https://bot.contoso.com/callback
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
      "resourceUrl": "/communications/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92",
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
##### <a name="notification---roster"></a><span data-ttu-id="1fd52-189">通知-名单</span><span class="sxs-lookup"><span data-stu-id="1fd52-189">Notification - roster</span></span>

```http
POST https://bot.contoso.com/callback
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
      "resourceUrl": "/communications/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92/participants",
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

><span data-ttu-id="1fd52-190">**注意：** 除了呼叫状态通知之外，对于加入会议方案，我们会收到名单通知。</span><span class="sxs-lookup"><span data-stu-id="1fd52-190">**Note:** For join meeting scenarios apart from call state notifications, we receive roster notifications.</span></span>

### <a name="example-6-join-scheduled-meeting-with-app-hosted-media"></a><span data-ttu-id="1fd52-191">示例6：加入带应用程序托管媒体的计划会议</span><span class="sxs-lookup"><span data-stu-id="1fd52-191">Example 6: Join scheduled meeting with app hosted media</span></span>
<span data-ttu-id="1fd52-192">若要使用应用程序托管媒体加入会议，请按照上面提供的示例中所示的[AppHostedMediaConfig](../resources/apphostedmediaconfig.md)更新媒体配置。</span><span class="sxs-lookup"><span data-stu-id="1fd52-192">To join the meeting with application hosted media update the media config with the [AppHostedMediaConfig](../resources/apphostedmediaconfig.md) as shown below, In the sample provided above.</span></span>

<!-- {
  "blockType": "example",
  "name": "join-meeting-app-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls
Content-Type: application/json

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


### <a name="example-7-join-channel-meeting-with-service-hosted-media"></a><span data-ttu-id="1fd52-193">示例7：加入使用服务托管媒体的渠道会议</span><span class="sxs-lookup"><span data-stu-id="1fd52-193">Example 7: Join channel meeting with service hosted media</span></span>
<span data-ttu-id="1fd52-194">频道内的会议需要特定的详细信息，例如，可以使用[获取联机会议 API](../api/onlinemeeting-get.md)获取的线程 id、messageid 和组织者详细信息。</span><span class="sxs-lookup"><span data-stu-id="1fd52-194">Meeting inside a channel requires specific details like thread id, messageid, and organizer details that can be obtained using the [Get Online Meetings API](../api/onlinemeeting-get.md).</span></span>

<span data-ttu-id="1fd52-195">授权令牌、回调 url、应用程序 id、应用程序名称、用户 id、用户名和租户 id 的值必须替换为通过获取具有实际值的[联机会议 API](../api/onlinemeeting-get.md)获取的详细信息，以使示例正常工作。</span><span class="sxs-lookup"><span data-stu-id="1fd52-195">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced along with the details obtained from  [Get Online Meetings API](../api/onlinemeeting-get.md) with actual values to make the example work.</span></span>

> <span data-ttu-id="1fd52-196">**注意：** 此示例需要该 `Calls.JoinGroupCalls.All` 权限。</span><span class="sxs-lookup"><span data-stu-id="1fd52-196">**Note:** This example needs the `Calls.JoinGroupCalls.All` permission.</span></span>

##### <a name="request"></a><span data-ttu-id="1fd52-197">请求</span><span class="sxs-lookup"><span data-stu-id="1fd52-197">Request</span></span>

<!-- {
  "blockType": "example",
  "name": "join-channel-meeting-service-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls
Content-Type: application/json

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

### <a name="example-8-join-channel-meeting-as-a-guest-with-service-hosted-media"></a><span data-ttu-id="1fd52-198">示例8：以具有服务托管媒体的来宾身份加入通道会议</span><span class="sxs-lookup"><span data-stu-id="1fd52-198">Example 8: Join channel meeting as a guest with service hosted media</span></span>
<span data-ttu-id="1fd52-199">若要将渠道会议作为来宾加入，您需要创建一个来宾[标识](../resources/identityset.md)，并将其添加为加入会议请求中的呼叫源。</span><span class="sxs-lookup"><span data-stu-id="1fd52-199">For joining a channel meeting as a guest you will need to create a guest [identity](../resources/identityset.md) and add it as the call source in the join meeting request.</span></span>
<span data-ttu-id="1fd52-200">显示名称是您希望在会议中为您的来宾标识显示的名称。</span><span class="sxs-lookup"><span data-stu-id="1fd52-200">The display name is the name you want to be displayed in the meeting for your guest identity.</span></span> <span data-ttu-id="1fd52-201">Id 可以是标识来宾标识的唯一 id。</span><span class="sxs-lookup"><span data-stu-id="1fd52-201">The id may be a unique id identifying the guest identity.</span></span>

> <span data-ttu-id="1fd52-202">**注意：** 此示例需要该 `Calls.JoinGroupCallsAsGuest.All` 权限。</span><span class="sxs-lookup"><span data-stu-id="1fd52-202">**Note:** This example needs the `Calls.JoinGroupCallsAsGuest.All` permission.</span></span>

##### <a name="request"></a><span data-ttu-id="1fd52-203">请求</span><span class="sxs-lookup"><span data-stu-id="1fd52-203">Request</span></span>

<!-- {
  "blockType": "example",
  "name": "join-channel-meeting-as-guest-service-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls
Content-Type: application/json

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
> <span data-ttu-id="1fd52-204">**注意：** 来宾加入取决于会议的租户设置。</span><span class="sxs-lookup"><span data-stu-id="1fd52-204">**Note:** The guest join depends on the tenant settings for meeting.</span></span> <span data-ttu-id="1fd52-205">应用程序可能放置在等待用户承认的大厅中。</span><span class="sxs-lookup"><span data-stu-id="1fd52-205">The application might be put in lobby waiting to be admitted by a user.</span></span> <span data-ttu-id="1fd52-206">此属性由属性定义 `isInLobby`</span><span class="sxs-lookup"><span data-stu-id="1fd52-206">This is defined by the `isInLobby` property</span></span>

##### <a name="notification---roster"></a><span data-ttu-id="1fd52-207">通知-名单</span><span class="sxs-lookup"><span data-stu-id="1fd52-207">Notification - roster</span></span>

```http
POST https://bot.contoso.com/callback
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
      "resourceUrl": "/communications/calls/2f1a1100-726f-4705-a071-30fb8f6b568f/participants",
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
> <span data-ttu-id="1fd52-208">**注意：** 应用程序将不会在会议厅中收到参与者的名单，除非其获准来自会议厅</span><span class="sxs-lookup"><span data-stu-id="1fd52-208">**Note:** The application will not receive the roster for participants in the meeting until its admitted from lobby</span></span>

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
