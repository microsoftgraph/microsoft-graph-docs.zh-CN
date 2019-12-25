---
title: 呼叫：应答
description: 应答传入呼叫。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: ab0380bca750f53e4f89c32c072843fd53849675
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868287"
---
# <a name="call-answer"></a><span data-ttu-id="0e016-103">呼叫：应答</span><span class="sxs-lookup"><span data-stu-id="0e016-103">call: answer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e016-104">使机器人能够应答传入[呼叫](../resources/call.md)。</span><span class="sxs-lookup"><span data-stu-id="0e016-104">Enable a bot to answer an incoming [call](../resources/call.md).</span></span> <span data-ttu-id="0e016-105">传入呼叫请求可以是来自组呼叫或对等呼叫中参与者的邀请。</span><span class="sxs-lookup"><span data-stu-id="0e016-105">The incoming call request can be an invite from a participant in a group call or a peer-to-peer call.</span></span> <span data-ttu-id="0e016-106">如果收到某个组呼叫邀请，则通知将包含[chatInfo](../resources/chatinfo.md)和[meetingInfo](../resources/meetinginfo.md)参数。</span><span class="sxs-lookup"><span data-stu-id="0e016-106">If an invite to a group call is received, the notification will contain the [chatInfo](../resources/chatinfo.md) and [meetingInfo](../resources/meetinginfo.md) parameters.</span></span>

<span data-ttu-id="0e016-107">在呼叫超时之前，机器人应应答、[拒绝](./call-reject.md)或[重定向](./call-redirect.md)呼叫。当前超时值为15秒。</span><span class="sxs-lookup"><span data-stu-id="0e016-107">The bot is expected to answer, [reject](./call-reject.md) or [redirect](./call-redirect.md) the call before the call times out. The current timeout value is 15 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e016-108">权限</span><span class="sxs-lookup"><span data-stu-id="0e016-108">Permissions</span></span>
<span data-ttu-id="0e016-109">您无需任何权限即可应答对等呼叫。</span><span class="sxs-lookup"><span data-stu-id="0e016-109">You do not need any permissions to answer a peer-to-peer call.</span></span> <span data-ttu-id="0e016-110">若要加入组呼叫，您需要以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="0e016-110">You need one of the following permissions to join a group call.</span></span> <span data-ttu-id="0e016-111">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0e016-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0e016-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="0e016-112">Permission type</span></span> | <span data-ttu-id="0e016-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0e016-113">Permissions (from least to most privileged)</span></span>                 |
| :-------------- | :-----------------------------------------------------------|
| <span data-ttu-id="0e016-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0e016-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="0e016-115">不支持</span><span class="sxs-lookup"><span data-stu-id="0e016-115">Not Supported</span></span>                        |
| <span data-ttu-id="0e016-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0e016-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e016-117">不支持</span><span class="sxs-lookup"><span data-stu-id="0e016-117">Not Supported</span></span>                        |
| <span data-ttu-id="0e016-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="0e016-118">Application</span></span>     | <span data-ttu-id="0e016-119">JoinGroupCalls 或 JoinGroupCallsasGuest 的所有请求。</span><span class="sxs-lookup"><span data-stu-id="0e016-119">Calls.JoinGroupCalls.All or Calls.JoinGroupCallsasGuest.All</span></span> |

> <span data-ttu-id="0e016-120">**注意：** 对于使用应用程序托管媒体的呼叫，您还需要 AccessMedia 权限。</span><span class="sxs-lookup"><span data-stu-id="0e016-120">**Note:** For a call that uses application-hosted media, you also need the Calls.AccessMedia.All permission.</span></span> <span data-ttu-id="0e016-121">您必须至少具有以下权限之一，才能确保传入呼叫通知中`source`的解密： AccessMedia、InitiateGroupCall、Calls、JoinGroupCall、、、、、、JoinGroupCallAsGuest 等。</span><span class="sxs-lookup"><span data-stu-id="0e016-121">You must have at least one of the following permissions to ensure that the `source` in the incoming call notification is decrypted: Calls.AccessMedia.All, Calls.Initiate.All, Calls.InitiateGroupCall.All, Calls.JoinGroupCall.All, Calls.JoinGroupCallAsGuest.All.</span></span> <span data-ttu-id="0e016-122">`source`是传入呼叫通知中的呼叫者信息。</span><span class="sxs-lookup"><span data-stu-id="0e016-122">The `source` is the caller info in the incoming call notification.</span></span> <span data-ttu-id="0e016-123">如果至少缺少其中一个权限，则`source`将保持加密。</span><span class="sxs-lookup"><span data-stu-id="0e016-123">Without at least one of these permissions, the `source` will remain encrypted.</span></span>

## <a name="http-request"></a><span data-ttu-id="0e016-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e016-124">HTTP request</span></span>
<!-- {"blockType": "ignored" } -->
```http
POST /app/calls/{id}/answer
POST /communications/calls/{id}/answer
```
> <span data-ttu-id="0e016-125">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="0e016-125">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="0e016-126">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="0e016-126">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0e016-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="0e016-127">Request headers</span></span>
| <span data-ttu-id="0e016-128">名称</span><span class="sxs-lookup"><span data-stu-id="0e016-128">Name</span></span>          | <span data-ttu-id="0e016-129">说明</span><span class="sxs-lookup"><span data-stu-id="0e016-129">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="0e016-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e016-130">Authorization</span></span> | <span data-ttu-id="0e016-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0e016-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0e016-133">Content-type</span><span class="sxs-lookup"><span data-stu-id="0e016-133">Content-type</span></span>  | <span data-ttu-id="0e016-p106">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0e016-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0e016-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="0e016-136">Request body</span></span>
<span data-ttu-id="0e016-137">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="0e016-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0e016-138">参数</span><span class="sxs-lookup"><span data-stu-id="0e016-138">Parameter</span></span>        | <span data-ttu-id="0e016-139">类型</span><span class="sxs-lookup"><span data-stu-id="0e016-139">Type</span></span>                                     |<span data-ttu-id="0e016-140">说明</span><span class="sxs-lookup"><span data-stu-id="0e016-140">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="0e016-141">callbackUri</span><span class="sxs-lookup"><span data-stu-id="0e016-141">callbackUri</span></span>       |<span data-ttu-id="0e016-142">String</span><span class="sxs-lookup"><span data-stu-id="0e016-142">String</span></span>                                    |<span data-ttu-id="0e016-143">允许 bot 为当前呼叫提供特定的回调 URI，以接收后续通知。</span><span class="sxs-lookup"><span data-stu-id="0e016-143">Allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="0e016-144">如果尚未设置此属性，则将改为使用 bot 的全局回调 URI。</span><span class="sxs-lookup"><span data-stu-id="0e016-144">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="0e016-145">这必须是`https`。</span><span class="sxs-lookup"><span data-stu-id="0e016-145">This must be `https`.</span></span>    |
|<span data-ttu-id="0e016-146">acceptedModalities</span><span class="sxs-lookup"><span data-stu-id="0e016-146">acceptedModalities</span></span>|<span data-ttu-id="0e016-147">String collection</span><span class="sxs-lookup"><span data-stu-id="0e016-147">String collection</span></span>                         |<span data-ttu-id="0e016-148">接受形式的列表。</span><span class="sxs-lookup"><span data-stu-id="0e016-148">The list of accept modalities.</span></span> <span data-ttu-id="0e016-149">可能的值为`audio`： `video`、 `videoBasedScreenSharing`、。</span><span class="sxs-lookup"><span data-stu-id="0e016-149">Possible value are: `audio`, `video`, `videoBasedScreenSharing`.</span></span> <span data-ttu-id="0e016-150">应答呼叫的必选。</span><span class="sxs-lookup"><span data-stu-id="0e016-150">Required for answering a call.</span></span> |
|<span data-ttu-id="0e016-151">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="0e016-151">mediaConfig</span></span>       | <span data-ttu-id="0e016-152">[appHostedMediaConfig](../resources/apphostedmediaconfig.md) 或 [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)</span><span class="sxs-lookup"><span data-stu-id="0e016-152">[appHostedMediaConfig](../resources/apphostedmediaconfig.md) or [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)</span></span> |<span data-ttu-id="0e016-153">媒体配置。</span><span class="sxs-lookup"><span data-stu-id="0e016-153">The media configuration.</span></span> <span data-ttu-id="0e016-154">需要</span><span class="sxs-lookup"><span data-stu-id="0e016-154">(Required)</span></span>                                                                                                            |

## <a name="response"></a><span data-ttu-id="0e016-155">响应</span><span class="sxs-lookup"><span data-stu-id="0e016-155">Response</span></span>
<span data-ttu-id="0e016-156">此方法返回`202 Accepted`响应代码。</span><span class="sxs-lookup"><span data-stu-id="0e016-156">This method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="0e016-157">示例</span><span class="sxs-lookup"><span data-stu-id="0e016-157">Examples</span></span>
<span data-ttu-id="0e016-158">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="0e016-158">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="0e016-159">请求</span><span class="sxs-lookup"><span data-stu-id="0e016-159">Request</span></span>
<span data-ttu-id="0e016-160">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="0e016-160">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0e016-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e016-161">HTTP</span></span>](#tab/http)
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
<span data-ttu-id="0e016-162">此 blob 是从媒体 SDK 生成的媒体会话的序列化配置。</span><span class="sxs-lookup"><span data-stu-id="0e016-162">This blob is the serialized configuration for media sessions which is generated from the media SDK.</span></span>

# <a name="ctabcsharp"></a>[<span data-ttu-id="0e016-163">C#</span><span class="sxs-lookup"><span data-stu-id="0e016-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0e016-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e016-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0e016-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e016-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0e016-166">响应</span><span class="sxs-lookup"><span data-stu-id="0e016-166">Response</span></span>
<span data-ttu-id="0e016-167">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0e016-167">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-1-answer-a-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="0e016-168">示例1：使用服务托管媒体应答对等 VoIP 呼叫</span><span class="sxs-lookup"><span data-stu-id="0e016-168">Example 1: Answer a Peer-to-Peer VoIP call with service hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="0e016-169">通知传入</span><span class="sxs-lookup"><span data-stu-id="0e016-169">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="0e016-170">请求</span><span class="sxs-lookup"><span data-stu-id="0e016-170">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="0e016-171">响应</span><span class="sxs-lookup"><span data-stu-id="0e016-171">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="0e016-172">通知-建立</span><span class="sxs-lookup"><span data-stu-id="0e016-172">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="0e016-173">已建立通知</span><span class="sxs-lookup"><span data-stu-id="0e016-173">Notification - established</span></span>

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

### <a name="example-2-answer-voip-call-with-application-hosted-media"></a><span data-ttu-id="0e016-174">示例2：使用应用程序托管媒体应答 VOIP 呼叫</span><span class="sxs-lookup"><span data-stu-id="0e016-174">Example 2: Answer VOIP call with application hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="0e016-175">通知传入</span><span class="sxs-lookup"><span data-stu-id="0e016-175">Notification - incoming</span></span>

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
            "@odata.type": "#microsoft.graph.invitationParticipantInfo",
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

##### <a name="request"></a><span data-ttu-id="0e016-176">请求</span><span class="sxs-lookup"><span data-stu-id="0e016-176">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0e016-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e016-177">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="0e016-178">C#</span><span class="sxs-lookup"><span data-stu-id="0e016-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-app-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0e016-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e016-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-app-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0e016-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e016-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-app-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0e016-181">响应</span><span class="sxs-lookup"><span data-stu-id="0e016-181">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="0e016-182">通知-建立</span><span class="sxs-lookup"><span data-stu-id="0e016-182">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="0e016-183">已建立通知</span><span class="sxs-lookup"><span data-stu-id="0e016-183">Notification - established</span></span>

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
