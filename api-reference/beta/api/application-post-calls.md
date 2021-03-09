---
title: 创建调用
description: 创建新呼叫。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 888fb523ad54f840b5ecbc807b5ed46c8f798efb
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574900"
---
# <a name="create-call"></a><span data-ttu-id="b4d9c-103">创建调用</span><span class="sxs-lookup"><span data-stu-id="b4d9c-103">Create call</span></span>

<span data-ttu-id="b4d9c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4d9c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4d9c-105">通过 [创建](../resources/call.md) 呼叫，机器人可以创建新的传出对等呼叫或组呼叫，或加入现有会议。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-105">Create [call](../resources/call.md) enables your bot to create a new outgoing peer-to-peer or group call, or join an existing meeting.</span></span> <span data-ttu-id="b4d9c-106">你将需要注册 [调用机器人](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot) ，并浏览下面提到的所需权限列表。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-106">You will need to [register the calling bot](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot) and go through the list of permissions needed as mentioned below.</span></span>

> <span data-ttu-id="b4d9c-107">**注意：** 目前，仅支持 VoIP 呼叫。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-107">**Note:** Currently, only VoIP calls are supported.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b4d9c-108">权限</span><span class="sxs-lookup"><span data-stu-id="b4d9c-108">Permissions</span></span>

<span data-ttu-id="b4d9c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot#add-microsoft-graph-permissions)。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot#add-microsoft-graph-permissions).</span></span>

| <span data-ttu-id="b4d9c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4d9c-111">Permission type</span></span>                        | <span data-ttu-id="b4d9c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b4d9c-112">Permissions (from least to most privileged)</span></span>                                             |
|:---------------------------------------|:----------------------------------------------------------------------------------------|
| <span data-ttu-id="b4d9c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4d9c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b4d9c-114">不支持</span><span class="sxs-lookup"><span data-stu-id="b4d9c-114">Not Supported</span></span>                                                                           |
| <span data-ttu-id="b4d9c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4d9c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4d9c-116">不支持</span><span class="sxs-lookup"><span data-stu-id="b4d9c-116">Not Supported</span></span>                                                                           |
| <span data-ttu-id="b4d9c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b4d9c-117">Application</span></span>                            | <span data-ttu-id="b4d9c-118">Calls.JoinGroupCallsasGuest.All、Calls.JoinGroupCalls.All、Calls.Initiate。All、Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="b4d9c-118">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All</span></span> |

> <span data-ttu-id="b4d9c-119">**注意：** 对于具有应用托管媒体的呼叫，除了列出的其中一个权限之外，还需要 Calls.AccessMedia.All 权限。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-119">**Note:** For a call with app-hosted media, you need the Calls.AccessMedia.All permission in addition to one of the permissions listed.</span></span>

## <a name="http-request"></a><span data-ttu-id="b4d9c-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4d9c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls
POST /communications/calls
```
> <span data-ttu-id="b4d9c-121">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-121">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="b4d9c-122">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-122">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b4d9c-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="b4d9c-123">Request headers</span></span>
| <span data-ttu-id="b4d9c-124">名称</span><span class="sxs-lookup"><span data-stu-id="b4d9c-124">Name</span></span>          | <span data-ttu-id="b4d9c-125">说明</span><span class="sxs-lookup"><span data-stu-id="b4d9c-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b4d9c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4d9c-126">Authorization</span></span> | <span data-ttu-id="b4d9c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b4d9c-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="b4d9c-129">Content-type</span></span>  | <span data-ttu-id="b4d9c-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b4d9c-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4d9c-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4d9c-132">Request body</span></span>
<span data-ttu-id="b4d9c-133">在请求正文中，提供调用对象的 JSON [表示形式](../resources/call.md) 。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-133">In the request body, supply a JSON representation of a [call](../resources/call.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b4d9c-134">响应</span><span class="sxs-lookup"><span data-stu-id="b4d9c-134">Response</span></span>
<span data-ttu-id="b4d9c-135">如果成功，此方法在响应正文中返回响应代码 `201 Created` 和调用对象。 [](../resources/call.md)</span><span class="sxs-lookup"><span data-stu-id="b4d9c-135">If successful, this method returns a `201 Created` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b4d9c-136">示例</span><span class="sxs-lookup"><span data-stu-id="b4d9c-136">Examples</span></span>

### <a name="example-1-create-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="b4d9c-137">示例 1：使用服务托管媒体创建对等 VoIP 呼叫</span><span class="sxs-lookup"><span data-stu-id="b4d9c-137">Example 1: Create peer-to-peer VoIP call with service hosted media</span></span>

> <span data-ttu-id="b4d9c-138">**注意：** 此调用需要Calls.Ini平铺。所有权限。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-138">**Note:** This call needs the Calls.Initiate.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="b4d9c-139">请求</span><span class="sxs-lookup"><span data-stu-id="b4d9c-139">Request</span></span>
<span data-ttu-id="b4d9c-140">以下示例显示了在自动程序与指定用户之间进行对等呼叫的请求。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-140">The following example shows the request which makes a peer-to-peer call between the bot and the specified user.</span></span> <span data-ttu-id="b4d9c-141">本示例中，媒体由服务托管。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-141">In this example, the media is hosted by the service.</span></span> <span data-ttu-id="b4d9c-142">必须将授权令牌、回调 URL、应用程序 ID、应用程序名称、用户 ID、用户名和租户 ID 的值替换为实际值，使示例有效。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-142">The values of authorization token, callback URL, application ID, application name, user ID, user name, and tenant ID must be replaced with actual values to make the example work.</span></span>


# <a name="http"></a>[<span data-ttu-id="b4d9c-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4d9c-143">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="b4d9c-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4d9c-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-call-service-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="b4d9c-145">C#</span><span class="sxs-lookup"><span data-stu-id="b4d9c-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-call-service-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b4d9c-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4d9c-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-call-service-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b4d9c-147">Java</span><span class="sxs-lookup"><span data-stu-id="b4d9c-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-call-service-hosted-media-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b4d9c-148">响应</span><span class="sxs-lookup"><span data-stu-id="b4d9c-148">Response</span></span>

> <span data-ttu-id="b4d9c-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-149">**Note:** The response object shown here might be shortened for readability.</span></span> 

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
  "transcription": null,
  "meetingCapability": null,
  "toneInfo": null
}
```

##### <a name="notification---establishing"></a><span data-ttu-id="b4d9c-150">通知 - 建立</span><span class="sxs-lookup"><span data-stu-id="b4d9c-150">Notification - establishing</span></span>

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
##### <a name="notification---established"></a><span data-ttu-id="b4d9c-151">通知 - 已建立</span><span class="sxs-lookup"><span data-stu-id="b4d9c-151">Notification - established</span></span>

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

### <a name="example-2-create-peer-to-peer-voip-call-with-application-hosted-media"></a><span data-ttu-id="b4d9c-152">示例 2：使用应用程序托管媒体创建对等 VoIP 呼叫</span><span class="sxs-lookup"><span data-stu-id="b4d9c-152">Example 2: Create peer-to-peer VoIP call with application hosted media</span></span>

> <span data-ttu-id="b4d9c-153">**注意**：此示例需要Calls.Ini平铺。All 和 Calls.AccessMedia.All 权限。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-153">**Note**: This example needs Calls.Initiate.All and Calls.AccessMedia.All permissions.</span></span>

##### <a name="request"></a><span data-ttu-id="b4d9c-154">请求</span><span class="sxs-lookup"><span data-stu-id="b4d9c-154">Request</span></span>
<span data-ttu-id="b4d9c-155">以下示例显示了在自动程序与指定用户之间进行对等呼叫的请求。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-155">The following example shows the request which makes a peer-to-peer call between the bot and the specified user.</span></span> <span data-ttu-id="b4d9c-156">本示例中，媒体由应用程序在本地托管。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-156">In this example the media is hosted locally by the application.</span></span> <span data-ttu-id="b4d9c-157">必须将授权令牌、回调 URL、应用程序 ID、应用程序名称、用户 ID、用户名和租户 ID 的值替换为实际值，使示例有效。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-157">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced with actual values to make the example work.</span></span>


# <a name="http"></a>[<span data-ttu-id="b4d9c-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4d9c-158">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b4d9c-159">C#</span><span class="sxs-lookup"><span data-stu-id="b4d9c-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-call-app-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b4d9c-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4d9c-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-call-app-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b4d9c-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4d9c-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-call-app-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b4d9c-162">Java</span><span class="sxs-lookup"><span data-stu-id="b4d9c-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-call-app-hosted-media-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="b4d9c-163">`<Media Session Configuration>` 是包含媒体堆栈的会话信息的序列化媒体会话配置。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-163">`<Media Session Configuration>` is the serialized media session configuration which contains the session information of the media stack.</span></span> <span data-ttu-id="b4d9c-164">此处应传递有关音频、视频、VBSS ssession 信息的特定信息。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-164">Specific information about audio, video, VBSS ssession information should be passed here.</span></span>

<span data-ttu-id="b4d9c-165">示例音频媒体会话 blob 如下所示</span><span class="sxs-lookup"><span data-stu-id="b4d9c-165">Sample audio media session blob is shown below</span></span>
```json
{\"mpUri\":\"net.tcp://bot.contoso.com:18732/MediaProcessor\",\"audioRenderContexts\":[\"14778cc4-f54c-43c7-989f-9092e34ef784\"],\"videoRenderContexts\":[],\"audioSourceContexts\":[\"a5dcfc9b-5a54-48ef-86f5-1fdd8508741a\"],\"videoSourceContexts\":[],\"dataRenderContexts\":null,\"dataSourceContexts\":null,\"supportedAudioFormat\":\"Pcm16K\",\"videoSinkEncodingFormats\":[],\"mpMediaSessionId\":\"2379cf46-acf3-4fef-a914-be9627075320\",\"regionAffinity\":null,\"skypeMediaBotsVersion\":\"1.11.1.0086\",\"mediaStackVersion\":\"2018.53.1.1\",\"mpVersion\":\"7.2.0.3881\",\"callId\":\"1b69b141-7f1a-4033-9c34-202737190a20\"}
```

><span data-ttu-id="b4d9c-166">**注意：** 对于对等呼叫，预期通知仅适用于呼叫状态更改。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-166">**Note:** For peer-to-peer calls, the expected notifications are for call state changes only.</span></span>

##### <a name="response"></a><span data-ttu-id="b4d9c-167">响应</span><span class="sxs-lookup"><span data-stu-id="b4d9c-167">Response</span></span>

> <span data-ttu-id="b4d9c-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "transcription": null,
  "meetingCapability": null,
  "toneInfo": null
}
```

### <a name="example-3-create-a-group-call-with-service-hosted-media"></a><span data-ttu-id="b4d9c-170">示例 3：使用服务托管媒体创建组呼叫</span><span class="sxs-lookup"><span data-stu-id="b4d9c-170">Example 3: Create a group call with service hosted media</span></span>

<span data-ttu-id="b4d9c-171">这支持最多 5 个 VoIP 用户。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-171">This supports up to 5 VoIP users.</span></span> <span data-ttu-id="b4d9c-172">该示例演示如何创建具有两个 VoIP 用户的组呼叫。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-172">The example shows how to create a group call with two VoIP users.</span></span>
> <span data-ttu-id="b4d9c-173">**注意：** 此示例调用需要 `Calls.InitiateGroupCalls.All` 权限。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-173">**Note:** This example call needs the `Calls.InitiateGroupCalls.All` permission.</span></span> <span data-ttu-id="b4d9c-174">创建的组呼叫不支持聊天或录制。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-174">The group call created doesn't support chat or recording.</span></span>

##### <a name="request"></a><span data-ttu-id="b4d9c-175">请求</span><span class="sxs-lookup"><span data-stu-id="b4d9c-175">Request</span></span>
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

### <a name="example-4-create-a-group-call-with-application-hosted-media"></a><span data-ttu-id="b4d9c-176">示例 4：使用应用程序托管媒体创建组呼叫</span><span class="sxs-lookup"><span data-stu-id="b4d9c-176">Example 4: Create a group call with application hosted media</span></span>

<span data-ttu-id="b4d9c-177">这支持最多 5 个 VoIP 用户。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-177">This supports up to 5 VoIP users.</span></span> <span data-ttu-id="b4d9c-178">该示例演示如何创建具有两个 VoIP 用户的组呼叫。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-178">The example shows how to create a group call with two VoIP users.</span></span>
> <span data-ttu-id="b4d9c-179">**注意：** 此示例调用需要 `Calls.InitiateGroupCalls.All` 权限。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-179">**Note:** This example call needs the `Calls.InitiateGroupCalls.All` permission.</span></span> <span data-ttu-id="b4d9c-180">创建的组呼叫不支持聊天或录制。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-180">The group call created doesn't support chat or recording.</span></span>

##### <a name="request"></a><span data-ttu-id="b4d9c-181">请求</span><span class="sxs-lookup"><span data-stu-id="b4d9c-181">Request</span></span>
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

### <a name="example-5-join-scheduled-meeting-with-service-hosted-media"></a><span data-ttu-id="b4d9c-182">示例 5：使用服务托管媒体加入计划会议</span><span class="sxs-lookup"><span data-stu-id="b4d9c-182">Example 5: Join scheduled meeting with service hosted media</span></span>
<span data-ttu-id="b4d9c-183">若要加入计划的会议，我们需要获取计划会议的线程 ID、消息 ID、组织者 ID 和租户 ID。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-183">To join the scheduled meeting we will need to get the thread id, message id, organizer id and the tenant id in which the meeting is scheduled.</span></span>
<span data-ttu-id="b4d9c-184">此信息可以从 Get Online [Meetings API 获取](../api/onlinemeeting-get.md)。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-184">This information can be obtained from [Get Online Meetings API](../api/onlinemeeting-get.md).</span></span>

<span data-ttu-id="b4d9c-185">必须将授权令牌、回调 URL、应用程序 ID、应用程序名称、用户 ID、用户名和租户 ID 的值与从 Get Online  [Meetings API](../api/onlinemeeting-get.md) 获取的详细信息一起替换为实际值，使示例有效。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-185">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced along with the details obtained from  [Get Online Meetings API](../api/onlinemeeting-get.md) with actual values to make the example work.</span></span>
> <span data-ttu-id="b4d9c-186">**注意：** 此示例需要 `Calls.JoinGroupCalls.All` 权限。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-186">**Note:** This example needs the `Calls.JoinGroupCalls.All` permission.</span></span>

##### <a name="request"></a><span data-ttu-id="b4d9c-187">请求</span><span class="sxs-lookup"><span data-stu-id="b4d9c-187">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b4d9c-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4d9c-188">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
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
        "displayName": "Bob",
        "tenantId":"86dc81db-c112-4228-9222-63f3esaa1edb"
      }
    },
    "allowConversationWithoutHost": true
  },
  "tenantId":"86dc81db-c112-4228-9222-63f3esaa1edb"
}
```
# <a name="c"></a>[<span data-ttu-id="b4d9c-189">C#</span><span class="sxs-lookup"><span data-stu-id="b4d9c-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/join-meeting-service-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b4d9c-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4d9c-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/join-meeting-service-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b4d9c-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4d9c-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/join-meeting-service-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b4d9c-192">响应</span><span class="sxs-lookup"><span data-stu-id="b4d9c-192">Response</span></span>

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
  "transcription": null,
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

##### <a name="notification---establishing"></a><span data-ttu-id="b4d9c-193">通知 - 建立</span><span class="sxs-lookup"><span data-stu-id="b4d9c-193">Notification - establishing</span></span>

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
##### <a name="notification---established"></a><span data-ttu-id="b4d9c-194">通知 - 已建立</span><span class="sxs-lookup"><span data-stu-id="b4d9c-194">Notification - established</span></span>

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
##### <a name="notification---roster"></a><span data-ttu-id="b4d9c-195">通知 - 名单</span><span class="sxs-lookup"><span data-stu-id="b4d9c-195">Notification - roster</span></span>

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

><span data-ttu-id="b4d9c-196">**注意：** 对于除呼叫状态通知外加入会议方案，我们接收名单通知。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-196">**Note:** For join meeting scenarios apart from call state notifications, we receive roster notifications.</span></span>

### <a name="example-6-join-scheduled-meeting-with-app-hosted-media"></a><span data-ttu-id="b4d9c-197">示例 6：使用应用托管媒体加入计划会议</span><span class="sxs-lookup"><span data-stu-id="b4d9c-197">Example 6: Join scheduled meeting with app hosted media</span></span>
<span data-ttu-id="b4d9c-198">若要使用应用程序托管媒体加入会议，请通过 [AppHostedMediaConfig](../resources/apphostedmediaconfig.md) 更新媒体配置，如下所示，如上文提供的示例所示。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-198">To join the meeting with application hosted media update the media config with the [AppHostedMediaConfig](../resources/apphostedmediaconfig.md) as shown below, In the sample provided above.</span></span>

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


### <a name="example-7-join-channel-meeting-with-service-hosted-media"></a><span data-ttu-id="b4d9c-199">示例 7：使用服务托管媒体加入频道会议</span><span class="sxs-lookup"><span data-stu-id="b4d9c-199">Example 7: Join channel meeting with service hosted media</span></span>
<span data-ttu-id="b4d9c-200">频道内的会议需要特定的详细信息，如线程 ID、messageid 和组织者详细信息，可以使用[Get Online 会议 API 获取。](../api/onlinemeeting-get.md)</span><span class="sxs-lookup"><span data-stu-id="b4d9c-200">Meeting inside a channel requires specific details like thread id, messageid, and organizer details that can be obtained using the [Get Online Meetings API](../api/onlinemeeting-get.md).</span></span>

<span data-ttu-id="b4d9c-201">必须将授权令牌、回调 URL、应用程序 ID、应用程序名称、用户 ID、用户名和租户 ID 的值与从 Get Online  [Meetings API](../api/onlinemeeting-get.md) 获取的详细信息一起替换为实际值，使示例有效。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-201">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced along with the details obtained from  [Get Online Meetings API](../api/onlinemeeting-get.md) with actual values to make the example work.</span></span>

> <span data-ttu-id="b4d9c-202">**注意：** 此示例需要 `Calls.JoinGroupCalls.All` 权限。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-202">**Note:** This example needs the `Calls.JoinGroupCalls.All` permission.</span></span>

##### <a name="request"></a><span data-ttu-id="b4d9c-203">请求</span><span class="sxs-lookup"><span data-stu-id="b4d9c-203">Request</span></span>

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

### <a name="example-8-join-channel-meeting-as-a-guest-with-service-hosted-media"></a><span data-ttu-id="b4d9c-204">示例 8：使用服务托管媒体作为来宾加入频道会议</span><span class="sxs-lookup"><span data-stu-id="b4d9c-204">Example 8: Join channel meeting as a guest with service hosted media</span></span>
<span data-ttu-id="b4d9c-205">若要以来宾身份加入频道会议，你需要创建来宾标识，并将其添加到加入[](../resources/identityset.md)会议请求中的呼叫源。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-205">For joining a channel meeting as a guest you will need to create a guest [identity](../resources/identityset.md) and add it as the call source in the join meeting request.</span></span>
<span data-ttu-id="b4d9c-206">显示名称是您希望在会议中显示的来宾标识的名称。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-206">The display name is the name you want to be displayed in the meeting for your guest identity.</span></span> <span data-ttu-id="b4d9c-207">ID 可能是标识来宾标识的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-207">The id may be a unique id identifying the guest identity.</span></span>

> <span data-ttu-id="b4d9c-208">**注意：** 此示例需要 `Calls.JoinGroupCallsAsGuest.All` 权限。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-208">**Note:** This example needs the `Calls.JoinGroupCallsAsGuest.All` permission.</span></span>

##### <a name="request"></a><span data-ttu-id="b4d9c-209">请求</span><span class="sxs-lookup"><span data-stu-id="b4d9c-209">Request</span></span>

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
> <span data-ttu-id="b4d9c-210">**注意：** 来宾加入取决于会议租户设置。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-210">**Note:** The guest join depends on the tenant settings for meeting.</span></span> <span data-ttu-id="b4d9c-211">应用程序可能会置于大厅中，等待用户进入。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-211">The application might be put in lobby waiting to be admitted by a user.</span></span> <span data-ttu-id="b4d9c-212">此属性由 `isInLobby` 属性定义</span><span class="sxs-lookup"><span data-stu-id="b4d9c-212">This is defined by the `isInLobby` property</span></span>

##### <a name="notification---roster"></a><span data-ttu-id="b4d9c-213">通知 - 名单</span><span class="sxs-lookup"><span data-stu-id="b4d9c-213">Notification - roster</span></span>

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
> <span data-ttu-id="b4d9c-214">**注意：** 在从会议厅中获准加入会议之前，应用程序不会收到与会者名单</span><span class="sxs-lookup"><span data-stu-id="b4d9c-214">**Note:** The application will not receive the roster for participants in the meeting until its admitted from lobby</span></span>

### <a name="example-9-create-peer-to-peer-pstn-call-with-service-hosted-media"></a><span data-ttu-id="b4d9c-215">示例 9：使用服务托管媒体创建对等 PSTN 呼叫</span><span class="sxs-lookup"><span data-stu-id="b4d9c-215">Example 9: Create peer-to-peer PSTN call with service hosted media</span></span>

> <span data-ttu-id="b4d9c-216">**注意：** 此调用需要Calls.Ini平铺。所有权限。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-216">**Note:** This call requires the Calls.Initiate.All permission.</span></span>

<span data-ttu-id="b4d9c-217">此呼叫需要分配有 PSTN 号码的应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-217">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="b4d9c-218">有关详细信息，请参阅 [为自动程序分配电话号码](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot)。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-218">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>

#### <a name="request"></a><span data-ttu-id="b4d9c-219">请求</span><span class="sxs-lookup"><span data-stu-id="b4d9c-219">Request</span></span>
<span data-ttu-id="b4d9c-220">以下示例显示了在机器人和 PSTN 号码之间进行对等呼叫的请求。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-220">The following example shows the request to make a peer-to-peer call between the bot and a PSTN number.</span></span> <span data-ttu-id="b4d9c-221">本示例中，媒体由服务托管。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-221">In this example, the media is hosted by the service.</span></span> <span data-ttu-id="b4d9c-222">必须将授权令牌、回调 URL、应用程序 ID、应用程序名称、用户 ID、用户名和租户 ID 的值替换为实际值，使示例有效。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-222">The values of authorization token, callback URL, application ID, application name, user ID, user name, and tenant ID must be replaced with actual values to make the example work.</span></span>

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
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "applicationInstance": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "3d913abb-aec0-4964-8fa6-3c6850c4f278"
      },
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
        "phone": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "+12345678901"
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

#### <a name="response"></a><span data-ttu-id="b4d9c-223">响应</span><span class="sxs-lookup"><span data-stu-id="b4d9c-223">Response</span></span>

> <span data-ttu-id="b4d9c-224">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-224">**Note:** The response object shown here might be shortened for readability.</span></span> 

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
      "applicationInstance": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "3d913abb-aec0-4964-8fa6-3c6850c4f278"
      },
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
        "phone": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "+12345678901"
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
  "transcription": null,
  "meetingCapability": null,
  "toneInfo": null
}
```

### <a name="example-10-create-peer-to-peer-pstn-call-with-application-hosted-media"></a><span data-ttu-id="b4d9c-225">示例 10：使用应用程序托管媒体创建对等 PSTN 呼叫</span><span class="sxs-lookup"><span data-stu-id="b4d9c-225">Example 10: Create peer-to-peer PSTN call with application hosted media</span></span>

> <span data-ttu-id="b4d9c-226">**注意**：此示例要求Calls.Ini平铺。All 和 Calls.AccessMedia.All 权限。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-226">**Note**: This example requires Calls.Initiate.All and Calls.AccessMedia.All permissions.</span></span>

<span data-ttu-id="b4d9c-227">此呼叫需要分配有 PSTN 号码的应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-227">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="b4d9c-228">有关详细信息，请参阅 [为自动程序分配电话号码](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot)。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-228">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>

#### <a name="request"></a><span data-ttu-id="b4d9c-229">请求</span><span class="sxs-lookup"><span data-stu-id="b4d9c-229">Request</span></span>
<span data-ttu-id="b4d9c-230">以下示例显示一个请求，请求在自动程序与 PSTN 号码之间进行对等呼叫。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-230">The following example shows a request to make a peer-to-peer call between the bot and a PSTN number.</span></span> <span data-ttu-id="b4d9c-231">本示例中，媒体由应用程序在本地托管。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-231">In this example, the media is hosted locally by the application.</span></span> <span data-ttu-id="b4d9c-232">替换授权令牌、回调 URL、应用程序 ID、应用程序名称、用户 ID、用户名和租户 ID 的值，使示例正常工作。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-232">Replace the values for authorization token, callback URL, application ID, application name, user ID, user name, and tenant ID to make the example work.</span></span>

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
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "applicationInstance": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "3d913abb-aec0-4964-8fa6-3c6850c4f278"
      },
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
        "phone": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "+12345678901"
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

#### <a name="response"></a><span data-ttu-id="b4d9c-233">响应</span><span class="sxs-lookup"><span data-stu-id="b4d9c-233">Response</span></span>

> <span data-ttu-id="b4d9c-234">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b4d9c-234">**Note:** The response object shown here might be shortened for readability.</span></span> 

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
      "applicationInstance": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "3d913abb-aec0-4964-8fa6-3c6850c4f278"
      },
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
        "phone": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "+12345678901"
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
  "transcription": null,
  "meetingCapability": null,
  "toneInfo": null
}
```

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
