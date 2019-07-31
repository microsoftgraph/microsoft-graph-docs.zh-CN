---
title: 创建调用
description: 创建新呼叫。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b645180c3f90f0d282aa70282ac362c8365e3f02
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945457"
---
# <a name="create-call"></a><span data-ttu-id="6591d-103">创建调用</span><span class="sxs-lookup"><span data-stu-id="6591d-103">Create call</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6591d-104">创建新呼叫。</span><span class="sxs-lookup"><span data-stu-id="6591d-104">Create a new call.</span></span>

## <a name="permissions"></a><span data-ttu-id="6591d-105">权限</span><span class="sxs-lookup"><span data-stu-id="6591d-105">Permissions</span></span>
<span data-ttu-id="6591d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6591d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6591d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6591d-108">Permission type</span></span>                        | <span data-ttu-id="6591d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6591d-109">Permissions (from least to most privileged)</span></span>                                             |
|:---------------------------------------|:----------------------------------------------------------------------------------------|
| <span data-ttu-id="6591d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6591d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6591d-111">不支持</span><span class="sxs-lookup"><span data-stu-id="6591d-111">Not Supported</span></span>                                                                           |
| <span data-ttu-id="6591d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6591d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6591d-113">不支持</span><span class="sxs-lookup"><span data-stu-id="6591d-113">Not Supported</span></span>                                                                           |
| <span data-ttu-id="6591d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6591d-114">Application</span></span>                            | <span data-ttu-id="6591d-115">JoinGroupCallsasGuest、JoinGroupCalls、calls、InitiateGroupCalls、All、和。</span><span class="sxs-lookup"><span data-stu-id="6591d-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All</span></span> |

> <span data-ttu-id="6591d-116">**注意:** 对于具有应用程序托管媒体的呼叫, 您需要 AccessMedia 具有上表中列出的权限之一的所有权限。</span><span class="sxs-lookup"><span data-stu-id="6591d-116">**Note:** For a call with app hosted media, you need the Calls.AccessMedia.All permission with one of the permissions listed in the previous table.</span></span>

## <a name="http-request"></a><span data-ttu-id="6591d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6591d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls
POST /applications/{id}/calls
```

## <a name="request-headers"></a><span data-ttu-id="6591d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6591d-118">Request headers</span></span>
| <span data-ttu-id="6591d-119">名称</span><span class="sxs-lookup"><span data-stu-id="6591d-119">Name</span></span>          | <span data-ttu-id="6591d-120">说明</span><span class="sxs-lookup"><span data-stu-id="6591d-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="6591d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6591d-121">Authorization</span></span> | <span data-ttu-id="6591d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6591d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6591d-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="6591d-124">Request body</span></span>
<span data-ttu-id="6591d-125">在请求正文中, 提供[call](../resources/call.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6591d-125">In the request body, supply a JSON representation of a [call](../resources/call.md) object.</span></span>

> <span data-ttu-id="6591d-126">**注意:** 在`Server generated` `app/calls`处理`POST`时, 被标记为的属性将被忽略。</span><span class="sxs-lookup"><span data-stu-id="6591d-126">**Note:** Properties marked as `Server generated` are ignored when processing `POST` on `app/calls`.</span></span>

## <a name="response"></a><span data-ttu-id="6591d-127">响应</span><span class="sxs-lookup"><span data-stu-id="6591d-127">Response</span></span>
<span data-ttu-id="6591d-128">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[call](../resources/call.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6591d-128">If successful, this method returns a `201 Created` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6591d-129">示例</span><span class="sxs-lookup"><span data-stu-id="6591d-129">Examples</span></span>

### <a name="create-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="6591d-130">使用服务托管媒体创建对等 VOIP 呼叫</span><span class="sxs-lookup"><span data-stu-id="6591d-130">Create peer to peer VOIP call with service hosted media</span></span>

> <span data-ttu-id="6591d-131">**注意:** 此调用需要调用. Initiate。 All 权限。</span><span class="sxs-lookup"><span data-stu-id="6591d-131">**Note:** This call needs the Calls.Initiate.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="6591d-132">请求</span><span class="sxs-lookup"><span data-stu-id="6591d-132">Request</span></span>
<span data-ttu-id="6591d-133">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="6591d-133">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6591d-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="6591d-134">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6591d-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="6591d-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-call-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6591d-136">响应</span><span class="sxs-lookup"><span data-stu-id="6591d-136">Response</span></span>

> <span data-ttu-id="6591d-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6591d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

##### <a name="notification---establishing"></a><span data-ttu-id="6591d-139">通知-建立</span><span class="sxs-lookup"><span data-stu-id="6591d-139">Notification - establishing</span></span>

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
##### <a name="notification---established"></a><span data-ttu-id="6591d-140">已建立通知</span><span class="sxs-lookup"><span data-stu-id="6591d-140">Notification - established</span></span>

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

### <a name="create-peer-to-peer-voip-call-with-application-hosted-media"></a><span data-ttu-id="6591d-141">使用应用程序托管媒体创建对等 VOIP 呼叫</span><span class="sxs-lookup"><span data-stu-id="6591d-141">Create peer to peer VOIP call with application hosted media</span></span>

> <span data-ttu-id="6591d-142">注意: 需要调用. Initiate. All 和 AccessMedia 权限。</span><span class="sxs-lookup"><span data-stu-id="6591d-142">Note: Needs Calls.Initiate.All and Calls.AccessMedia.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="6591d-143">请求</span><span class="sxs-lookup"><span data-stu-id="6591d-143">Request</span></span>
<span data-ttu-id="6591d-144">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="6591d-144">The following example shows the request.</span></span>

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

### <a name="create-group-call-with-service-hosted-media"></a><span data-ttu-id="6591d-145">使用服务托管媒体创建组呼叫</span><span class="sxs-lookup"><span data-stu-id="6591d-145">Create group call with service hosted media</span></span>

> <span data-ttu-id="6591d-146">**注意:** 此示例需要 InitiateGroupCalls 和 AccessMedia。所有权限。</span><span class="sxs-lookup"><span data-stu-id="6591d-146">**Note:** This example needs the Calls.InitiateGroupCalls.All and Calls.AccessMedia.All permissions.</span></span>

##### <a name="request"></a><span data-ttu-id="6591d-147">请求</span><span class="sxs-lookup"><span data-stu-id="6591d-147">Request</span></span>

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

### <a name="join-private-meeting-with-service-hosted-media"></a><span data-ttu-id="6591d-148">加入具有服务托管媒体的专用会议</span><span class="sxs-lookup"><span data-stu-id="6591d-148">Join private meeting with service hosted media</span></span>

> <span data-ttu-id="6591d-149">**注意:** 此示例需要 JoinGroupCalls 权限。</span><span class="sxs-lookup"><span data-stu-id="6591d-149">**Note:** This example needs the Calls.JoinGroupCalls.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="6591d-150">请求</span><span class="sxs-lookup"><span data-stu-id="6591d-150">Request</span></span>

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

### <a name="join-channel-meeting-with-service-hosted-media"></a><span data-ttu-id="6591d-151">加入使用服务托管媒体的渠道会议</span><span class="sxs-lookup"><span data-stu-id="6591d-151">Join channel meeting with service hosted media</span></span>

> <span data-ttu-id="6591d-152">**注意:** 此示例需要 JoinGroupCalls 权限。</span><span class="sxs-lookup"><span data-stu-id="6591d-152">**Note:** This example needs the Calls.JoinGroupCalls.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="6591d-153">请求</span><span class="sxs-lookup"><span data-stu-id="6591d-153">Request</span></span>

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

### <a name="join-channel-meeting-as-a-guest-with-service-hosted-media"></a><span data-ttu-id="6591d-154">以具有服务托管媒体的来宾身份加入频道会议</span><span class="sxs-lookup"><span data-stu-id="6591d-154">Join channel meeting as a guest with service hosted media</span></span>

> <span data-ttu-id="6591d-155">**注意:** 此示例需要 JoinGroupCallsAsGuest 权限。</span><span class="sxs-lookup"><span data-stu-id="6591d-155">**Note:** This example needs the Calls.JoinGroupCallsAsGuest.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="6591d-156">请求</span><span class="sxs-lookup"><span data-stu-id="6591d-156">Request</span></span>

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
