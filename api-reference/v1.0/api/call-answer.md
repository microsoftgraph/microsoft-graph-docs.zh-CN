---
title: call： answer
description: 应答传入呼叫。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: a0cf83ea366e8d2c03c8f3d28f4262bfc9616d65
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2021
ms.locfileid: "53430268"
---
# <a name="call-answer"></a><span data-ttu-id="5a92f-103">call： answer</span><span class="sxs-lookup"><span data-stu-id="5a92f-103">call: answer</span></span>

<span data-ttu-id="5a92f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a92f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5a92f-105">使机器人能够应答传入 [呼叫](../resources/call.md)。</span><span class="sxs-lookup"><span data-stu-id="5a92f-105">Enable a bot to answer an incoming [call](../resources/call.md).</span></span> <span data-ttu-id="5a92f-106">传入呼叫请求可以是来自组呼叫参与者的邀请或对等呼叫。</span><span class="sxs-lookup"><span data-stu-id="5a92f-106">The incoming call request can be an invite from a participant in a group call or a peer-to-peer call.</span></span> <span data-ttu-id="5a92f-107">如果收到组呼叫邀请，通知将包含 [chatInfo](../resources/chatinfo.md) 和 [meetingInfo](../resources/meetinginfo.md) 参数。</span><span class="sxs-lookup"><span data-stu-id="5a92f-107">If an invite to a group call is received, the notification will contain the [chatInfo](../resources/chatinfo.md) and [meetingInfo](../resources/meetinginfo.md) parameters.</span></span>

<span data-ttu-id="5a92f-108">机器人预期在呼叫退出[之前](./call-reject.md)应答、拒绝或[](./call-redirect.md)重定向呼叫。对于常规方案，当前超时值为 15 秒，基于策略的录制方案为 5 秒。</span><span class="sxs-lookup"><span data-stu-id="5a92f-108">The bot is expected to answer, [reject](./call-reject.md), or [redirect](./call-redirect.md) the call before the call times out. The current timeout value is 15 seconds for regular scenarios, and 5 seconds for policy-based recording scenarios.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a92f-109">权限</span><span class="sxs-lookup"><span data-stu-id="5a92f-109">Permissions</span></span>
<span data-ttu-id="5a92f-110">无需任何权限来应答对等呼叫。</span><span class="sxs-lookup"><span data-stu-id="5a92f-110">You do not need any permissions to answer a peer-to-peer call.</span></span> <span data-ttu-id="5a92f-111">需要以下权限之一才能加入组呼叫。</span><span class="sxs-lookup"><span data-stu-id="5a92f-111">You need one of the following permissions to join a group call.</span></span> <span data-ttu-id="5a92f-112">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5a92f-112">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5a92f-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="5a92f-113">Permission type</span></span> | <span data-ttu-id="5a92f-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5a92f-114">Permissions (from least to most privileged)</span></span>                 |
| :-------------- | :-----------------------------------------------------------|
| <span data-ttu-id="5a92f-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5a92f-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="5a92f-116">不支持</span><span class="sxs-lookup"><span data-stu-id="5a92f-116">Not Supported</span></span>                        |
| <span data-ttu-id="5a92f-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5a92f-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a92f-118">不支持</span><span class="sxs-lookup"><span data-stu-id="5a92f-118">Not Supported</span></span>                        |
| <span data-ttu-id="5a92f-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="5a92f-119">Application</span></span>     | <span data-ttu-id="5a92f-120">Calls.JoinGroupCalls.All 或 Calls.JoinGroupCallsasGuest.All</span><span class="sxs-lookup"><span data-stu-id="5a92f-120">Calls.JoinGroupCalls.All or Calls.JoinGroupCallsasGuest.All</span></span> |

> <span data-ttu-id="5a92f-121">**注意：** 对于使用应用程序托管媒体的呼叫，还需要 Calls.AccessMedia.All 权限。</span><span class="sxs-lookup"><span data-stu-id="5a92f-121">**Note:** For a call that uses application-hosted media, you also need the Calls.AccessMedia.All permission.</span></span> <span data-ttu-id="5a92f-122">必须至少具有以下权限之一才能确保传入呼叫通知中的 解密 `source` ：Calls.AccessMedia.All、Calls.Initiate。全部，Calls.InitiateGroupCall.All、Calls.JoinGroupCall.All、Calls.JoinGroupCallAsGuest.All。</span><span class="sxs-lookup"><span data-stu-id="5a92f-122">You must have at least one of the following permissions to ensure that the `source` in the incoming call notification is decrypted: Calls.AccessMedia.All, Calls.Initiate.All, Calls.InitiateGroupCall.All, Calls.JoinGroupCall.All, Calls.JoinGroupCallAsGuest.All.</span></span> <span data-ttu-id="5a92f-123">`source`是传入呼叫通知中的呼叫者信息。</span><span class="sxs-lookup"><span data-stu-id="5a92f-123">The `source` is the caller info in the incoming call notification.</span></span> <span data-ttu-id="5a92f-124">如果没有其中至少一个权限， `source` 将保持加密状态。</span><span class="sxs-lookup"><span data-stu-id="5a92f-124">Without at least one of these permissions, the `source` will remain encrypted.</span></span>

## <a name="http-request"></a><span data-ttu-id="5a92f-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5a92f-125">HTTP request</span></span>
<!-- {"blockType": "ignored" } -->
```http
POST /communications/calls/{id}/answer
```

## <a name="request-headers"></a><span data-ttu-id="5a92f-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="5a92f-126">Request headers</span></span>
| <span data-ttu-id="5a92f-127">名称</span><span class="sxs-lookup"><span data-stu-id="5a92f-127">Name</span></span>          | <span data-ttu-id="5a92f-128">说明</span><span class="sxs-lookup"><span data-stu-id="5a92f-128">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="5a92f-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a92f-129">Authorization</span></span> | <span data-ttu-id="5a92f-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5a92f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5a92f-132">Content-type</span><span class="sxs-lookup"><span data-stu-id="5a92f-132">Content-type</span></span>  | <span data-ttu-id="5a92f-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="5a92f-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a92f-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="5a92f-135">Request body</span></span>
<span data-ttu-id="5a92f-136">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="5a92f-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5a92f-137">参数</span><span class="sxs-lookup"><span data-stu-id="5a92f-137">Parameter</span></span>        | <span data-ttu-id="5a92f-138">类型</span><span class="sxs-lookup"><span data-stu-id="5a92f-138">Type</span></span>                                     |<span data-ttu-id="5a92f-139">说明</span><span class="sxs-lookup"><span data-stu-id="5a92f-139">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="5a92f-140">callbackUri</span><span class="sxs-lookup"><span data-stu-id="5a92f-140">callbackUri</span></span>       |<span data-ttu-id="5a92f-141">String</span><span class="sxs-lookup"><span data-stu-id="5a92f-141">String</span></span>                                    |<span data-ttu-id="5a92f-142">允许机器人为并发呼叫提供特定的回调 URI 以接收以后的通知。</span><span class="sxs-lookup"><span data-stu-id="5a92f-142">Allows bots to provide a specific callback URI for the concurrent call to receive later notifications.</span></span> <span data-ttu-id="5a92f-143">如果尚未设置此属性，将改为使用自动程序全局回调 URI。</span><span class="sxs-lookup"><span data-stu-id="5a92f-143">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="5a92f-144">这必须是 `https` 。</span><span class="sxs-lookup"><span data-stu-id="5a92f-144">This must be `https`.</span></span>    |
|<span data-ttu-id="5a92f-145">acceptedModalities</span><span class="sxs-lookup"><span data-stu-id="5a92f-145">acceptedModalities</span></span>|<span data-ttu-id="5a92f-146">字符串集合</span><span class="sxs-lookup"><span data-stu-id="5a92f-146">String collection</span></span>                         |<span data-ttu-id="5a92f-147">接受形式列表。</span><span class="sxs-lookup"><span data-stu-id="5a92f-147">The list of accept modalities.</span></span> <span data-ttu-id="5a92f-148">可取值为：`audio`、`video`、`videoBasedScreenSharing`。</span><span class="sxs-lookup"><span data-stu-id="5a92f-148">Possible values are: `audio`, `video`, `videoBasedScreenSharing`.</span></span> <span data-ttu-id="5a92f-149">应答呼叫时必需。</span><span class="sxs-lookup"><span data-stu-id="5a92f-149">Required for answering a call.</span></span> |
|<span data-ttu-id="5a92f-150">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="5a92f-150">mediaConfig</span></span>       | <span data-ttu-id="5a92f-151">[appHostedMediaConfig](../resources/apphostedmediaconfig.md) 或 [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)</span><span class="sxs-lookup"><span data-stu-id="5a92f-151">[appHostedMediaConfig](../resources/apphostedmediaconfig.md) or [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)</span></span> |<span data-ttu-id="5a92f-152">媒体配置。</span><span class="sxs-lookup"><span data-stu-id="5a92f-152">The media configuration.</span></span> <span data-ttu-id="5a92f-153"> (必需) </span><span class="sxs-lookup"><span data-stu-id="5a92f-153">(Required)</span></span>                                                                                                            |
| <span data-ttu-id="5a92f-154">participantCapacity</span><span class="sxs-lookup"><span data-stu-id="5a92f-154">participantCapacity</span></span> | <span data-ttu-id="5a92f-155">Int</span><span class="sxs-lookup"><span data-stu-id="5a92f-155">Int</span></span> | <span data-ttu-id="5a92f-156">对于基于策略的录制方案，应用程序可以处理Teams[的数量](/MicrosoftTeams/teams-recording-policy)。</span><span class="sxs-lookup"><span data-stu-id="5a92f-156">The number of participant that the application can handle for the call, for [Teams policy-based recording](/MicrosoftTeams/teams-recording-policy) scenario.</span></span>                                                     |

## <a name="response"></a><span data-ttu-id="5a92f-157">响应</span><span class="sxs-lookup"><span data-stu-id="5a92f-157">Response</span></span>
<span data-ttu-id="5a92f-158">此方法返回 响应 `202 Accepted` 代码。</span><span class="sxs-lookup"><span data-stu-id="5a92f-158">This method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5a92f-159">示例</span><span class="sxs-lookup"><span data-stu-id="5a92f-159">Examples</span></span>
<span data-ttu-id="5a92f-160">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="5a92f-160">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="5a92f-161">请求</span><span class="sxs-lookup"><span data-stu-id="5a92f-161">Request</span></span>
<span data-ttu-id="5a92f-162">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="5a92f-162">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5a92f-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a92f-163">HTTP</span></span>](#tab/http)
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
  ],
  "participantCapacity": 200
}
```
<span data-ttu-id="5a92f-164">此 blob 是由媒体 SDK 生成的媒体会话的序列化配置。</span><span class="sxs-lookup"><span data-stu-id="5a92f-164">This blob is the serialized configuration for media sessions which is generated from the media SDK.</span></span>

# <a name="c"></a>[<span data-ttu-id="5a92f-165">C#</span><span class="sxs-lookup"><span data-stu-id="5a92f-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5a92f-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a92f-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5a92f-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a92f-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5a92f-168">Java</span><span class="sxs-lookup"><span data-stu-id="5a92f-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-answer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5a92f-169">响应</span><span class="sxs-lookup"><span data-stu-id="5a92f-169">Response</span></span>
<span data-ttu-id="5a92f-170">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5a92f-170">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-1-answer-a-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="5a92f-171">示例 1：使用服务托管媒体应答对等 VoIP 呼叫</span><span class="sxs-lookup"><span data-stu-id="5a92f-171">Example 1: Answer a Peer-to-Peer VoIP call with service hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="5a92f-172">通知 - 传入</span><span class="sxs-lookup"><span data-stu-id="5a92f-172">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="5a92f-173">请求</span><span class="sxs-lookup"><span data-stu-id="5a92f-173">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="5a92f-174">响应</span><span class="sxs-lookup"><span data-stu-id="5a92f-174">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="5a92f-175">通知 - 建立</span><span class="sxs-lookup"><span data-stu-id="5a92f-175">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="5a92f-176">通知 - 已建立</span><span class="sxs-lookup"><span data-stu-id="5a92f-176">Notification - established</span></span>

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

### <a name="example-2-answer-voip-call-with-application-hosted-media"></a><span data-ttu-id="5a92f-177">示例 2：使用应用程序托管媒体应答 VOIP 呼叫</span><span class="sxs-lookup"><span data-stu-id="5a92f-177">Example 2: Answer VOIP call with application hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="5a92f-178">通知 - 传入</span><span class="sxs-lookup"><span data-stu-id="5a92f-178">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="5a92f-179">请求</span><span class="sxs-lookup"><span data-stu-id="5a92f-179">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5a92f-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a92f-180">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5a92f-181">C#</span><span class="sxs-lookup"><span data-stu-id="5a92f-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-app-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5a92f-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a92f-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-app-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5a92f-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a92f-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-app-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5a92f-184">Java</span><span class="sxs-lookup"><span data-stu-id="5a92f-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-answer-app-hosted-media-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5a92f-185">响应</span><span class="sxs-lookup"><span data-stu-id="5a92f-185">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="5a92f-186">通知 - 建立</span><span class="sxs-lookup"><span data-stu-id="5a92f-186">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="5a92f-187">通知 - 已建立</span><span class="sxs-lookup"><span data-stu-id="5a92f-187">Notification - established</span></span>

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

### <a name="example-3-answer-a-policy-based-recording-call"></a><span data-ttu-id="5a92f-188">示例 3：应答基于策略的录制呼叫</span><span class="sxs-lookup"><span data-stu-id="5a92f-188">Example 3: Answer a policy-based recording call</span></span>

<span data-ttu-id="5a92f-189">在基于 [策略的录制](/microsoftteams/teams-recording-policy)方案下，在策略下的参与者加入呼叫之前，传入呼叫通知将发送到与该策略关联的机器人。</span><span class="sxs-lookup"><span data-stu-id="5a92f-189">Under the [Policy-based recording scenario](/microsoftteams/teams-recording-policy), before a participant under policy joins a call, an incoming call notification will be sent to the bot associated with the policy.</span></span>
<span data-ttu-id="5a92f-190">可以在 **botData** 属性下找到加入信息。</span><span class="sxs-lookup"><span data-stu-id="5a92f-190">The join information can be found under the **botData** property.</span></span> <span data-ttu-id="5a92f-191">然后，机器人可以选择应答呼叫 [并相应地更新录制](call-updaterecordingstatus.md) 状态。</span><span class="sxs-lookup"><span data-stu-id="5a92f-191">The bot can then choose to answer the call and [update the recording status](call-updaterecordingstatus.md) accordingly.</span></span>

<span data-ttu-id="5a92f-192">当在基于策略的录制通知的请求中指定时，属于同一策略组的后续参与者加入事件将发送为 `participantCapacity` `Answer` [participantJoiningNotification，](../resources/participantJoiningNotification.md)而不是新的传入呼叫通知，直到当前呼叫实例处理的参与者数达到 中指定的号码。 `participantCapacity`</span><span class="sxs-lookup"><span data-stu-id="5a92f-192">When `participantCapacity` is specified in the `Answer` request for a policy-based recording notification, subsequent participant joining event belonging to the same policy group will be sent out as [participantJoiningNotification](../resources/participantJoiningNotification.md) instead of new incoming call notification, until number of participants that current call instance is handling has reached the number specified in `participantCapacity`.</span></span>

<span data-ttu-id="5a92f-193">下面是机器人在这种情况下将收到的传入呼叫通知的示例。</span><span class="sxs-lookup"><span data-stu-id="5a92f-193">Here is an example of the incoming call notification that a bot would recieve in this case.</span></span>

```json
{
   "@odata.type":"#microsoft.graph.commsNotifications",
   "value":[
      {
         "@odata.type":"#microsoft.graph.commsNotification",
         "changeType":"created",
         "resource":"/app/calls/e71f0300-9c1f-4d99-b5f4-2722e877d497",
         "resourceUrl":"/communications/calls/e71f0300-9c1f-4d99-b5f4-2722e877d497",
         "resourceData":{
            "@odata.type":"#microsoft.graph.call",
            "state":"incoming",
            "direction":"incoming",
            "source":{
               "@odata.type":"#microsoft.graph.participantInfo",
               "id":"90fad2ce-8989-41a1-8a66-f6636e629a2a",
               "identity":{
                  "@odata.type":"#microsoft.graph.identitySet",
                  "user":{
                     "@odata.type":"#microsoft.graph.identity",
                     "id":"8A34A46B-3D17-4ADC-8DCE-DC4E7D572698",
                     "identityProvider":"AAD"
                  }
               },
               "endpointType":"default",
               "region":"amer"
            },
            "targets":[
               {
                  "@odata.type":"#microsoft.graph.invitationParticipantInfo",
                  "identity":{
                     "@odata.type":"#microsoft.graph.identitySet",
                     "applicationInstance":{
                        "@odata.type":"#microsoft.graph.identity",
                        "id":"832899f8-2ea1-4604-8413-27bd2892079f",
                        "identityProvider":"AAD"
                     }
                  },
                  "endpointType":"default",
                  "id":"4520a1a5-5394-5a41-aa12-9ee6fa18cfc8",
                  "region":null,
                  "languageId":null
               }
            ],
            "meetingInfo":{
               "@odata.type":"#microsoft.graph.tokenMeetingInfo",
               "token":"join token"
            },
            "tenantId":"932899f8-2ea1-4604-8413-27bd2892079f",
            "myParticipantId":"1520a1a5-5394-4a41-aa72-9ee6fa18cfc8",
            "callChainId":"05f2f70f-3a9c-47c1-80a9-cc79e91d8cec",
            "incomingContext":{
               "@odata.type":"#microsoft.graph.incomingContext",
               "sourceParticipantId":"30fad2ce-8989-41a1-8a66-f6636e629a2a",
               "observedParticipantId":"30fad2ce-8989-41a1-8a66-f6636e629a2a"
            },
            "id":"e71f0300-9c1f-4d99-b5f4-2722e877d497",
            "applicationMetadata":{
               "botData":{
                  "mediaHostedRegion":"USEA",
                  "user":{
                     "participationMethod":"callee",
                     "clientLocation":"US"
                  },
                  "otherSideUser":{
                     "id":"971f0300-9c1f-4d99-b5f4-2722e877d490",
                     "participantId":"3520a1a5-5394-4a41-aa72-9ee6fa18cfc8",
                     "tenantId":"1540a1a5-2394-4a41-aa72-9ee6fa18cfc8",
                     "onBehalfOf":{
                        "id":"871f0300-9c1f-4d99-b5f4-2722e877d490"
                     },
                     "participationMethod":"caller",
                     "clientLocation":"EUNO"
                  },
                  "inviteReasons":[
                     "PolicyBasedRecording"
                  ],
                  "policyIdentifier":"Test Policy",
                  "pairedRecorders":[
                     {
                        "id":"471f0300-5c1f-4d99-b5f4-2722e877d490",
                        "participantId":"371f0300-2c1f-4d99-b5f4-2722e877d490"
                     }
                  ],
                  "otherRecorders":[
                     {
                        "id":"671f0300-9c1f-4d99-b5f4-2722e877d490",
                        "participantId":"a71f0300-ec1f-4d99-b5f4-2722e877d490"
                     }
                  ]
               }
            }
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
