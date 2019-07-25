---
title: '呼叫: 应答'
description: 应答传入呼叫。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 6966c9804c5a3f7570f2decf6f35090130637786
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864945"
---
# <a name="call-answer"></a><span data-ttu-id="aa0b5-103">呼叫: 应答</span><span class="sxs-lookup"><span data-stu-id="aa0b5-103">call: answer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa0b5-104">应答传入呼叫。</span><span class="sxs-lookup"><span data-stu-id="aa0b5-104">Answer an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa0b5-105">权限</span><span class="sxs-lookup"><span data-stu-id="aa0b5-105">Permissions</span></span>
<span data-ttu-id="aa0b5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aa0b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aa0b5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="aa0b5-108">Permission type</span></span> | <span data-ttu-id="aa0b5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aa0b5-109">Permissions (from least to most privileged)</span></span>                 |
| :-------------- | :-----------------------------------------------------------|
| <span data-ttu-id="aa0b5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aa0b5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="aa0b5-111">不支持</span><span class="sxs-lookup"><span data-stu-id="aa0b5-111">Not Supported</span></span>                        |
| <span data-ttu-id="aa0b5-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aa0b5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa0b5-113">不支持</span><span class="sxs-lookup"><span data-stu-id="aa0b5-113">Not Supported</span></span>                        |
| <span data-ttu-id="aa0b5-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="aa0b5-114">Application</span></span>     | <span data-ttu-id="aa0b5-115">无</span><span class="sxs-lookup"><span data-stu-id="aa0b5-115">None</span></span>                                                        |

## <a name="http-request"></a><span data-ttu-id="aa0b5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aa0b5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/answer
POST /applications/{id}/calls/{id}/answer
```

## <a name="request-headers"></a><span data-ttu-id="aa0b5-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="aa0b5-117">Request headers</span></span>
| <span data-ttu-id="aa0b5-118">名称</span><span class="sxs-lookup"><span data-stu-id="aa0b5-118">Name</span></span>          | <span data-ttu-id="aa0b5-119">说明</span><span class="sxs-lookup"><span data-stu-id="aa0b5-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="aa0b5-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa0b5-120">Authorization</span></span> | <span data-ttu-id="aa0b5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aa0b5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa0b5-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="aa0b5-123">Request body</span></span>
<span data-ttu-id="aa0b5-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="aa0b5-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="aa0b5-125">参数</span><span class="sxs-lookup"><span data-stu-id="aa0b5-125">Parameter</span></span>        | <span data-ttu-id="aa0b5-126">类型</span><span class="sxs-lookup"><span data-stu-id="aa0b5-126">Type</span></span>                                     |<span data-ttu-id="aa0b5-127">说明</span><span class="sxs-lookup"><span data-stu-id="aa0b5-127">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="aa0b5-128">callbackUri</span><span class="sxs-lookup"><span data-stu-id="aa0b5-128">callbackUri</span></span>       |<span data-ttu-id="aa0b5-129">String</span><span class="sxs-lookup"><span data-stu-id="aa0b5-129">String</span></span>                                    |<span data-ttu-id="aa0b5-130">用于传递回拨的回拨或订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="aa0b5-130">The callback or subscription ID on which callbacks will be delivered.</span></span> <span data-ttu-id="aa0b5-131">需要</span><span class="sxs-lookup"><span data-stu-id="aa0b5-131">(Required)</span></span>                                                               |
|<span data-ttu-id="aa0b5-132">acceptedModalities</span><span class="sxs-lookup"><span data-stu-id="aa0b5-132">acceptedModalities</span></span>|<span data-ttu-id="aa0b5-133">String collection</span><span class="sxs-lookup"><span data-stu-id="aa0b5-133">String collection</span></span>                         |<span data-ttu-id="aa0b5-134">接受形式的列表。</span><span class="sxs-lookup"><span data-stu-id="aa0b5-134">The list of accept modalities.</span></span> <span data-ttu-id="aa0b5-135">可能的值为`unknown`: `audio`、 `video`、 `screenSharing`、 `videoBasedScreenSharing`、 `data`、。</span><span class="sxs-lookup"><span data-stu-id="aa0b5-135">Possible value are: `unknown`, `audio`, `video`, `screenSharing`, `videoBasedScreenSharing`, `data`.</span></span> <span data-ttu-id="aa0b5-136">需要</span><span class="sxs-lookup"><span data-stu-id="aa0b5-136">(Required)</span></span> |
|<span data-ttu-id="aa0b5-137">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="aa0b5-137">mediaConfig</span></span>       |[<span data-ttu-id="aa0b5-138">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="aa0b5-138">mediaConfig</span></span>](../resources/mediaconfig.md)|<span data-ttu-id="aa0b5-139">媒体配置。</span><span class="sxs-lookup"><span data-stu-id="aa0b5-139">The media configuration.</span></span> <span data-ttu-id="aa0b5-140">需要</span><span class="sxs-lookup"><span data-stu-id="aa0b5-140">(Required)</span></span>                                                                                                            |

## <a name="response"></a><span data-ttu-id="aa0b5-141">响应</span><span class="sxs-lookup"><span data-stu-id="aa0b5-141">Response</span></span>
<span data-ttu-id="aa0b5-142">此方法返回`202 Accepted`响应代码。</span><span class="sxs-lookup"><span data-stu-id="aa0b5-142">This method returns `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="aa0b5-143">示例</span><span class="sxs-lookup"><span data-stu-id="aa0b5-143">Examples</span></span>
<span data-ttu-id="aa0b5-144">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="aa0b5-144">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="aa0b5-145">请求</span><span class="sxs-lookup"><span data-stu-id="aa0b5-145">Request</span></span>
<span data-ttu-id="aa0b5-146">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="aa0b5-146">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="aa0b5-147">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="aa0b5-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-answer"
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="aa0b5-148">C#</span><span class="sxs-lookup"><span data-stu-id="aa0b5-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aa0b5-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="aa0b5-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="aa0b5-150">目标-C</span><span class="sxs-lookup"><span data-stu-id="aa0b5-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="aa0b5-151">Java</span><span class="sxs-lookup"><span data-stu-id="aa0b5-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-answer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="aa0b5-152">响应</span><span class="sxs-lookup"><span data-stu-id="aa0b5-152">Response</span></span>
<span data-ttu-id="aa0b5-153">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="aa0b5-153">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="answer-voip-call-with-service-hosted-media"></a><span data-ttu-id="aa0b5-154">使用服务托管媒体应答 VOIP 呼叫</span><span class="sxs-lookup"><span data-stu-id="aa0b5-154">Answer VOIP call with service hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="aa0b5-155">通知传入</span><span class="sxs-lookup"><span data-stu-id="aa0b5-155">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="aa0b5-156">请求</span><span class="sxs-lookup"><span data-stu-id="aa0b5-156">Request</span></span>

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/answer
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "ignored",
  "name": "call-answer"
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

##### <a name="response"></a><span data-ttu-id="aa0b5-157">响应</span><span class="sxs-lookup"><span data-stu-id="aa0b5-157">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="aa0b5-158">通知-建立</span><span class="sxs-lookup"><span data-stu-id="aa0b5-158">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="aa0b5-159">已建立通知</span><span class="sxs-lookup"><span data-stu-id="aa0b5-159">Notification - established</span></span>

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

### <a name="answer-voip-call-with-application-hosted-media"></a><span data-ttu-id="aa0b5-160">使用应用程序托管媒体应答 VOIP 呼叫</span><span class="sxs-lookup"><span data-stu-id="aa0b5-160">Answer VOIP call with application hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="aa0b5-161">通知传入</span><span class="sxs-lookup"><span data-stu-id="aa0b5-161">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="aa0b5-162">请求</span><span class="sxs-lookup"><span data-stu-id="aa0b5-162">Request</span></span>

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/answer
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "ignored",
  "name": "call-answer"
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

##### <a name="response"></a><span data-ttu-id="aa0b5-163">响应</span><span class="sxs-lookup"><span data-stu-id="aa0b5-163">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="aa0b5-164">通知-建立</span><span class="sxs-lookup"><span data-stu-id="aa0b5-164">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="aa0b5-165">已建立通知</span><span class="sxs-lookup"><span data-stu-id="aa0b5-165">Notification - established</span></span>

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
