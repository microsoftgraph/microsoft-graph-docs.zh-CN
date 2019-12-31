---
title: 创建调用
description: 创建新呼叫。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 3c10d3ec18e3bfa3704be7a152a10fcfc53760b6
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913616"
---
# <a name="create-call"></a><span data-ttu-id="53b4a-103">创建调用</span><span class="sxs-lookup"><span data-stu-id="53b4a-103">Create call</span></span>

<span data-ttu-id="53b4a-104">创建[呼叫](../resources/call.md)使你的 bot 能够创建新的传出对等或组呼叫，或加入现有会议。</span><span class="sxs-lookup"><span data-stu-id="53b4a-104">Create [call](../resources/call.md) enables your bot to create a new outgoing peer-to-peer or group call, or join an existing meeting.</span></span> <span data-ttu-id="53b4a-105">你需要[注册呼叫机器人](https://docs.microsoft.com/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot)并查看所需的权限列表，如下所述。</span><span class="sxs-lookup"><span data-stu-id="53b4a-105">You will need to [register the calling bot](https://docs.microsoft.com/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot) and go through the list of permissions needed as mentioned below.</span></span>

> <span data-ttu-id="53b4a-106">**注意：** 目前，仅支持 VoIP 呼叫。</span><span class="sxs-lookup"><span data-stu-id="53b4a-106">**Note:** Currently, only VoIP calls are supported.</span></span> 

## <a name="permissions"></a><span data-ttu-id="53b4a-107">权限</span><span class="sxs-lookup"><span data-stu-id="53b4a-107">Permissions</span></span>

<span data-ttu-id="53b4a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](https://docs.microsoft.com/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot#add-microsoft-graph-permissions)。</span><span class="sxs-lookup"><span data-stu-id="53b4a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://docs.microsoft.com/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot#add-microsoft-graph-permissions).</span></span>

| <span data-ttu-id="53b4a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="53b4a-110">Permission type</span></span>                        | <span data-ttu-id="53b4a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="53b4a-111">Permissions (from least to most privileged)</span></span>                                             |
|:---------------------------------------|:----------------------------------------------------------------------------------------|
| <span data-ttu-id="53b4a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53b4a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="53b4a-113">不支持</span><span class="sxs-lookup"><span data-stu-id="53b4a-113">Not Supported</span></span>                                                                           |
| <span data-ttu-id="53b4a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53b4a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53b4a-115">不支持</span><span class="sxs-lookup"><span data-stu-id="53b4a-115">Not Supported</span></span>                                                                           |
| <span data-ttu-id="53b4a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="53b4a-116">Application</span></span>                            | <span data-ttu-id="53b4a-117">JoinGroupCallsasGuest、JoinGroupCalls、calls、InitiateGroupCalls、All、和。</span><span class="sxs-lookup"><span data-stu-id="53b4a-117">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All</span></span> |

> <span data-ttu-id="53b4a-118">**注意：** 对于包含应用托管媒体的呼叫，除了上表中列出的权限之一之外，还需要 AccessMedia 权限。</span><span class="sxs-lookup"><span data-stu-id="53b4a-118">**Note:** For a call with app-hosted media, you need the Calls.AccessMedia.All permission in addition to one of the permissions listed in the table above.</span></span>

## <a name="http-request"></a><span data-ttu-id="53b4a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53b4a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls
```

## <a name="request-headers"></a><span data-ttu-id="53b4a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="53b4a-120">Request headers</span></span>
| <span data-ttu-id="53b4a-121">名称</span><span class="sxs-lookup"><span data-stu-id="53b4a-121">Name</span></span>          | <span data-ttu-id="53b4a-122">说明</span><span class="sxs-lookup"><span data-stu-id="53b4a-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="53b4a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="53b4a-123">Authorization</span></span> | <span data-ttu-id="53b4a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="53b4a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="53b4a-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="53b4a-126">Content-type</span></span>  | <span data-ttu-id="53b4a-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="53b4a-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="53b4a-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="53b4a-129">Request body</span></span>
<span data-ttu-id="53b4a-130">在请求正文中，提供[call](../resources/call.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53b4a-130">In the request body, supply a JSON representation of a [call](../resources/call.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="53b4a-131">响应</span><span class="sxs-lookup"><span data-stu-id="53b4a-131">Response</span></span>
<span data-ttu-id="53b4a-132">如果成功，此方法在响应`201 Created`正文中返回响应代码和[call](../resources/call.md)对象。</span><span class="sxs-lookup"><span data-stu-id="53b4a-132">If successful, this method returns a `201 Created` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="53b4a-133">示例</span><span class="sxs-lookup"><span data-stu-id="53b4a-133">Examples</span></span>

### <a name="example-1-create-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="53b4a-134">示例1：使用服务托管媒体创建对等 VoIP 呼叫</span><span class="sxs-lookup"><span data-stu-id="53b4a-134">Example 1: Create peer-to-peer VoIP call with service hosted media</span></span>

> <span data-ttu-id="53b4a-135">**注意：** 此调用需要调用. Initiate。 All 权限。</span><span class="sxs-lookup"><span data-stu-id="53b4a-135">**Note:** This call needs the Calls.Initiate.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="53b4a-136">请求</span><span class="sxs-lookup"><span data-stu-id="53b4a-136">Request</span></span>
<span data-ttu-id="53b4a-137">以下示例显示了在 bot 和指定用户之间进行对等呼叫的请求。</span><span class="sxs-lookup"><span data-stu-id="53b4a-137">The following example shows the request which makes a peer-to-peer call between the bot and the specified user.</span></span> <span data-ttu-id="53b4a-138">在此示例中，媒体由服务托管。</span><span class="sxs-lookup"><span data-stu-id="53b4a-138">In this example, the media is hosted by the service.</span></span> <span data-ttu-id="53b4a-139">必须使用实际值替换授权令牌、回调 URL、应用程序 ID、应用程序名称、用户 ID、用户名和租户 ID 的值，以使示例正常工作。</span><span class="sxs-lookup"><span data-stu-id="53b4a-139">The values of authorization token, callback URL, application ID, application name, user ID, user name, and tenant ID must be replaced with actual values to make the example work.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="53b4a-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="53b4a-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-call-service-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls
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
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
  }
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="53b4a-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53b4a-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-call-service-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="53b4a-142">C#</span><span class="sxs-lookup"><span data-stu-id="53b4a-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-call-service-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="53b4a-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53b4a-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-call-service-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="53b4a-144">Java</span><span class="sxs-lookup"><span data-stu-id="53b4a-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-call-service-hosted-media-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="53b4a-145">响应</span><span class="sxs-lookup"><span data-stu-id="53b4a-145">Response</span></span>

> <span data-ttu-id="53b4a-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="53b4a-146">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "state": "establishing",
  "direction": "outgoing",
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
      "replacesCallId": null,
    }
  ],
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
  "myParticipantId": "499ff390-7a72-40e8-83a0-8fac6295ae7e",
  "id": "2e1a0b00-2db4-4022-9570-243709c565ab",
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#app/calls/$entity",
  "subject": null,
  "ringingTimeoutInSeconds": null,
  "mediaState": null,
  "resultInfo": null,
  "answeredBy": null,
  "chatInfo": null,
  "meetingInfo": null,
  "toneInfo": null
}
```

##### <a name="notification---establishing"></a><span data-ttu-id="53b4a-147">通知-建立</span><span class="sxs-lookup"><span data-stu-id="53b4a-147">Notification - establishing</span></span>

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
##### <a name="notification---established"></a><span data-ttu-id="53b4a-148">已建立通知</span><span class="sxs-lookup"><span data-stu-id="53b4a-148">Notification - established</span></span>

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
        "id": "2e1a0b00-b3c5-4b0f-99b3-c133bc1e6116"
      }
    }
  ]
}
```

### <a name="example-2-create-peer-to-peer-voip-call-with-application-hosted-media"></a><span data-ttu-id="53b4a-149">示例2：使用应用程序托管媒体创建对等 VoIP 呼叫</span><span class="sxs-lookup"><span data-stu-id="53b4a-149">Example 2: Create peer-to-peer VoIP call with application hosted media</span></span>

> <span data-ttu-id="53b4a-150">**注意**：此示例需要调用 AccessMedia 所有权限。</span><span class="sxs-lookup"><span data-stu-id="53b4a-150">**Note**: This example needs Calls.Initiate.All and Calls.AccessMedia.All permissions.</span></span>

##### <a name="request"></a><span data-ttu-id="53b4a-151">请求</span><span class="sxs-lookup"><span data-stu-id="53b4a-151">Request</span></span>
<span data-ttu-id="53b4a-152">以下示例显示了在 bot 和指定用户之间进行对等呼叫的请求。</span><span class="sxs-lookup"><span data-stu-id="53b4a-152">The following example shows the request which makes a peer-to-peer call between the bot and the specified user.</span></span> <span data-ttu-id="53b4a-153">在此示例中，媒体由应用程序本地承载。</span><span class="sxs-lookup"><span data-stu-id="53b4a-153">In this example the media is hosted locally by the application.</span></span> <span data-ttu-id="53b4a-154">必须使用实际值替换授权令牌、回调 url、应用程序 id、应用程序名称、用户 id、用户名和租户 id 的值，以使示例正常工作。</span><span class="sxs-lookup"><span data-stu-id="53b4a-154">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced with actual values to make the example work.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="53b4a-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="53b4a-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-call-app-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="53b4a-156">C#</span><span class="sxs-lookup"><span data-stu-id="53b4a-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-call-app-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="53b4a-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53b4a-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-call-app-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="53b4a-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53b4a-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-call-app-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="53b4a-159">Java</span><span class="sxs-lookup"><span data-stu-id="53b4a-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-call-app-hosted-media-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

><span data-ttu-id="53b4a-160">**注意：** 对于点对点呼叫，预期的通知仅适用于呼叫状态更改。</span><span class="sxs-lookup"><span data-stu-id="53b4a-160">**Note:** For peer-to-peer calls, the expected notifications are for call state changes only.</span></span>

##### <a name="response"></a><span data-ttu-id="53b4a-161">响应</span><span class="sxs-lookup"><span data-stu-id="53b4a-161">Response</span></span>

> <span data-ttu-id="53b4a-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="53b4a-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "state": "establishing",
  "direction": "outgoing",
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
    "blob": "<Media Session Configuration>",
  },
  "myParticipantId": "499ff390-7a72-40e8-83a0-8fac6295ae7e",
  "id": "2e1a0b00-2db4-4022-9570-243709c565ab",
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#app/calls/$entity",
  "subject": null,
  "ringingTimeoutInSeconds": null,
  "mediaState": null,
  "resultInfo": null,
  "answeredBy": null,
  "chatInfo": null,
  "meetingInfo": null,
  "toneInfo": null
}
```

### <a name="example-3-create-a-group-call-with-service-hosted-media"></a><span data-ttu-id="53b4a-164">示例3：使用服务托管媒体创建组呼叫</span><span class="sxs-lookup"><span data-stu-id="53b4a-164">Example 3: Create a group call with service hosted media</span></span>

<span data-ttu-id="53b4a-165">这最高支持5个 VoIP 用户。</span><span class="sxs-lookup"><span data-stu-id="53b4a-165">This supports up to 5 VoIP users.</span></span> <span data-ttu-id="53b4a-166">此示例演示如何使用两个 VoIP 用户创建组呼叫。</span><span class="sxs-lookup"><span data-stu-id="53b4a-166">The example shows how to create a group call with two VoIP users.</span></span>
> <span data-ttu-id="53b4a-167">**注意：** 此示例调用需要该`Calls.InitiateGroupCalls.All`权限。</span><span class="sxs-lookup"><span data-stu-id="53b4a-167">**Note:** This example call needs the `Calls.InitiateGroupCalls.All` permission.</span></span> <span data-ttu-id="53b4a-168">创建的组呼叫不支持聊天或录制。</span><span class="sxs-lookup"><span data-stu-id="53b4a-168">The group call created doesn't support chat or recording.</span></span>

##### <a name="request"></a><span data-ttu-id="53b4a-169">请求</span><span class="sxs-lookup"><span data-stu-id="53b4a-169">Request</span></span>

<!-- {
  "blockType": "example",
  "name": "create-group-call-service-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->

```http
POST https://graph.microsoft.com/v1.0/communications/calls
Content-Type: application/json

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
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
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
  }
}
```

### <a name="example-4-create-a-group-call-with-application-hosted-media"></a><span data-ttu-id="53b4a-170">示例4：使用应用程序托管媒体创建组调用</span><span class="sxs-lookup"><span data-stu-id="53b4a-170">Example 4: Create a group call with application hosted media</span></span>

<span data-ttu-id="53b4a-171">这最高支持5个 VoIP 用户。</span><span class="sxs-lookup"><span data-stu-id="53b4a-171">This supports up to 5 VoIP users.</span></span> <span data-ttu-id="53b4a-172">此示例演示如何使用两个 VoIP 用户创建组呼叫。</span><span class="sxs-lookup"><span data-stu-id="53b4a-172">The example shows how to create a group call with two VoIP users.</span></span>
> <span data-ttu-id="53b4a-173">**注意：** 此示例调用需要该`Calls.InitiateGroupCalls.All`权限。</span><span class="sxs-lookup"><span data-stu-id="53b4a-173">**Note:** This example call needs the `Calls.InitiateGroupCalls.All` permission.</span></span> <span data-ttu-id="53b4a-174">创建的组呼叫不支持聊天或录制。</span><span class="sxs-lookup"><span data-stu-id="53b4a-174">The group call created doesn't support chat or recording.</span></span>

##### <a name="request"></a><span data-ttu-id="53b4a-175">请求</span><span class="sxs-lookup"><span data-stu-id="53b4a-175">Request</span></span>

<!-- {
  "blockType": "example",
  "name": "create-group-call-app-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->

```http
POST https://graph.microsoft.com/v1.0/communications/calls
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "direction": "outgoing",
  "subject": "Create a group call with application hosted media",
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
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
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
    "removeFromDefaultAudioGroup": false
  }
}
```

### <a name="example-5-join-scheduled-meeting-with-service-hosted-media"></a><span data-ttu-id="53b4a-176">示例5：加入服务托管媒体的计划会议</span><span class="sxs-lookup"><span data-stu-id="53b4a-176">Example 5: Join scheduled meeting with service hosted media</span></span>
<span data-ttu-id="53b4a-177">若要加入计划的会议，我们需要获取线程 id、邮件 id、组织者 id 以及在其中安排会议的租户 id。</span><span class="sxs-lookup"><span data-stu-id="53b4a-177">To join the scheduled meeting we will need to get the thread id, message id, organizer id and the tenant id in which the meeting is scheduled.</span></span>
<span data-ttu-id="53b4a-178">此信息可从[Get Online 会议 API](../api/onlinemeeting-get.md) （仅限基于 VTC 的会议）获取。</span><span class="sxs-lookup"><span data-stu-id="53b4a-178">This information can be obtained from the [Get Online Meetings API](../api/onlinemeeting-get.md) (VTC-based meetings only).</span></span>

<span data-ttu-id="53b4a-179">必须将授权令牌、回调 url、应用程序 id、应用程序名称、用户 id、用户名和租户 id 的值替换为使用实际值[获取联机会议 API](../api/onlinemeeting-get.md) （仅限 VTC 会议）获取的详细信息，以使示例工作。</span><span class="sxs-lookup"><span data-stu-id="53b4a-179">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced along with the details obtained from  [Get Online Meetings API](../api/onlinemeeting-get.md) (VTC-based meetings only) with actual values to make the example work.</span></span>
> <span data-ttu-id="53b4a-180">**注意：** 此示例需要该`Calls.JoinGroupCalls.All`权限。</span><span class="sxs-lookup"><span data-stu-id="53b4a-180">**Note:** This example needs the `Calls.JoinGroupCalls.All` permission.</span></span>

##### <a name="request"></a><span data-ttu-id="53b4a-181">请求</span><span class="sxs-lookup"><span data-stu-id="53b4a-181">Request</span></span>

<!-- {
  "blockType": "example",
  "name": "join-scheduled-meeting-service-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls
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
        "displayName": "Bob"
      }
    },
    "allowConversationWithoutHost": true
  }
}
```
##### <a name="response"></a><span data-ttu-id="53b4a-182">响应</span><span class="sxs-lookup"><span data-stu-id="53b4a-182">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": "true",
  "@odata.type": "microsoft.graph.call"
}-->
```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/communications/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "state": "establishing",
  "direction": "outgoing",
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
  "targets": [],
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
        "displayName": "Bob"
      }
    },
    "allowConversationWithoutHost": true
  },
  "myParticipantId": "05491616-385f-44a8-9974-18cc5f9933c1",
  "id": "2f1a1100-b174-40a0-aba7-0b405e01ed92",
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#app/calls/$entity",
  "ringingTimeoutInSeconds": null,
  "mediaState": null,
  "subject": null,
  "resultInfo": null,
  "answeredBy": null,
  "toneInfo": null
}
```

##### <a name="notification---establishing"></a><span data-ttu-id="53b4a-183">通知-建立</span><span class="sxs-lookup"><span data-stu-id="53b4a-183">Notification - establishing</span></span>

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
##### <a name="notification---established"></a><span data-ttu-id="53b4a-184">已建立通知</span><span class="sxs-lookup"><span data-stu-id="53b4a-184">Notification - established</span></span>

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
##### <a name="notification---roster"></a><span data-ttu-id="53b4a-185">通知-名单</span><span class="sxs-lookup"><span data-stu-id="53b4a-185">Notification - roster</span></span>

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

><span data-ttu-id="53b4a-186">**注意：** 除了呼叫状态通知之外，对于加入会议方案，我们会收到名单通知。</span><span class="sxs-lookup"><span data-stu-id="53b4a-186">**Note:** For join meeting scenarios apart from call state notifications, we receive roster notifications.</span></span>

### <a name="example-6-join-scheduled-meeting-with-application-hosted-media"></a><span data-ttu-id="53b4a-187">示例6：加入使用应用程序托管媒体的计划会议</span><span class="sxs-lookup"><span data-stu-id="53b4a-187">Example 6: Join scheduled meeting with application hosted media</span></span>
<span data-ttu-id="53b4a-188">按如下所示更新[AppHostedMediaConfig](../resources/apphostedmediaconfig.md)的媒体配置。</span><span class="sxs-lookup"><span data-stu-id="53b4a-188">Update the media config with the [AppHostedMediaConfig](../resources/apphostedmediaconfig.md) as shown below.</span></span>

<!-- {
  "blockType": "example",
  "name": "join-scheduled-meeting-app-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig"
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
        "displayName": "Bob"
      }
    },
    "allowConversationWithoutHost": true
  }
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
