---
title: 呼叫：重定向
description: 重定向传入呼叫。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: aac03c9f27d6d9d62d4781d16487538fc212be56
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073374"
---
# <a name="call-redirect"></a><span data-ttu-id="795a5-103">呼叫：重定向</span><span class="sxs-lookup"><span data-stu-id="795a5-103">call: redirect</span></span>

<span data-ttu-id="795a5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="795a5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="795a5-105">重定向尚未 [应答](./call-answer.md) 或 [拒绝](./call-reject.md) 的传入呼叫。</span><span class="sxs-lookup"><span data-stu-id="795a5-105">Redirect an incoming call that hasn't been [answered](./call-answer.md) or [rejected](./call-reject.md) yet.</span></span> <span data-ttu-id="795a5-106">术语 "重定向" 和 "转发" 可交换使用呼叫。</span><span class="sxs-lookup"><span data-stu-id="795a5-106">The terms "redirecting" and "forwarding" a call are used interchangeably.</span></span>

<span data-ttu-id="795a5-107">在呼叫超时之前，机器人应重定向呼叫。当前超时值为15秒。</span><span class="sxs-lookup"><span data-stu-id="795a5-107">The bot is expected to redirect the call before the call times out. The current timeout value is 15 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="795a5-108">权限</span><span class="sxs-lookup"><span data-stu-id="795a5-108">Permissions</span></span>

<span data-ttu-id="795a5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="795a5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="795a5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="795a5-111">Permission type</span></span> | <span data-ttu-id="795a5-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="795a5-112">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="795a5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="795a5-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="795a5-114">不支持</span><span class="sxs-lookup"><span data-stu-id="795a5-114">Not Supported</span></span>                |
| <span data-ttu-id="795a5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="795a5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="795a5-116">不支持</span><span class="sxs-lookup"><span data-stu-id="795a5-116">Not Supported</span></span>                |
| <span data-ttu-id="795a5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="795a5-117">Application</span></span>     | <span data-ttu-id="795a5-118">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="795a5-118">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="795a5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="795a5-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /communications/calls/{id}/redirect
```

## <a name="request-headers"></a><span data-ttu-id="795a5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="795a5-120">Request headers</span></span>

| <span data-ttu-id="795a5-121">名称</span><span class="sxs-lookup"><span data-stu-id="795a5-121">Name</span></span>          | <span data-ttu-id="795a5-122">说明</span><span class="sxs-lookup"><span data-stu-id="795a5-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="795a5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="795a5-123">Authorization</span></span> | <span data-ttu-id="795a5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="795a5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="795a5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="795a5-126">Request body</span></span>

<span data-ttu-id="795a5-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="795a5-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="795a5-128">参数</span><span class="sxs-lookup"><span data-stu-id="795a5-128">Parameter</span></span>      | <span data-ttu-id="795a5-129">类型</span><span class="sxs-lookup"><span data-stu-id="795a5-129">Type</span></span>    |<span data-ttu-id="795a5-130">说明</span><span class="sxs-lookup"><span data-stu-id="795a5-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="795a5-131">targets</span><span class="sxs-lookup"><span data-stu-id="795a5-131">targets</span></span>|<span data-ttu-id="795a5-132">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="795a5-132">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>|<span data-ttu-id="795a5-133">重定向操作的目标参与者。</span><span class="sxs-lookup"><span data-stu-id="795a5-133">The target participants of the redirect operation.</span></span> <span data-ttu-id="795a5-134">如果指定了多个目标，则为同时调用。</span><span class="sxs-lookup"><span data-stu-id="795a5-134">If more than one target is specified, it's a simulring call.</span></span> <span data-ttu-id="795a5-135">这意味着将同时 rang 所有目标，并且只会连接所选取的第一个目标。</span><span class="sxs-lookup"><span data-stu-id="795a5-135">This means that all of the targets will be rang at the same time and only the first target that picks up will be connected.</span></span> <span data-ttu-id="795a5-136">对于同时，我们最高支持25个目标。</span><span class="sxs-lookup"><span data-stu-id="795a5-136">We support up to 25 targets for simulring.</span></span>
|<span data-ttu-id="795a5-137">timeout</span><span class="sxs-lookup"><span data-stu-id="795a5-137">timeout</span></span>|<span data-ttu-id="795a5-138">Int32</span><span class="sxs-lookup"><span data-stu-id="795a5-138">Int32</span></span>|<span data-ttu-id="795a5-139">用于重定向操作) 的超时 (（秒）。</span><span class="sxs-lookup"><span data-stu-id="795a5-139">The timeout (in seconds) for the redirect operation.</span></span> <span data-ttu-id="795a5-140">超时值的范围介于15和90秒之间（含这两个值）。</span><span class="sxs-lookup"><span data-stu-id="795a5-140">The range of the timeout value is between 15 and 90 seconds inclusive.</span></span> <span data-ttu-id="795a5-141">对于多个目标，默认超时值为每个目标为60秒的一个目标，默认值为55秒 (主题将) 。</span><span class="sxs-lookup"><span data-stu-id="795a5-141">The default timeout value is 55 seconds for one target and 60 seconds for multiple targets (subject to change).</span></span> |
|<span data-ttu-id="795a5-142">callbackUri</span><span class="sxs-lookup"><span data-stu-id="795a5-142">callbackUri</span></span>|<span data-ttu-id="795a5-143">String</span><span class="sxs-lookup"><span data-stu-id="795a5-143">String</span></span>|<span data-ttu-id="795a5-144">这将允许 bot 为当前呼叫提供特定的回调 URI，以接收后续通知。</span><span class="sxs-lookup"><span data-stu-id="795a5-144">This allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="795a5-145">如果尚未设置此属性，则将改为使用 bot 的全局回调 URI。</span><span class="sxs-lookup"><span data-stu-id="795a5-145">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="795a5-146">这必须是 `https` 。</span><span class="sxs-lookup"><span data-stu-id="795a5-146">This must be `https`.</span></span>|

## <a name="response"></a><span data-ttu-id="795a5-147">响应</span><span class="sxs-lookup"><span data-stu-id="795a5-147">Response</span></span>
<span data-ttu-id="795a5-148">如果成功，此方法返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="795a5-148">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="795a5-149">示例</span><span class="sxs-lookup"><span data-stu-id="795a5-149">Examples</span></span>
<span data-ttu-id="795a5-150">这些示例将涵盖传入呼叫通知的工作流以及该呼叫将如何重定向。</span><span class="sxs-lookup"><span data-stu-id="795a5-150">These examples will cover a workflow of an incoming call notification and how that call will be redirected.</span></span>

> <span data-ttu-id="795a5-151">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="795a5-151">**Note:** The response objects shown here might be shortened for readability.</span></span> <span data-ttu-id="795a5-152">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="795a5-152">All the properties will be returned from an actual call.</span></span>

### <a name="example-1-forward-a-call-to-a-target"></a><span data-ttu-id="795a5-153">示例1：将呼叫转接到目标</span><span class="sxs-lookup"><span data-stu-id="795a5-153">Example 1: Forward a Call to a Target</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="795a5-154">通知传入</span><span class="sxs-lookup"><span data-stu-id="795a5-154">Notification - incoming</span></span>
<!-- {
  "blockType": "example", 
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "created",
      "resourceUrl": "/communications/calls/491f0b00-ffff-4bc9-a43e-b226498ec22a",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "incoming",
        "direction": "incoming",
        "callbackUri": "https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039",
        "source": {
          "@odata.type": "#microsoft.graph.participantInfo",
          "identity": {
            "@odata.type": "#microsoft.graph.identitySet",
            "user": {
              "@odata.type": "#microsoft.graph.identity",
              "id": "8d1e6ab6-26c5-4e22-a1bc-06ea7343958e"
            }
          },
          "region": "amer",
        },
        "targets": [
          {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "application": {
                "@odata.type": "#microsoft.graph.identity",
                "displayName": "test bot",
                "id": "24701998-1a73-4d42-8085-bf46ed0ae039"
              }
            }
          }
        ],
        "myParticipantId": "c339cede-4bd6-4f20-ab9f-3a13e65f6d00",
        "id": "491f0b00-ffff-4bc9-a43e-b226498ec22a"
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="795a5-155">请求</span><span class="sxs-lookup"><span data-stu-id="795a5-155">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="795a5-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="795a5-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request", 
  "name": "call-redirect"
} -->
``` http
POST https://graph.microsoft.com/v1.0/communications/calls/491f0b00-ffff-4bc9-a43e-b226498ec22a/redirect
Content-Type: application/json

{
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "application": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "test bot 2",
          "id": "22bfd41f-550e-477d-8789-f6f7bd2a5e8b"
        }
      }
    }
  ],
  "callbackUri": "https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039"
}
```
# <a name="c"></a>[<span data-ttu-id="795a5-157">C#</span><span class="sxs-lookup"><span data-stu-id="795a5-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-redirect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="795a5-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="795a5-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-redirect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="795a5-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="795a5-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-redirect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="795a5-160">Java</span><span class="sxs-lookup"><span data-stu-id="795a5-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-redirect-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="795a5-161">响应</span><span class="sxs-lookup"><span data-stu-id="795a5-161">Response</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
##### <a name="notification---terminated"></a><span data-ttu-id="795a5-162">通知终止</span><span class="sxs-lookup"><span data-stu-id="795a5-162">Notification - terminated</span></span>

<!-- {
  "blockType": "example", 
  "name": "call-redirect"
} -->
``` http
POST https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039
Content-Type: application/json
```

<!-- {
  "blockType": "example", 
  "@odata.type": "microsoft.graph.commsNotifications"
} -->
``` json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resourceUrl": "/communications/calls/491f0b00-ffff-4bc9-a43e-b226498ec22a",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminated",
        "direction": "incoming",
        "callbackUri": "https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039",
        "source": {
          "@odata.type": "#microsoft.graph.participantInfo",
          "identity": {
            "@odata.type": "#microsoft.graph.identitySet",
            "user": {
              "@odata.type": "#microsoft.graph.identity",
              "id": "8d1e6ab6-26c5-4e22-a1bc-06ea7343958e"
            }
          },
          "region": "amer",
        },
        "targets": [
          {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "application": {
                "@odata.type": "#microsoft.graph.identity",
                "displayName": "test bot",
                "id": "24701998-1a73-4d42-8085-bf46ed0ae039"
              }
            }
          }
        ],
        "myParticipantId": "c339cede-4bd6-4f20-ab9f-3a13e65f6d00",
        "id": "491f0b00-ffff-4bc9-a43e-b226498ec22a"
      }
    }
  ]
}
```

### <a name="example-2-forward-a-call-to-multiple-targets-with-simultaneous-ring"></a><span data-ttu-id="795a5-163">示例2：通过同时响铃向多个目标转发呼叫</span><span class="sxs-lookup"><span data-stu-id="795a5-163">Example 2: Forward a call to multiple targets with simultaneous ring</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="795a5-164">通知传入</span><span class="sxs-lookup"><span data-stu-id="795a5-164">Notification - incoming</span></span>

<!-- {
  "blockType": "example", 
  "name": "call-redirect"
} -->
``` http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example", 
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "created",
      "resourceUrl": "/communications/calls/481f0b00-ffff-4ca1-8c67-a5f1e31e8e82",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "incoming",
        "direction": "incoming",
        "callbackUri": "https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039",
        "source": {
          "@odata.type": "#microsoft.graph.participantInfo",
          "identity": {
            "@odata.type": "#microsoft.graph.identitySet",
            "user": {
              "@odata.type": "#microsoft.graph.identity",
              "id": "ec040873-8235-45fd-a403-c7259a5a548e"
            }
          },
          "region": "amer"
        },
        "targets": [
          {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "application": {
                "@odata.type": "#microsoft.graph.identity",
                "displayName": "test bot",
                "id": "24701998-1a73-4d42-8085-bf46ed0ae039"
              }
            }
          }
        ],
        "myParticipantId": "f540f1b6-994b-4866-be95-8aad34c4f4dc",
        "id": "481f0b00-ffff-4ca1-8c67-a5f1e31e8e82"
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="795a5-165">请求</span><span class="sxs-lookup"><span data-stu-id="795a5-165">Request</span></span>

<!-- {
  "blockType": "ignored", 
  "name": "call-redirect-simuring"
} -->

``` http
POST https://graph.microsoft.com/v1.0/communications/calls/481f0b00-ffff-4ca1-8c67-a5f1e31e8e82/redirect
Content-Type: application/json

{
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "test user",
          "id": "98da8a1a-1b87-452c-a713-65d3f10b1253"
        }
      }
    },
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "test user 2",
          "id": "bf5aae9a-d11d-47a8-93b1-782504c9c3f3"
        }
      }
    }
  ],
  "routingPolicies": [
    "disableForwarding"
  ],
  "callbackUri": "https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039"
}
```

##### <a name="response"></a><span data-ttu-id="795a5-166">响应</span><span class="sxs-lookup"><span data-stu-id="795a5-166">Response</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->

``` http
HTTP/1.1 202 Accepted
```

##### <a name="notification---terminated"></a><span data-ttu-id="795a5-167">通知终止</span><span class="sxs-lookup"><span data-stu-id="795a5-167">Notification - terminated</span></span>

<!-- {
  "blockType": "example", 
  "@odata.type": "microsoft.graph.commsNotifications"
} -->

``` http
POST https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resourceUrl": "/communications/calls/491f0b00-ffff-4bc9-a43e-b226498ec22a",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminated",
        "direction": "incoming",
        "callbackUri": "https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039",
        "source": {
          "@odata.type": "#microsoft.graph.participantInfo",
          "identity": {
            "@odata.type": "#microsoft.graph.identitySet",
            "user": {
              "@odata.type": "#microsoft.graph.identity",
              "id": "ec040873-8235-45fd-a403-c7259a5a548e"
            }
          },
          "region": "amer"
        },
        "targets": [
          {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "application": {
                "@odata.type": "#microsoft.graph.identity",
                "displayName": "test bot",
                "id": "24701998-1a73-4d42-8085-bf46ed0ae039"
              }
            }
          }
        ],
        "myParticipantId": "f540f1b6-994b-4866-be95-8aad34c4f4dc",
        "id": "481f0b00-ffff-4ca1-8c67-a5f1e31e8e82"
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
  "description": "call: redirect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

