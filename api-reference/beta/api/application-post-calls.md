---
title: 创建呼叫
description: 创建新的呼叫。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 185c20bceb311f5b0c5ece0f70aaa5e3ffd15042
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952333"
---
# <a name="create-call"></a><span data-ttu-id="c82c5-103">创建呼叫</span><span class="sxs-lookup"><span data-stu-id="c82c5-103">Create call</span></span>

> <span data-ttu-id="c82c5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c82c5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c82c5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c82c5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c82c5-106">创建新的呼叫。</span><span class="sxs-lookup"><span data-stu-id="c82c5-106">Create a new call.</span></span>

## <a name="permissions"></a><span data-ttu-id="c82c5-107">权限</span><span class="sxs-lookup"><span data-stu-id="c82c5-107">Permissions</span></span>
<span data-ttu-id="c82c5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c82c5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c82c5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c82c5-110">Permission type</span></span>                        | <span data-ttu-id="c82c5-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c82c5-111">Permissions (from least to most privileged)</span></span>                                             |
|:---------------------------------------|:----------------------------------------------------------------------------------------|
| <span data-ttu-id="c82c5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c82c5-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c82c5-113">不支持</span><span class="sxs-lookup"><span data-stu-id="c82c5-113">Not Supported</span></span>                                                                           |
| <span data-ttu-id="c82c5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c82c5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c82c5-115">不支持</span><span class="sxs-lookup"><span data-stu-id="c82c5-115">Not Supported</span></span>                                                                           |
| <span data-ttu-id="c82c5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c82c5-116">Application</span></span>                            | <span data-ttu-id="c82c5-117">Calls.JoinGroupCallsasGuest.All，Calls.JoinGroupCalls.All，Calls.Initiate.All Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="c82c5-117">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All</span></span> |

> <span data-ttu-id="c82c5-118">**注意：** 与承载的应用程序媒体呼叫，您需要使用上表中列出的权限之一 Calls.AccessMedia.All 权限。</span><span class="sxs-lookup"><span data-stu-id="c82c5-118">**Note:** For a call with app hosted media, you need the Calls.AccessMedia.All permission with one of the permissions listed in the previous table.</span></span>

## <a name="http-request"></a><span data-ttu-id="c82c5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c82c5-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls
POST /applications/{id}/calls
```

## <a name="request-headers"></a><span data-ttu-id="c82c5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c82c5-120">Request headers</span></span>
| <span data-ttu-id="c82c5-121">名称</span><span class="sxs-lookup"><span data-stu-id="c82c5-121">Name</span></span>          | <span data-ttu-id="c82c5-122">说明</span><span class="sxs-lookup"><span data-stu-id="c82c5-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="c82c5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c82c5-123">Authorization</span></span> | <span data-ttu-id="c82c5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c82c5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c82c5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c82c5-126">Request body</span></span>
<span data-ttu-id="c82c5-127">在请求正文中，提供[呼叫](../resources/call.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c82c5-127">In the request body, supply a JSON representation of a [call](../resources/call.md) object.</span></span>

> <span data-ttu-id="c82c5-128">**注意：** 属性标记为`Server generated`处理时，将忽略`POST`上`app/calls`。</span><span class="sxs-lookup"><span data-stu-id="c82c5-128">**Note:** Properties marked as `Server generated` are ignored when processing `POST` on `app/calls`.</span></span>

## <a name="response"></a><span data-ttu-id="c82c5-129">响应</span><span class="sxs-lookup"><span data-stu-id="c82c5-129">Response</span></span>
<span data-ttu-id="c82c5-130">如果成功，此方法返回`201 Created`响应代码和响应正文中的[呼叫](../resources/call.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c82c5-130">If successful, this method returns a `201 Created` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c82c5-131">示例</span><span class="sxs-lookup"><span data-stu-id="c82c5-131">Examples</span></span>

### <a name="create-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="c82c5-132">创建与承载的服务媒体的对等 VOIP 呼叫</span><span class="sxs-lookup"><span data-stu-id="c82c5-132">Create peer to peer VOIP call with service hosted media</span></span>

> <span data-ttu-id="c82c5-133">**注意：** 此呼叫需要 Calls.Initiate.All 权限。</span><span class="sxs-lookup"><span data-stu-id="c82c5-133">**Note:** This call needs the Calls.Initiate.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="c82c5-134">请求</span><span class="sxs-lookup"><span data-stu-id="c82c5-134">Request</span></span>
<span data-ttu-id="c82c5-135">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="c82c5-135">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create-call-from-application"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json

{
  "callbackUri": "https://bot.contoso.com/api/calls",
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
  },
  "source": {
    "identity": {
      "application": {
        "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "subject": "Test Call",
  "targets": [
    {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      }
    }
  ],
  "tenantId": "tenantId-value"
}
```

##### <a name="response"></a><span data-ttu-id="c82c5-136">响应</span><span class="sxs-lookup"><span data-stu-id="c82c5-136">Response</span></span>

> <span data-ttu-id="c82c5-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c82c5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json


{
  "id": "57DAB8B1894C409AB240BD8BEAE78896",
  "callbackUri": "https://bot.contoso.com/api/calls",
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
  },
  "source": {
    "identity": {
      "application": {
        "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "subject": "Test Call",
  "targets": [
    {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      }
    }
  ],
  "tenantId": "tenantId-value"
}
```

##### <a name="notification---establishing"></a><span data-ttu-id="c82c5-139">通知-建立</span><span class="sxs-lookup"><span data-stu-id="c82c5-139">Notification - establishing</span></span>

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
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "state": "establishing",
        "direction": "outgoing"
      }
    }
  ]
}
```
##### <a name="notification---established"></a><span data-ttu-id="c82c5-140">通知-建立</span><span class="sxs-lookup"><span data-stu-id="c82c5-140">Notification - established</span></span>

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
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "established"
        }
    }
  ]
}
```

### <a name="create-peer-to-peer-voip-call-with-application-hosted-media"></a><span data-ttu-id="c82c5-141">创建与承载的应用程序媒体的对等 VOIP 呼叫</span><span class="sxs-lookup"><span data-stu-id="c82c5-141">Create peer to peer VOIP call with application hosted media</span></span>

> <span data-ttu-id="c82c5-142">注意： 需要 Calls.Initiate.All 和 Calls.AccessMedia.All 权限。</span><span class="sxs-lookup"><span data-stu-id="c82c5-142">Note: Needs Calls.Initiate.All and Calls.AccessMedia.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="c82c5-143">请求</span><span class="sxs-lookup"><span data-stu-id="c82c5-143">Request</span></span>
<span data-ttu-id="c82c5-144">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="c82c5-144">The following example shows the request.</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "callbackUri": "https://bot.contoso.com/api/calls",
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<media config blob>"
  },
  "requestedModalities": [ "audio" ],
  "source": {
    "identity": {
      "application": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "IT Bot"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "subject": "Test Call",
  "targets": [
    {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      }
    }
  ],
  "tenantId": "tenantId-value"
}
```

### <a name="create-group-call-with-service-hosted-media"></a><span data-ttu-id="c82c5-145">创建承载服务媒体组呼叫</span><span class="sxs-lookup"><span data-stu-id="c82c5-145">Create group call with service hosted media</span></span>

> <span data-ttu-id="c82c5-146">**注意：** 本示例需要 Calls.InitiateGroupCalls.All 和 Calls.AccessMedia.All 的权限。</span><span class="sxs-lookup"><span data-stu-id="c82c5-146">**Note:** This example needs the Calls.InitiateGroupCalls.All and Calls.AccessMedia.All permissions.</span></span>

##### <a name="request"></a><span data-ttu-id="c82c5-147">请求</span><span class="sxs-lookup"><span data-stu-id="c82c5-147">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "subject": "Test Call",
  "callbackUri": "https://bot.contoso.com/api/calls",
  "source": {
    "identity": {
      "application": {
        "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
      }
    }
  },
  "targets": [
    {
      "identity": {
        "user": {
          "id": "29362BD4-CD58-4ED0-A206-0E4A33DBB0B6",
          "displayName": "Heidi Steen"
        }
      }
    },
    {
      "identity": {
        "phone": {
          "displayName": "+12345678890",
          "id": "+12345678890"
        }
      }
    }
  ],
  "requestedModalities": [ "audio", "video" ],
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
  },
  "chatInfo": {
    "threadId": "19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2",
    "messageId": "0",
    "replyChainMessageId": null
  }
}
```

### <a name="join-private-meeting-with-service-hosted-media"></a><span data-ttu-id="c82c5-148">加入与服务的专用会议承载媒体</span><span class="sxs-lookup"><span data-stu-id="c82c5-148">Join private meeting with service hosted media</span></span>

> <span data-ttu-id="c82c5-149">**注意：** 本示例需要 Calls.JoinGroupCalls.All 权限。</span><span class="sxs-lookup"><span data-stu-id="c82c5-149">**Note:** This example needs the Calls.JoinGroupCalls.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="c82c5-150">请求</span><span class="sxs-lookup"><span data-stu-id="c82c5-150">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "subject": "Test Call",
  "callbackUri": "https://bot.contoso.com/api/calls",
  "source": {
    "identity": {
      "application": {
        "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
      }
    }
  },
  "requestedModalities": [ "audio", "video" ],
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
  },
  "chatInfo": {
    "threadId": "19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2",
    "messageId": "0"
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

### <a name="join-channel-meeting-with-service-hosted-media"></a><span data-ttu-id="c82c5-151">通道使用加入会议服务承载媒体</span><span class="sxs-lookup"><span data-stu-id="c82c5-151">Join channel meeting with service hosted media</span></span>

> <span data-ttu-id="c82c5-152">**注意：** 本示例需要 Calls.JoinGroupCalls.All 权限。</span><span class="sxs-lookup"><span data-stu-id="c82c5-152">**Note:** This example needs the Calls.JoinGroupCalls.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="c82c5-153">请求</span><span class="sxs-lookup"><span data-stu-id="c82c5-153">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "subject": "Test Call",
  "callbackUri": "https://bot.contoso.com/api/calls",
  "source": {
    "identity": {
      "application": {
        "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
      }
    }
  },
  "requestedModalities": [ "audio", "video" ],
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
  },
  "chatInfo": {
    "threadId": "19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2",
    "messageId": "1507228578052",
    "replyChainMessageId": null
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

### <a name="join-channel-meeting-as-a-guest-with-service-hosted-media"></a><span data-ttu-id="c82c5-154">以与承载的服务媒体来宾身份加入通道</span><span class="sxs-lookup"><span data-stu-id="c82c5-154">Join channel meeting as a guest with service hosted media</span></span>

> <span data-ttu-id="c82c5-155">**注意：** 本示例需要 Calls.JoinGroupCallsAsGuest.All 权限。</span><span class="sxs-lookup"><span data-stu-id="c82c5-155">**Note:** This example needs the Calls.JoinGroupCallsAsGuest.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="c82c5-156">请求</span><span class="sxs-lookup"><span data-stu-id="c82c5-156">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
```
<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "subject": "Test Call",
  "callbackUri": "https://bot.contoso.com/api/calls",
  "source": {
    "identity": {
      "user": {
        "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698",
        "displayName": "App_Guest_DisplayName",
        "identityProvider": "None"
      }
    }
  },
  "requestedModalities": [ "audio", "video" ],
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
  },
  "chatInfo": {
    "threadId": "19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2",
    "messageId": "1507228578052",
    "replyChainMessageId": null
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
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create call",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
