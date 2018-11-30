---
title: 呼叫： 答案
description: 应答传入呼叫。
ms.openlocfilehash: d2cf1030179d8822fd4620224addbabb95c5482f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042024"
---
# <a name="call-answer"></a><span data-ttu-id="6cead-103">呼叫： 答案</span><span class="sxs-lookup"><span data-stu-id="6cead-103">call: answer</span></span>

> <span data-ttu-id="6cead-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6cead-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6cead-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6cead-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6cead-106">应答传入呼叫。</span><span class="sxs-lookup"><span data-stu-id="6cead-106">Answer an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="6cead-107">权限</span><span class="sxs-lookup"><span data-stu-id="6cead-107">Permissions</span></span>
<span data-ttu-id="6cead-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6cead-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6cead-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6cead-110">Permission type</span></span> | <span data-ttu-id="6cead-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6cead-111">Permissions (from least to most privileged)</span></span>                 |
| :-------------- | :-----------------------------------------------------------|
| <span data-ttu-id="6cead-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6cead-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6cead-113">不支持</span><span class="sxs-lookup"><span data-stu-id="6cead-113">Not Supported</span></span>                        |
| <span data-ttu-id="6cead-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6cead-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6cead-115">不支持</span><span class="sxs-lookup"><span data-stu-id="6cead-115">Not Supported</span></span>                        |
| <span data-ttu-id="6cead-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6cead-116">Application</span></span>     | <span data-ttu-id="6cead-117">无</span><span class="sxs-lookup"><span data-stu-id="6cead-117">None</span></span>                                                        |

## <a name="http-request"></a><span data-ttu-id="6cead-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6cead-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/answer
POST /applications/{id}/calls/{id}/answer
```

## <a name="request-headers"></a><span data-ttu-id="6cead-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6cead-119">Request headers</span></span>
| <span data-ttu-id="6cead-120">名称</span><span class="sxs-lookup"><span data-stu-id="6cead-120">Name</span></span>          | <span data-ttu-id="6cead-121">说明</span><span class="sxs-lookup"><span data-stu-id="6cead-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="6cead-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cead-122">Authorization</span></span> | <span data-ttu-id="6cead-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6cead-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6cead-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="6cead-125">Request body</span></span>
<span data-ttu-id="6cead-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="6cead-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6cead-127">参数</span><span class="sxs-lookup"><span data-stu-id="6cead-127">Parameter</span></span>        | <span data-ttu-id="6cead-128">类型</span><span class="sxs-lookup"><span data-stu-id="6cead-128">Type</span></span>                                     |<span data-ttu-id="6cead-129">说明</span><span class="sxs-lookup"><span data-stu-id="6cead-129">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="6cead-130">callbackUri</span><span class="sxs-lookup"><span data-stu-id="6cead-130">callbackUri</span></span>       |<span data-ttu-id="6cead-131">字符串</span><span class="sxs-lookup"><span data-stu-id="6cead-131">String</span></span>                                    |<span data-ttu-id="6cead-132">将在其传递回调回调或订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="6cead-132">The callback or subscription ID on which callbacks will be delivered.</span></span> <span data-ttu-id="6cead-133">（必需）</span><span class="sxs-lookup"><span data-stu-id="6cead-133">(Required)</span></span>                                                               |
|<span data-ttu-id="6cead-134">acceptedModalities</span><span class="sxs-lookup"><span data-stu-id="6cead-134">acceptedModalities</span></span>|<span data-ttu-id="6cead-135">String 集合</span><span class="sxs-lookup"><span data-stu-id="6cead-135">String collection</span></span>                         |<span data-ttu-id="6cead-136">列表接受形式。</span><span class="sxs-lookup"><span data-stu-id="6cead-136">The list of accept modalities.</span></span> <span data-ttu-id="6cead-137">可能的值是： `unknown`， `audio`， `video`， `screenSharing`， `videoBasedScreenSharing`， `data`。</span><span class="sxs-lookup"><span data-stu-id="6cead-137">Possible value are: `unknown`, `audio`, `video`, `screenSharing`, `videoBasedScreenSharing`, `data`.</span></span> <span data-ttu-id="6cead-138">（必需）</span><span class="sxs-lookup"><span data-stu-id="6cead-138">(Required)</span></span> |
|<span data-ttu-id="6cead-139">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="6cead-139">mediaConfig</span></span>       |[<span data-ttu-id="6cead-140">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="6cead-140">mediaConfig</span></span>](../resources/mediaconfig.md)|<span data-ttu-id="6cead-141">媒体配置。</span><span class="sxs-lookup"><span data-stu-id="6cead-141">The media configuration.</span></span> <span data-ttu-id="6cead-142">（必需）</span><span class="sxs-lookup"><span data-stu-id="6cead-142">(Required)</span></span>                                                                                                            |

## <a name="response"></a><span data-ttu-id="6cead-143">响应</span><span class="sxs-lookup"><span data-stu-id="6cead-143">Response</span></span>
<span data-ttu-id="6cead-144">此方法返回`202 Accepted`响应代码。</span><span class="sxs-lookup"><span data-stu-id="6cead-144">This method returns `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6cead-145">示例</span><span class="sxs-lookup"><span data-stu-id="6cead-145">Examples</span></span>
<span data-ttu-id="6cead-146">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="6cead-146">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="6cead-147">请求</span><span class="sxs-lookup"><span data-stu-id="6cead-147">Request</span></span>
<span data-ttu-id="6cead-148">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="6cead-148">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call_answer"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/answer
Content-Type: application/json
Content-Length: 211

{
  "callbackUri": "callbackUri-value",
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<media config blob>"
  },
  "acceptedModalities": [
    "audio"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="6cead-149">响应</span><span class="sxs-lookup"><span data-stu-id="6cead-149">Response</span></span>
<span data-ttu-id="6cead-150">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6cead-150">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="answer-voip-call-with-service-hosted-media"></a><span data-ttu-id="6cead-151">服务承载媒体与 VOIP 呼叫应答</span><span class="sxs-lookup"><span data-stu-id="6cead-151">Answer VOIP call with service hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="6cead-152">通知-传入</span><span class="sxs-lookup"><span data-stu-id="6cead-152">Notification - incoming</span></span>

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
      "changeType": "created",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
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

##### <a name="request"></a><span data-ttu-id="6cead-153">请求</span><span class="sxs-lookup"><span data-stu-id="6cead-153">Request</span></span>

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/answer
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "ignored",
  "name": "call_answer"
}-->
```json
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

##### <a name="response"></a><span data-ttu-id="6cead-154">响应</span><span class="sxs-lookup"><span data-stu-id="6cead-154">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="6cead-155">通知-建立</span><span class="sxs-lookup"><span data-stu-id="6cead-155">Notification - establishing</span></span>

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
        "state": "establishing"
      }
    }
  ]
}
```

##### <a name="notification---established"></a><span data-ttu-id="6cead-156">通知-建立</span><span class="sxs-lookup"><span data-stu-id="6cead-156">Notification - established</span></span>

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

### <a name="answer-voip-call-with-application-hosted-media"></a><span data-ttu-id="6cead-157">应答与承载的应用程序媒体的 VOIP 呼叫</span><span class="sxs-lookup"><span data-stu-id="6cead-157">Answer VOIP call with application hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="6cead-158">通知-传入</span><span class="sxs-lookup"><span data-stu-id="6cead-158">Notification - incoming</span></span>

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
      "changeType": "created",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
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

##### <a name="request"></a><span data-ttu-id="6cead-159">请求</span><span class="sxs-lookup"><span data-stu-id="6cead-159">Request</span></span>

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/answer
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "ignored",
  "name": "call_answer"
}-->
```json
{
  "callbackUri": "https://bot.contoso.com/api/calls",
  "acceptedModalities": [ "audio" ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<media config blob>"
  }
}
```

##### <a name="response"></a><span data-ttu-id="6cead-160">响应</span><span class="sxs-lookup"><span data-stu-id="6cead-160">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="6cead-161">通知-建立</span><span class="sxs-lookup"><span data-stu-id="6cead-161">Notification - establishing</span></span>

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
        "state": "establishing"
      }
    }
  ]
}
```

##### <a name="notification---established"></a><span data-ttu-id="6cead-162">通知-建立</span><span class="sxs-lookup"><span data-stu-id="6cead-162">Notification - established</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call: answer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
