---
title: 呼叫：应答
description: 应答传入呼叫。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 344aa48fd3b816e5d72141a5388fd1abdce50406
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/20/2019
ms.locfileid: "38747593"
---
# <a name="call-answer"></a><span data-ttu-id="6cc54-103">呼叫：应答</span><span class="sxs-lookup"><span data-stu-id="6cc54-103">call: answer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6cc54-104">使机器人能够应答传入[呼叫](../resources/call.md)。</span><span class="sxs-lookup"><span data-stu-id="6cc54-104">Enable a bot to answer an incoming [call](../resources/call.md).</span></span> <span data-ttu-id="6cc54-105">传入呼叫请求可以是来自组呼叫或对等呼叫中参与者的邀请。</span><span class="sxs-lookup"><span data-stu-id="6cc54-105">The incoming call request can be an invite from a participant in a group call or a peer-to-peer call.</span></span> <span data-ttu-id="6cc54-106">如果收到某个组呼叫邀请，则通知将包含[chatInfo](../resources/chatinfo.md)和[meetingInfo](../resources/meetinginfo.md)参数。</span><span class="sxs-lookup"><span data-stu-id="6cc54-106">If an invite to a group call is received, the notification will contain the [chatInfo](../resources/chatinfo.md) and [meetingInfo](../resources/meetinginfo.md) parameters.</span></span>

<span data-ttu-id="6cc54-107">在呼叫超时之前，机器人应应答或[拒绝](./call-reject.md)呼叫。当前超时值为15秒。</span><span class="sxs-lookup"><span data-stu-id="6cc54-107">The bot is expected to answer or [reject](./call-reject.md) the call before the call times out. The current timeout value is 15 seconds.</span></span>

> <span data-ttu-id="6cc54-108">**注意：** 自动程序只能通过 VoIP 访问机器人。</span><span class="sxs-lookup"><span data-stu-id="6cc54-108">**Note:** The bot can only be reached by VoIP.</span></span> <span data-ttu-id="6cc54-109">不支持 PSTN 呼叫。</span><span class="sxs-lookup"><span data-stu-id="6cc54-109">PSTN calling isn't supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="6cc54-110">权限</span><span class="sxs-lookup"><span data-stu-id="6cc54-110">Permissions</span></span>
<span data-ttu-id="6cc54-111">您无需任何权限即可应答对等呼叫。</span><span class="sxs-lookup"><span data-stu-id="6cc54-111">You do not need any permissions to answer a peer-to-peer call.</span></span> <span data-ttu-id="6cc54-112">若要加入组呼叫，您需要以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="6cc54-112">You need one of the following permissions to join a group call.</span></span> <span data-ttu-id="6cc54-113">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6cc54-113">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6cc54-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="6cc54-114">Permission type</span></span> | <span data-ttu-id="6cc54-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6cc54-115">Permissions (from least to most privileged)</span></span>                 |
| :-------------- | :-----------------------------------------------------------|
| <span data-ttu-id="6cc54-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6cc54-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="6cc54-117">不支持</span><span class="sxs-lookup"><span data-stu-id="6cc54-117">Not Supported</span></span>                        |
| <span data-ttu-id="6cc54-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6cc54-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6cc54-119">不支持</span><span class="sxs-lookup"><span data-stu-id="6cc54-119">Not Supported</span></span>                        |
| <span data-ttu-id="6cc54-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="6cc54-120">Application</span></span>     | <span data-ttu-id="6cc54-121">JoinGroupCalls 或 JoinGroupCallsasGuest 的所有请求。</span><span class="sxs-lookup"><span data-stu-id="6cc54-121">Calls.JoinGroupCalls.All or Calls.JoinGroupCallsasGuest.All</span></span> |

> <span data-ttu-id="6cc54-122">**注意：** 对于使用应用程序托管媒体的呼叫，您还需要 AccessMedia 权限。</span><span class="sxs-lookup"><span data-stu-id="6cc54-122">**Note:** For a call that uses application-hosted media, you also need the Calls.AccessMedia.All permission.</span></span> <span data-ttu-id="6cc54-123">您必须至少具有以下权限之一，才能确保传入呼叫通知中`source`的解密： AccessMedia、InitiateGroupCall、Calls、JoinGroupCall、、、、、、JoinGroupCallAsGuest 等。</span><span class="sxs-lookup"><span data-stu-id="6cc54-123">You must have at least one of the following permissions to ensure that the `source` in the incoming call notification is decrypted: Calls.AccessMedia.All, Calls.Initiate.All, Calls.InitiateGroupCall.All, Calls.JoinGroupCall.All, Calls.JoinGroupCallAsGuest.All.</span></span> <span data-ttu-id="6cc54-124">`source`是传入呼叫通知中的呼叫者信息。</span><span class="sxs-lookup"><span data-stu-id="6cc54-124">The `source` is the caller info in the incoming call notification.</span></span> <span data-ttu-id="6cc54-125">如果至少缺少其中一个权限，则`source`将保持加密。</span><span class="sxs-lookup"><span data-stu-id="6cc54-125">Without at least one of these permissions, the `source` will remain encrypted.</span></span>

## <a name="http-request"></a><span data-ttu-id="6cc54-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6cc54-126">HTTP request</span></span>
<!-- {"blockType": "ignored" } -->
```http
POST /app/calls/{id}/answer
POST /communications/calls/{id}/answer
```
> <span data-ttu-id="6cc54-127">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="6cc54-127">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="6cc54-128">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="6cc54-128">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6cc54-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="6cc54-129">Request headers</span></span>
| <span data-ttu-id="6cc54-130">名称</span><span class="sxs-lookup"><span data-stu-id="6cc54-130">Name</span></span>          | <span data-ttu-id="6cc54-131">说明</span><span class="sxs-lookup"><span data-stu-id="6cc54-131">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="6cc54-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cc54-132">Authorization</span></span> | <span data-ttu-id="6cc54-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6cc54-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6cc54-135">Content-type</span><span class="sxs-lookup"><span data-stu-id="6cc54-135">Content-type</span></span>  | <span data-ttu-id="6cc54-p107">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="6cc54-p107">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6cc54-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="6cc54-138">Request body</span></span>
<span data-ttu-id="6cc54-139">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="6cc54-139">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6cc54-140">参数</span><span class="sxs-lookup"><span data-stu-id="6cc54-140">Parameter</span></span>        | <span data-ttu-id="6cc54-141">类型</span><span class="sxs-lookup"><span data-stu-id="6cc54-141">Type</span></span>                                     |<span data-ttu-id="6cc54-142">说明</span><span class="sxs-lookup"><span data-stu-id="6cc54-142">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="6cc54-143">callbackUri</span><span class="sxs-lookup"><span data-stu-id="6cc54-143">callbackUri</span></span>       |<span data-ttu-id="6cc54-144">String</span><span class="sxs-lookup"><span data-stu-id="6cc54-144">String</span></span>                                    |<span data-ttu-id="6cc54-145">允许 bot 为当前呼叫提供特定的回调 URI，以接收后续通知。</span><span class="sxs-lookup"><span data-stu-id="6cc54-145">Allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="6cc54-146">如果尚未设置此属性，则将改为使用 bot 的全局回调 URI。</span><span class="sxs-lookup"><span data-stu-id="6cc54-146">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="6cc54-147">这必须是`https`。</span><span class="sxs-lookup"><span data-stu-id="6cc54-147">This must be `https`.</span></span>    |
|<span data-ttu-id="6cc54-148">acceptedModalities</span><span class="sxs-lookup"><span data-stu-id="6cc54-148">acceptedModalities</span></span>|<span data-ttu-id="6cc54-149">String collection</span><span class="sxs-lookup"><span data-stu-id="6cc54-149">String collection</span></span>                         |<span data-ttu-id="6cc54-150">接受形式的列表。</span><span class="sxs-lookup"><span data-stu-id="6cc54-150">The list of accept modalities.</span></span> <span data-ttu-id="6cc54-151">可能的值为`audio`： `video`、 `videoBasedScreenSharing`、。</span><span class="sxs-lookup"><span data-stu-id="6cc54-151">Possible value are: `audio`, `video`, `videoBasedScreenSharing`.</span></span> <span data-ttu-id="6cc54-152">应答呼叫的必选。</span><span class="sxs-lookup"><span data-stu-id="6cc54-152">Required for answering a call.</span></span> |
|<span data-ttu-id="6cc54-153">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="6cc54-153">mediaConfig</span></span>       | <span data-ttu-id="6cc54-154">[appHostedMediaConfig](../resources/apphostedmediaconfig.md) 或 [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)</span><span class="sxs-lookup"><span data-stu-id="6cc54-154">[appHostedMediaConfig](../resources/apphostedmediaconfig.md) or [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)</span></span> |<span data-ttu-id="6cc54-155">媒体配置。</span><span class="sxs-lookup"><span data-stu-id="6cc54-155">The media configuration.</span></span> <span data-ttu-id="6cc54-156">需要</span><span class="sxs-lookup"><span data-stu-id="6cc54-156">(Required)</span></span>                                                                                                            |

## <a name="response"></a><span data-ttu-id="6cc54-157">响应</span><span class="sxs-lookup"><span data-stu-id="6cc54-157">Response</span></span>
<span data-ttu-id="6cc54-158">此方法返回`202 Accepted`响应代码。</span><span class="sxs-lookup"><span data-stu-id="6cc54-158">This method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6cc54-159">示例</span><span class="sxs-lookup"><span data-stu-id="6cc54-159">Examples</span></span>
<span data-ttu-id="6cc54-160">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="6cc54-160">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="6cc54-161">请求</span><span class="sxs-lookup"><span data-stu-id="6cc54-161">Request</span></span>
<span data-ttu-id="6cc54-162">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="6cc54-162">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6cc54-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="6cc54-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-answer"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/answer
Content-Type: application/json
Content-Length: 211

{
  "callbackUri": "callbackUri-value",
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<Media Session Configuration Blob>"
  },
  "acceptedModalities": [
    "audio"
  ]
}
```
<span data-ttu-id="6cc54-164">此 blob 是从媒体 SDK 生成的媒体会话的序列化配置。</span><span class="sxs-lookup"><span data-stu-id="6cc54-164">This blob is the serialized configuration for media sessions which is generated from the media SDK.</span></span>

# <a name="ctabcsharp"></a>[<span data-ttu-id="6cc54-165">C#</span><span class="sxs-lookup"><span data-stu-id="6cc54-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6cc54-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6cc54-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6cc54-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6cc54-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6cc54-168">响应</span><span class="sxs-lookup"><span data-stu-id="6cc54-168">Response</span></span>
<span data-ttu-id="6cc54-169">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6cc54-169">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-1-answer-a-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="6cc54-170">示例1：使用服务托管媒体应答对等 VoIP 呼叫</span><span class="sxs-lookup"><span data-stu-id="6cc54-170">Example 1: Answer a Peer-to-Peer VoIP call with service hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="6cc54-171">通知传入</span><span class="sxs-lookup"><span data-stu-id="6cc54-171">Notification - incoming</span></span>

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
      "changeType": "created",
      "resourceUrl": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "incoming",
        "direction": "incoming",
        "callRoutes": [
          {
            "routingType": "lookup",
            "original": {
              "phone": {
                "id": "+14258828080"
              }
            },
            "final": {
              "user": {
                "id": "29362BD4-CD58-4ED0-A206-0E4A33DBB0B6",
                "displayName": "Heidi Steen"
              }
            }
          }
        ],
        "source": {
          "identity": {
            "user": {
              "displayName": "Test User",
              "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
            }
          },
          "region": "westus",
          "languageId": "en-US"
        },
        "targets": [
          {
            "identity": {
              "application": {
                "displayName": "Test BOT",
                "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
              }
            },
            "languageId": "en-US"
          }
        ],
        "requestedModalities": [ "audio" ]
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="6cc54-172">请求</span><span class="sxs-lookup"><span data-stu-id="6cc54-172">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "call-answer-service-hosted-media"
}-->
```http
POST /communications/calls/57DAB8B1894C409AB240BD8BEAE78896/answer
Content-Type: application/json

{
  "callbackUri": "https://bot.contoso.com/api/calls",
  "acceptedModalities": [ "audio" ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
      {
        "uri": "https://cdn.contoso.com/beep.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      },
      {
        "uri": "https://cdn.contoso.com/cool.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088F"
      }
    ]
  }
}
```

##### <a name="response"></a><span data-ttu-id="6cc54-173">响应</span><span class="sxs-lookup"><span data-stu-id="6cc54-173">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="6cc54-174">通知-建立</span><span class="sxs-lookup"><span data-stu-id="6cc54-174">Notification - establishing</span></span>

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
      "resourceUrl": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "establishing"
      }
    }
  ]
}
```

##### <a name="notification---established"></a><span data-ttu-id="6cc54-175">已建立通知</span><span class="sxs-lookup"><span data-stu-id="6cc54-175">Notification - established</span></span>

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
      "resourceUrl": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "established"
      }
    }
  ]
}
```

### <a name="example-2-answer-voip-call-with-application-hosted-media"></a><span data-ttu-id="6cc54-176">示例2：使用应用程序托管媒体应答 VOIP 呼叫</span><span class="sxs-lookup"><span data-stu-id="6cc54-176">Example 2: Answer VOIP call with application hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="6cc54-177">通知传入</span><span class="sxs-lookup"><span data-stu-id="6cc54-177">Notification - incoming</span></span>

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
      "changeType": "created",
      "resourceUrl": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "incoming",
        "direction": "incoming",
        "source": {
          "@odata.type": "#microsoft.graph.participantInfo",
          "identity": {
            "user": {
              "displayName": "Test User",
              "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
            }
          },
          "region": "westus",
          "languageId": "en-US"
        },
        "targets": [
          {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "application": {
                "displayName": "Test BOT",
                "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          }
        ],
        "requestedModalities": [ "audio" ]
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="6cc54-178">请求</span><span class="sxs-lookup"><span data-stu-id="6cc54-178">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6cc54-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="6cc54-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-answer-app-hosted-media"
}-->
```http
POST /communications/calls/57DAB8B1894C409AB240BD8BEAE78896/answer
Content-Type: application/json

{
  "callbackUri": "https://bot.contoso.com/api/calls",
  "acceptedModalities": [ "audio" ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<Media Session Configuration Blob>"
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6cc54-180">C#</span><span class="sxs-lookup"><span data-stu-id="6cc54-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-app-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6cc54-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6cc54-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-app-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6cc54-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6cc54-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-app-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6cc54-183">响应</span><span class="sxs-lookup"><span data-stu-id="6cc54-183">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="6cc54-184">通知-建立</span><span class="sxs-lookup"><span data-stu-id="6cc54-184">Notification - establishing</span></span>

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
      "resourceUrl": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "establishing"
      }
    }
  ]
}
```

##### <a name="notification---established"></a><span data-ttu-id="6cc54-185">已建立通知</span><span class="sxs-lookup"><span data-stu-id="6cc54-185">Notification - established</span></span>

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
      "resourceUrl": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "established"
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
  "description": "call: answer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
