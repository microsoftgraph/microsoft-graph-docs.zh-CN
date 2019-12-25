---
title: 呼叫：重定向
description: 重定向传入呼叫。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: d9f366f601fe7b9580b359c2b469f6a074771b5d
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871103"
---
# <a name="call-redirect"></a><span data-ttu-id="8ae8d-103">呼叫：重定向</span><span class="sxs-lookup"><span data-stu-id="8ae8d-103">call: redirect</span></span>

<span data-ttu-id="8ae8d-104">重定向尚未[应答](./call-answer.md)或[拒绝](./call-reject.md)的传入呼叫。</span><span class="sxs-lookup"><span data-stu-id="8ae8d-104">Redirect an incoming call that hasn't been [answered](./call-answer.md) or [rejected](./call-reject.md) yet.</span></span> <span data-ttu-id="8ae8d-105">术语 "重定向" 和 "转发" 可交换使用呼叫。</span><span class="sxs-lookup"><span data-stu-id="8ae8d-105">The terms "redirecting" and "forwarding" a call are used interchangeably.</span></span>

<span data-ttu-id="8ae8d-106">在呼叫超时之前，机器人应重定向呼叫。当前超时值为15秒。</span><span class="sxs-lookup"><span data-stu-id="8ae8d-106">The bot is expected to redirect the call before the call times out. The current timeout value is 15 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ae8d-107">权限</span><span class="sxs-lookup"><span data-stu-id="8ae8d-107">Permissions</span></span>

<span data-ttu-id="8ae8d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8ae8d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8ae8d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8ae8d-110">Permission type</span></span> | <span data-ttu-id="8ae8d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8ae8d-111">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="8ae8d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8ae8d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="8ae8d-113">不支持</span><span class="sxs-lookup"><span data-stu-id="8ae8d-113">Not Supported</span></span>                |
| <span data-ttu-id="8ae8d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8ae8d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ae8d-115">不支持</span><span class="sxs-lookup"><span data-stu-id="8ae8d-115">Not Supported</span></span>                |
| <span data-ttu-id="8ae8d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8ae8d-116">Application</span></span>     | <span data-ttu-id="8ae8d-117">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="8ae8d-117">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="8ae8d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8ae8d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /communications/calls/{id}/redirect
```

## <a name="request-headers"></a><span data-ttu-id="8ae8d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8ae8d-119">Request headers</span></span>

| <span data-ttu-id="8ae8d-120">名称</span><span class="sxs-lookup"><span data-stu-id="8ae8d-120">Name</span></span>          | <span data-ttu-id="8ae8d-121">说明</span><span class="sxs-lookup"><span data-stu-id="8ae8d-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8ae8d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ae8d-122">Authorization</span></span> | <span data-ttu-id="8ae8d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8ae8d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ae8d-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="8ae8d-125">Request body</span></span>

<span data-ttu-id="8ae8d-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="8ae8d-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8ae8d-127">参数</span><span class="sxs-lookup"><span data-stu-id="8ae8d-127">Parameter</span></span>      | <span data-ttu-id="8ae8d-128">类型</span><span class="sxs-lookup"><span data-stu-id="8ae8d-128">Type</span></span>    |<span data-ttu-id="8ae8d-129">说明</span><span class="sxs-lookup"><span data-stu-id="8ae8d-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ae8d-130">targets</span><span class="sxs-lookup"><span data-stu-id="8ae8d-130">targets</span></span>|<span data-ttu-id="8ae8d-131">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8ae8d-131">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>|<span data-ttu-id="8ae8d-132">重定向操作的目标参与者。</span><span class="sxs-lookup"><span data-stu-id="8ae8d-132">The target participants of the redirect operation.</span></span> <span data-ttu-id="8ae8d-133">如果指定了多个目标，则为同时调用。</span><span class="sxs-lookup"><span data-stu-id="8ae8d-133">If more than one target is specified, it's a simulring call.</span></span> <span data-ttu-id="8ae8d-134">这意味着将同时 rang 所有目标，并且只会连接所选取的第一个目标。</span><span class="sxs-lookup"><span data-stu-id="8ae8d-134">This means that all of the targets will be rang at the same time and only the first target that picks up will be connected.</span></span> <span data-ttu-id="8ae8d-135">对于同时，我们最高支持25个目标。</span><span class="sxs-lookup"><span data-stu-id="8ae8d-135">We support up to 25 targets for simulring.</span></span>
|<span data-ttu-id="8ae8d-136">timeout</span><span class="sxs-lookup"><span data-stu-id="8ae8d-136">timeout</span></span>|<span data-ttu-id="8ae8d-137">Int32</span><span class="sxs-lookup"><span data-stu-id="8ae8d-137">Int32</span></span>|<span data-ttu-id="8ae8d-138">重定向操作的超时（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="8ae8d-138">The timeout (in seconds) for the redirect operation.</span></span> <span data-ttu-id="8ae8d-139">超时值的范围介于15和90秒之间（含这两个值）。</span><span class="sxs-lookup"><span data-stu-id="8ae8d-139">The range of the timeout value is between 15 and 90 seconds inclusive.</span></span> <span data-ttu-id="8ae8d-140">对于多个目标，默认超时值为55秒，为多个目标为60秒（可能会发生更改）。</span><span class="sxs-lookup"><span data-stu-id="8ae8d-140">The default timeout value is 55 seconds for one target and 60 seconds for multiple targets (subject to change).</span></span> |
|<span data-ttu-id="8ae8d-141">callbackUri</span><span class="sxs-lookup"><span data-stu-id="8ae8d-141">callbackUri</span></span>|<span data-ttu-id="8ae8d-142">String</span><span class="sxs-lookup"><span data-stu-id="8ae8d-142">String</span></span>|<span data-ttu-id="8ae8d-143">这将允许 bot 为当前呼叫提供特定的回调 URI，以接收后续通知。</span><span class="sxs-lookup"><span data-stu-id="8ae8d-143">This allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="8ae8d-144">如果尚未设置此属性，则将改为使用 bot 的全局回调 URI。</span><span class="sxs-lookup"><span data-stu-id="8ae8d-144">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="8ae8d-145">这必须是`https`。</span><span class="sxs-lookup"><span data-stu-id="8ae8d-145">This must be `https`.</span></span>|

## <a name="response"></a><span data-ttu-id="8ae8d-146">响应</span><span class="sxs-lookup"><span data-stu-id="8ae8d-146">Response</span></span>
<span data-ttu-id="8ae8d-147">如果成功，此方法返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="8ae8d-147">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="8ae8d-148">示例</span><span class="sxs-lookup"><span data-stu-id="8ae8d-148">Examples</span></span>
<span data-ttu-id="8ae8d-149">这些示例将涵盖传入呼叫通知的工作流以及该呼叫将如何重定向。</span><span class="sxs-lookup"><span data-stu-id="8ae8d-149">These examples will cover a workflow of an incoming call notification and how that call will be redirected.</span></span>

> <span data-ttu-id="8ae8d-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8ae8d-150">**Note:** The response objects shown here might be shortened for readability.</span></span> <span data-ttu-id="8ae8d-151">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8ae8d-151">All the properties will be returned from an actual call.</span></span>

### <a name="example-1-forward-a-call-to-a-target"></a><span data-ttu-id="8ae8d-152">示例1：将呼叫转接到目标</span><span class="sxs-lookup"><span data-stu-id="8ae8d-152">Example 1: Forward a Call to a Target</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="8ae8d-153">通知传入</span><span class="sxs-lookup"><span data-stu-id="8ae8d-153">Notification - incoming</span></span>
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

##### <a name="request"></a><span data-ttu-id="8ae8d-154">请求</span><span class="sxs-lookup"><span data-stu-id="8ae8d-154">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8ae8d-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ae8d-155">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="8ae8d-156">C#</span><span class="sxs-lookup"><span data-stu-id="8ae8d-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-redirect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8ae8d-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ae8d-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-redirect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8ae8d-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8ae8d-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-redirect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8ae8d-159">Java</span><span class="sxs-lookup"><span data-stu-id="8ae8d-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-redirect-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8ae8d-160">响应</span><span class="sxs-lookup"><span data-stu-id="8ae8d-160">Response</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
##### <a name="notification---terminated"></a><span data-ttu-id="8ae8d-161">通知终止</span><span class="sxs-lookup"><span data-stu-id="8ae8d-161">Notification - terminated</span></span>

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

### <a name="example-2-forward-a-call-to-multiple-targets-with-simultaneous-ring"></a><span data-ttu-id="8ae8d-162">示例2：通过同时响铃向多个目标转发呼叫</span><span class="sxs-lookup"><span data-stu-id="8ae8d-162">Example 2: Forward a call to multiple targets with simultaneous ring</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="8ae8d-163">通知传入</span><span class="sxs-lookup"><span data-stu-id="8ae8d-163">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="8ae8d-164">请求</span><span class="sxs-lookup"><span data-stu-id="8ae8d-164">Request</span></span>

<!-- {
  "blockType": "request", 
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

##### <a name="response"></a><span data-ttu-id="8ae8d-165">响应</span><span class="sxs-lookup"><span data-stu-id="8ae8d-165">Response</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->

``` http
HTTP/1.1 202 Accepted
```

##### <a name="notification---terminated"></a><span data-ttu-id="8ae8d-166">通知终止</span><span class="sxs-lookup"><span data-stu-id="8ae8d-166">Notification - terminated</span></span>

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
