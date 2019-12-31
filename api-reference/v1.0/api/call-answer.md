---
title: 呼叫：应答
description: 应答传入呼叫。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 4df2ddafad5dc2dd22852101f32ba46f8f15fe56
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913371"
---
# <a name="call-answer"></a><span data-ttu-id="7002f-103">呼叫：应答</span><span class="sxs-lookup"><span data-stu-id="7002f-103">call: answer</span></span>

<span data-ttu-id="7002f-104">使机器人能够应答传入[呼叫](../resources/call.md)。</span><span class="sxs-lookup"><span data-stu-id="7002f-104">Enable a bot to answer an incoming [call](../resources/call.md).</span></span> <span data-ttu-id="7002f-105">传入呼叫请求可以是来自组呼叫或对等呼叫中参与者的邀请。</span><span class="sxs-lookup"><span data-stu-id="7002f-105">The incoming call request can be an invite from a participant in a group call or a peer-to-peer call.</span></span> <span data-ttu-id="7002f-106">如果收到某个组呼叫邀请，则通知将包含[chatInfo](../resources/chatinfo.md)和[meetingInfo](../resources/meetinginfo.md)参数。</span><span class="sxs-lookup"><span data-stu-id="7002f-106">If an invite to a group call is received, the notification will contain the [chatInfo](../resources/chatinfo.md) and [meetingInfo](../resources/meetinginfo.md) parameters.</span></span>

<span data-ttu-id="7002f-107">在呼叫超时之前，机器人应应答、[拒绝](./call-reject.md)或[重定向](./call-redirect.md)呼叫。当前超时值为15秒。</span><span class="sxs-lookup"><span data-stu-id="7002f-107">The bot is expected to answer, [reject](./call-reject.md), or [redirect](./call-redirect.md) the call before the call times out. The current timeout value is 15 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="7002f-108">权限</span><span class="sxs-lookup"><span data-stu-id="7002f-108">Permissions</span></span>
<span data-ttu-id="7002f-109">您无需任何权限即可应答对等呼叫。</span><span class="sxs-lookup"><span data-stu-id="7002f-109">You do not need any permissions to answer a peer-to-peer call.</span></span> <span data-ttu-id="7002f-110">若要加入组呼叫，您需要以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="7002f-110">You need one of the following permissions to join a group call.</span></span> <span data-ttu-id="7002f-111">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7002f-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7002f-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="7002f-112">Permission type</span></span> | <span data-ttu-id="7002f-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7002f-113">Permissions (from least to most privileged)</span></span>                 |
| :-------------- | :-----------------------------------------------------------|
| <span data-ttu-id="7002f-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7002f-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="7002f-115">不支持</span><span class="sxs-lookup"><span data-stu-id="7002f-115">Not Supported</span></span>                        |
| <span data-ttu-id="7002f-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7002f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7002f-117">不支持</span><span class="sxs-lookup"><span data-stu-id="7002f-117">Not Supported</span></span>                        |
| <span data-ttu-id="7002f-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="7002f-118">Application</span></span>     | <span data-ttu-id="7002f-119">JoinGroupCalls 或 JoinGroupCallsasGuest 的所有请求。</span><span class="sxs-lookup"><span data-stu-id="7002f-119">Calls.JoinGroupCalls.All or Calls.JoinGroupCallsasGuest.All</span></span> |

> <span data-ttu-id="7002f-120">**注意：** 对于使用应用程序托管媒体的呼叫，您还需要 AccessMedia 权限。</span><span class="sxs-lookup"><span data-stu-id="7002f-120">**Note:** For a call that uses application-hosted media, you also need the Calls.AccessMedia.All permission.</span></span> <span data-ttu-id="7002f-121">您必须至少具有以下权限之一，才能确保传入呼叫通知中`source`的解密： AccessMedia、InitiateGroupCall、Calls、JoinGroupCall、、、、、、JoinGroupCallAsGuest 等。</span><span class="sxs-lookup"><span data-stu-id="7002f-121">You must have at least one of the following permissions to ensure that the `source` in the incoming call notification is decrypted: Calls.AccessMedia.All, Calls.Initiate.All, Calls.InitiateGroupCall.All, Calls.JoinGroupCall.All, Calls.JoinGroupCallAsGuest.All.</span></span> <span data-ttu-id="7002f-122">`source`是传入呼叫通知中的呼叫者信息。</span><span class="sxs-lookup"><span data-stu-id="7002f-122">The `source` is the caller info in the incoming call notification.</span></span> <span data-ttu-id="7002f-123">如果至少缺少其中一个权限，则`source`将保持加密。</span><span class="sxs-lookup"><span data-stu-id="7002f-123">Without at least one of these permissions, the `source` will remain encrypted.</span></span>

## <a name="http-request"></a><span data-ttu-id="7002f-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7002f-124">HTTP request</span></span>
<!-- {"blockType": "ignored" } -->
```http
POST /communications/calls/{id}/answer
```

## <a name="request-headers"></a><span data-ttu-id="7002f-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="7002f-125">Request headers</span></span>
| <span data-ttu-id="7002f-126">名称</span><span class="sxs-lookup"><span data-stu-id="7002f-126">Name</span></span>          | <span data-ttu-id="7002f-127">说明</span><span class="sxs-lookup"><span data-stu-id="7002f-127">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="7002f-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="7002f-128">Authorization</span></span> | <span data-ttu-id="7002f-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7002f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7002f-131">Content-type</span><span class="sxs-lookup"><span data-stu-id="7002f-131">Content-type</span></span>  | <span data-ttu-id="7002f-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="7002f-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7002f-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="7002f-134">Request body</span></span>
<span data-ttu-id="7002f-135">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="7002f-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7002f-136">参数</span><span class="sxs-lookup"><span data-stu-id="7002f-136">Parameter</span></span>        | <span data-ttu-id="7002f-137">类型</span><span class="sxs-lookup"><span data-stu-id="7002f-137">Type</span></span>                                     |<span data-ttu-id="7002f-138">说明</span><span class="sxs-lookup"><span data-stu-id="7002f-138">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="7002f-139">callbackUri</span><span class="sxs-lookup"><span data-stu-id="7002f-139">callbackUri</span></span>       |<span data-ttu-id="7002f-140">String</span><span class="sxs-lookup"><span data-stu-id="7002f-140">String</span></span>                                    |<span data-ttu-id="7002f-141">允许 bot 为当前呼叫提供特定的回调 URI，以接收后续通知。</span><span class="sxs-lookup"><span data-stu-id="7002f-141">Allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="7002f-142">如果尚未设置此属性，则将改为使用 bot 的全局回调 URI。</span><span class="sxs-lookup"><span data-stu-id="7002f-142">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="7002f-143">这必须是`https`。</span><span class="sxs-lookup"><span data-stu-id="7002f-143">This must be `https`.</span></span>    |
|<span data-ttu-id="7002f-144">acceptedModalities</span><span class="sxs-lookup"><span data-stu-id="7002f-144">acceptedModalities</span></span>|<span data-ttu-id="7002f-145">String collection</span><span class="sxs-lookup"><span data-stu-id="7002f-145">String collection</span></span>                         |<span data-ttu-id="7002f-146">接受形式的列表。</span><span class="sxs-lookup"><span data-stu-id="7002f-146">The list of accept modalities.</span></span> <span data-ttu-id="7002f-147">可取值为：`audio`、`video`、`videoBasedScreenSharing`。</span><span class="sxs-lookup"><span data-stu-id="7002f-147">Possible values are: `audio`, `video`, `videoBasedScreenSharing`.</span></span> <span data-ttu-id="7002f-148">应答呼叫的必选。</span><span class="sxs-lookup"><span data-stu-id="7002f-148">Required for answering a call.</span></span> |
|<span data-ttu-id="7002f-149">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="7002f-149">mediaConfig</span></span>       | <span data-ttu-id="7002f-150">[appHostedMediaConfig](../resources/apphostedmediaconfig.md) 或 [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)</span><span class="sxs-lookup"><span data-stu-id="7002f-150">[appHostedMediaConfig](../resources/apphostedmediaconfig.md) or [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)</span></span> |<span data-ttu-id="7002f-151">媒体配置。</span><span class="sxs-lookup"><span data-stu-id="7002f-151">The media configuration.</span></span> <span data-ttu-id="7002f-152">需要</span><span class="sxs-lookup"><span data-stu-id="7002f-152">(Required)</span></span>                                                                                                            |

## <a name="response"></a><span data-ttu-id="7002f-153">响应</span><span class="sxs-lookup"><span data-stu-id="7002f-153">Response</span></span>
<span data-ttu-id="7002f-154">此方法返回`202 Accepted`响应代码。</span><span class="sxs-lookup"><span data-stu-id="7002f-154">This method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7002f-155">示例</span><span class="sxs-lookup"><span data-stu-id="7002f-155">Examples</span></span>
<span data-ttu-id="7002f-156">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="7002f-156">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="7002f-157">请求</span><span class="sxs-lookup"><span data-stu-id="7002f-157">Request</span></span>
<span data-ttu-id="7002f-158">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="7002f-158">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7002f-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="7002f-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-answer"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/{id}/answer
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
<span data-ttu-id="7002f-160">此 blob 是从媒体 SDK 生成的媒体会话的序列化配置。</span><span class="sxs-lookup"><span data-stu-id="7002f-160">This blob is the serialized configuration for media sessions which is generated from the media SDK.</span></span>

# <a name="ctabcsharp"></a>[<span data-ttu-id="7002f-161">C#</span><span class="sxs-lookup"><span data-stu-id="7002f-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7002f-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7002f-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7002f-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7002f-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7002f-164">Java</span><span class="sxs-lookup"><span data-stu-id="7002f-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-answer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7002f-165">响应</span><span class="sxs-lookup"><span data-stu-id="7002f-165">Response</span></span>
<span data-ttu-id="7002f-166">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7002f-166">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-1-answer-a-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="7002f-167">示例1：使用服务托管媒体应答对等 VoIP 呼叫</span><span class="sxs-lookup"><span data-stu-id="7002f-167">Example 1: Answer a Peer-to-Peer VoIP call with service hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="7002f-168">通知传入</span><span class="sxs-lookup"><span data-stu-id="7002f-168">Notification - incoming</span></span>

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
            }
          }
        ],
        "requestedModalities": [ "audio" ]
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="7002f-169">请求</span><span class="sxs-lookup"><span data-stu-id="7002f-169">Request</span></span>

<!-- {
  "blockType": "request",
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

##### <a name="response"></a><span data-ttu-id="7002f-170">响应</span><span class="sxs-lookup"><span data-stu-id="7002f-170">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="7002f-171">通知-建立</span><span class="sxs-lookup"><span data-stu-id="7002f-171">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="7002f-172">已建立通知</span><span class="sxs-lookup"><span data-stu-id="7002f-172">Notification - established</span></span>

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

### <a name="example-2-answer-voip-call-with-application-hosted-media"></a><span data-ttu-id="7002f-173">示例2：使用应用程序托管媒体应答 VOIP 呼叫</span><span class="sxs-lookup"><span data-stu-id="7002f-173">Example 2: Answer VOIP call with application hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="7002f-174">通知传入</span><span class="sxs-lookup"><span data-stu-id="7002f-174">Notification - incoming</span></span>

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
            }
          }
        ],
        "requestedModalities": [ "audio" ]
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="7002f-175">请求</span><span class="sxs-lookup"><span data-stu-id="7002f-175">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7002f-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="7002f-176">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="7002f-177">C#</span><span class="sxs-lookup"><span data-stu-id="7002f-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-app-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7002f-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7002f-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-app-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7002f-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7002f-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-app-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7002f-180">Java</span><span class="sxs-lookup"><span data-stu-id="7002f-180">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-answer-app-hosted-media-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7002f-181">响应</span><span class="sxs-lookup"><span data-stu-id="7002f-181">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="7002f-182">通知-建立</span><span class="sxs-lookup"><span data-stu-id="7002f-182">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="7002f-183">已建立通知</span><span class="sxs-lookup"><span data-stu-id="7002f-183">Notification - established</span></span>

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
