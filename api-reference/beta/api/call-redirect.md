---
title: call： redirect
description: 重定向传入呼叫。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 8a3919c2a84b8b248f81599359dcba92d58f830f
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/19/2020
ms.locfileid: "49719676"
---
# <a name="call-redirect"></a><span data-ttu-id="39990-103">call： redirect</span><span class="sxs-lookup"><span data-stu-id="39990-103">call: redirect</span></span>

<span data-ttu-id="39990-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39990-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39990-105">重定向尚未应答[或拒绝的传入](./call-answer.md)[呼叫。](./call-reject.md)</span><span class="sxs-lookup"><span data-stu-id="39990-105">Redirect an incoming call that hasn't been [answered](./call-answer.md) or [rejected](./call-reject.md) yet.</span></span> <span data-ttu-id="39990-106">呼叫的术语"重定向"和"转发"可以互换使用。</span><span class="sxs-lookup"><span data-stu-id="39990-106">The terms "redirecting" and "forwarding" a call are used interchangeably.</span></span>

<span data-ttu-id="39990-107">机器人预期在呼叫退出之前重定向呼叫。当前超时值为 15 秒。</span><span class="sxs-lookup"><span data-stu-id="39990-107">The bot is expected to redirect the call before the call times out. The current timeout value is 15 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="39990-108">权限</span><span class="sxs-lookup"><span data-stu-id="39990-108">Permissions</span></span>

<span data-ttu-id="39990-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="39990-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="39990-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="39990-111">Permission type</span></span> | <span data-ttu-id="39990-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="39990-112">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="39990-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="39990-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="39990-114">不支持</span><span class="sxs-lookup"><span data-stu-id="39990-114">Not Supported</span></span>                |
| <span data-ttu-id="39990-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="39990-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39990-116">不支持</span><span class="sxs-lookup"><span data-stu-id="39990-116">Not Supported</span></span>                |
| <span data-ttu-id="39990-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="39990-117">Application</span></span>     | <span data-ttu-id="39990-118">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="39990-118">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="39990-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="39990-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /app/calls/{id}/redirect
POST /communications/calls/{id}/redirect
```
> <span data-ttu-id="39990-120">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="39990-120">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="39990-121">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="39990-121">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="39990-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="39990-122">Request headers</span></span>

| <span data-ttu-id="39990-123">名称</span><span class="sxs-lookup"><span data-stu-id="39990-123">Name</span></span>          | <span data-ttu-id="39990-124">说明</span><span class="sxs-lookup"><span data-stu-id="39990-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="39990-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="39990-125">Authorization</span></span> | <span data-ttu-id="39990-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="39990-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="39990-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="39990-128">Request body</span></span>

<span data-ttu-id="39990-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="39990-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="39990-130">参数</span><span class="sxs-lookup"><span data-stu-id="39990-130">Parameter</span></span>      | <span data-ttu-id="39990-131">类型</span><span class="sxs-lookup"><span data-stu-id="39990-131">Type</span></span>    |<span data-ttu-id="39990-132">说明</span><span class="sxs-lookup"><span data-stu-id="39990-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="39990-133">targets</span><span class="sxs-lookup"><span data-stu-id="39990-133">targets</span></span>|<span data-ttu-id="39990-134">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="39990-134">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>|<span data-ttu-id="39990-135">重定向操作的目标参与者。</span><span class="sxs-lookup"><span data-stu-id="39990-135">The target participants of the redirect operation.</span></span> <span data-ttu-id="39990-136">如果指定了多个目标，则这是一个模拟调用。</span><span class="sxs-lookup"><span data-stu-id="39990-136">If more than one target is specified, it's a simulring call.</span></span> <span data-ttu-id="39990-137">这意味着将同时设定所有目标范围，并且仅连接第一个选取的目标。</span><span class="sxs-lookup"><span data-stu-id="39990-137">This means that all of the targets will be rang at the same time and only the first target that picks up will be connected.</span></span> <span data-ttu-id="39990-138">我们最多支持 25 个目标进行模拟。</span><span class="sxs-lookup"><span data-stu-id="39990-138">We support up to 25 targets for simulring.</span></span>
|<span data-ttu-id="39990-139">targetDisposition</span><span class="sxs-lookup"><span data-stu-id="39990-139">targetDisposition</span></span>|<span data-ttu-id="39990-140">String</span><span class="sxs-lookup"><span data-stu-id="39990-140">String</span></span>|<span data-ttu-id="39990-141"> (弃) 可能的值是： `default` `simultaneousRing` ， `forward` 。</span><span class="sxs-lookup"><span data-stu-id="39990-141">(Deprecated) The possible values are: `default` , `simultaneousRing` , `forward`.</span></span> <span data-ttu-id="39990-142">此参数已弃用，我们将根据提供的目标数自动标识它是一个转发呼叫还是模拟呼叫。</span><span class="sxs-lookup"><span data-stu-id="39990-142">This parameter is deprecated, we will automatically identify whether it's a forward call or simulring call from the number of targets provided.</span></span>|
|<span data-ttu-id="39990-143">timeout</span><span class="sxs-lookup"><span data-stu-id="39990-143">timeout</span></span>|<span data-ttu-id="39990-144">Int32</span><span class="sxs-lookup"><span data-stu-id="39990-144">Int32</span></span>|<span data-ttu-id="39990-145">对于重定向 (超时) 秒。</span><span class="sxs-lookup"><span data-stu-id="39990-145">The timeout (in seconds) for the redirect operation.</span></span> <span data-ttu-id="39990-146">超时值的范围介于 15 到 90 秒之间（包括 15 秒和 90 秒）。</span><span class="sxs-lookup"><span data-stu-id="39990-146">The range of the timeout value is between 15 and 90 seconds inclusive.</span></span> <span data-ttu-id="39990-147">一个目标的默认超时值为 55 秒，多个目标的默认超时值为 60 (可能会) 。</span><span class="sxs-lookup"><span data-stu-id="39990-147">The default timeout value is 55 seconds for one target and 60 seconds for multiple targets (subject to change).</span></span> |
|<span data-ttu-id="39990-148">maskCallee</span><span class="sxs-lookup"><span data-stu-id="39990-148">maskCallee</span></span>|<span data-ttu-id="39990-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="39990-149">Boolean</span></span>|<span data-ttu-id="39990-150">指示是否向呼叫者隐藏被叫方。</span><span class="sxs-lookup"><span data-stu-id="39990-150">Indicates whether the callee is to be hidden from the caller.</span></span> <span data-ttu-id="39990-151">如果为 true，则被叫方标识为机器人标识。</span><span class="sxs-lookup"><span data-stu-id="39990-151">If true, then the callee identity is the bot identity.</span></span> <span data-ttu-id="39990-152">默认值：false。</span><span class="sxs-lookup"><span data-stu-id="39990-152">Default: false.</span></span>|
|<span data-ttu-id="39990-153">maskCaller</span><span class="sxs-lookup"><span data-stu-id="39990-153">maskCaller</span></span>|<span data-ttu-id="39990-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="39990-154">Boolean</span></span>|<span data-ttu-id="39990-155">指示是否对被叫方隐藏呼叫者。</span><span class="sxs-lookup"><span data-stu-id="39990-155">Indicates whether the caller is to be hidden from the callee.</span></span> <span data-ttu-id="39990-156">如果为 true，则呼叫者标识为机器人标识。</span><span class="sxs-lookup"><span data-stu-id="39990-156">If true, then the caller identity is the bot identity.</span></span> <span data-ttu-id="39990-157">默认值：false。</span><span class="sxs-lookup"><span data-stu-id="39990-157">Default: false.</span></span>|
|<span data-ttu-id="39990-158">callbackUri</span><span class="sxs-lookup"><span data-stu-id="39990-158">callbackUri</span></span>|<span data-ttu-id="39990-159">String</span><span class="sxs-lookup"><span data-stu-id="39990-159">String</span></span>|<span data-ttu-id="39990-160">这允许机器人为当前调用提供特定的回调 URI，以接收以后的通知。</span><span class="sxs-lookup"><span data-stu-id="39990-160">This allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="39990-161">如果尚未设置此属性，将改为使用自动程序全局回调 URI。</span><span class="sxs-lookup"><span data-stu-id="39990-161">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="39990-162">这必须是 `https` 。</span><span class="sxs-lookup"><span data-stu-id="39990-162">This must be `https`.</span></span>|

## <a name="response"></a><span data-ttu-id="39990-163">响应</span><span class="sxs-lookup"><span data-stu-id="39990-163">Response</span></span>
<span data-ttu-id="39990-164">如果成功，此方法返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="39990-164">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="39990-165">示例</span><span class="sxs-lookup"><span data-stu-id="39990-165">Examples</span></span>
<span data-ttu-id="39990-166">这些示例将介绍传入呼叫通知的工作流以及如何重定向该呼叫。</span><span class="sxs-lookup"><span data-stu-id="39990-166">These examples will cover a workflow of an incoming call notification and how that call will be redirected.</span></span>

> <span data-ttu-id="39990-167">**注意：** 为了可读性，可能会缩短此处所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="39990-167">**Note:** The response objects shown here might be shortened for readability.</span></span> <span data-ttu-id="39990-168">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="39990-168">All the properties will be returned from an actual call.</span></span>

### <a name="example-1-forward-a-call-to-a-target"></a><span data-ttu-id="39990-169">示例 1：将呼叫转发到目标</span><span class="sxs-lookup"><span data-stu-id="39990-169">Example 1: Forward a call to a target</span></span>

#### <a name="notification---incoming"></a><span data-ttu-id="39990-170">通知 - 传入</span><span class="sxs-lookup"><span data-stu-id="39990-170">Notification - incoming</span></span>
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
              "id": "8d1e6ab6-26c5-4e22-a1bc-06ea7343958e",
              "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f"
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
        "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f",
        "myParticipantId": "c339cede-4bd6-4f20-ab9f-3a13e65f6d00",
        "id": "491f0b00-ffff-4bc9-a43e-b226498ec22a"
      }
    }
  ]
}
```

#### <a name="request"></a><span data-ttu-id="39990-171">请求</span><span class="sxs-lookup"><span data-stu-id="39990-171">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="39990-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="39990-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request", 
  "name": "call-redirect"
} -->
``` http
POST https://graph.microsoft.com/beta/communications/calls/491f0b00-ffff-4bc9-a43e-b226498ec22a/redirect
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
# <a name="c"></a>[<span data-ttu-id="39990-173">C#</span><span class="sxs-lookup"><span data-stu-id="39990-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-redirect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39990-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39990-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-redirect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39990-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39990-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-redirect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="39990-176">Java</span><span class="sxs-lookup"><span data-stu-id="39990-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-redirect-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="39990-177">响应</span><span class="sxs-lookup"><span data-stu-id="39990-177">Response</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="notification---terminated"></a><span data-ttu-id="39990-178">Notification - 已终止</span><span class="sxs-lookup"><span data-stu-id="39990-178">Notification - terminated</span></span>

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
              "id": "8d1e6ab6-26c5-4e22-a1bc-06ea7343958e",
              "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f"
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
        "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f",
        "myParticipantId": "c339cede-4bd6-4f20-ab9f-3a13e65f6d00",
        "id": "491f0b00-ffff-4bc9-a43e-b226498ec22a"
      }
    }
  ]
}
```

### <a name="example-2-forward-a-call-to-multiple-targets-with-simultaneous-ring"></a><span data-ttu-id="39990-179">示例 2：将呼叫转发到同时响铃的多个目标</span><span class="sxs-lookup"><span data-stu-id="39990-179">Example 2: Forward a call to multiple targets with simultaneous ring</span></span>

#### <a name="notification---incoming"></a><span data-ttu-id="39990-180">通知 - 传入</span><span class="sxs-lookup"><span data-stu-id="39990-180">Notification - incoming</span></span>

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
              "id": "ec040873-8235-45fd-a403-c7259a5a548e",
              "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f"
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
        "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f",
        "myParticipantId": "f540f1b6-994b-4866-be95-8aad34c4f4dc",
        "id": "481f0b00-ffff-4ca1-8c67-a5f1e31e8e82"
      }
    }
  ]
}
```

#### <a name="request"></a><span data-ttu-id="39990-181">请求</span><span class="sxs-lookup"><span data-stu-id="39990-181">Request</span></span>

<!-- {
  "blockType": "ignored", 
  "name": "call-redirect-simuring"
} -->

``` http
POST https://graph.microsoft.com/beta/communications/calls/481f0b00-ffff-4ca1-8c67-a5f1e31e8e82/redirect
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

#### <a name="response"></a><span data-ttu-id="39990-182">响应</span><span class="sxs-lookup"><span data-stu-id="39990-182">Response</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->

``` http
HTTP/1.1 202 Accepted
```

#### <a name="notification---terminated"></a><span data-ttu-id="39990-183">Notification - 已终止</span><span class="sxs-lookup"><span data-stu-id="39990-183">Notification - terminated</span></span>

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
              "id": "ec040873-8235-45fd-a403-c7259a5a548e",
              "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f"
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
        "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f",
        "myParticipantId": "f540f1b6-994b-4866-be95-8aad34c4f4dc",
        "id": "481f0b00-ffff-4ca1-8c67-a5f1e31e8e82"
      }
    }
  ]
}
```

### <a name="example-3-forward-a-call-to-a-pstn-number"></a><span data-ttu-id="39990-184">示例 3：将呼叫转发到 PSTN 号码</span><span class="sxs-lookup"><span data-stu-id="39990-184">Example 3: Forward a call to a PSTN number</span></span>

<span data-ttu-id="39990-185">此呼叫需要分配有 PSTN 号码的应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="39990-185">This call requires an application instance with a PSTN number assigned.</span></span>

#### <a name="step-1-create-application-instance"></a><span data-ttu-id="39990-186">步骤 1：创建应用程序实例</span><span class="sxs-lookup"><span data-stu-id="39990-186">Step 1: Create application instance</span></span>
<span data-ttu-id="39990-187">使用租户管理员凭据，在租户远程 PowerShell 上调用以下 cmdlet 以创建应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="39990-187">Using tenant admin credentials, call the following cmdlets on the tenant remote PowerShell to create the application instance.</span></span> <span data-ttu-id="39990-188">有关详细信息，请参阅 [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) 和 [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true)。</span><span class="sxs-lookup"><span data-stu-id="39990-188">For more information, see [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>
```
PS C:\> New-CsOnlineApplicationInstance -UserPrincipalName <UPN> -DisplayName <DisplayName> -ApplicationId <AppId>
PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <ObjectId>
```
#### <a name="step-2-assign-microsoft-365-licenses"></a><span data-ttu-id="39990-189">步骤 2：分配 Microsoft 365 许可证</span><span class="sxs-lookup"><span data-stu-id="39990-189">Step 2: Assign Microsoft 365 licenses</span></span>
1. <span data-ttu-id="39990-190">使用租户管理员凭据登录并转到"用户 https://admin.microsoft.com/ **->活动用户"** 选项卡。</span><span class="sxs-lookup"><span data-stu-id="39990-190">Use tenant admin credentials to sign in to https://admin.microsoft.com/ and go to the **Users -> Active users** tab.</span></span>
2. <span data-ttu-id="39990-191">选择应用程序实例，分配 **Microsoft 365 国内和国际** 通话套餐和 **Microsoft 365 电话系统 - 虚拟用户** 许可证，然后单击"**保存更改"。**</span><span class="sxs-lookup"><span data-stu-id="39990-191">Select the application instance, assign **Microsoft 365 Domestic and International Calling Plan** and **Microsoft 365 Phone System - Virtual User** licenses, and click **Save changes**.</span></span> <span data-ttu-id="39990-192">如果所需的许可证在租户中不可用，可以从"计费-> **购买服务"** 选项卡获取它们。</span><span class="sxs-lookup"><span data-stu-id="39990-192">If the required licenses are not available in the tenant, you can get them from the **Billing -> Purchase services** tab.</span></span>
#### <a name="step-3-acquire-pstn-number"></a><span data-ttu-id="39990-193">步骤 3：获取 PSTN 号码</span><span class="sxs-lookup"><span data-stu-id="39990-193">Step 3: Acquire PSTN number</span></span>
1. <span data-ttu-id="39990-194">使用租户管理员凭据登录并单击左侧面板上的"旧版 https://admin.teams.microsoft.com/ 门户"选项卡。 </span><span class="sxs-lookup"><span data-stu-id="39990-194">Use tenant admin credentials to sign in to https://admin.teams.microsoft.com/ and click the **Legacy portal** tab on the left panel.</span></span>
2. <span data-ttu-id="39990-195">In the new page， go to the **voice -> phone numbers** tab.</span><span class="sxs-lookup"><span data-stu-id="39990-195">In the new page, go to the **voice -> phone numbers** tab.</span></span>
3. <span data-ttu-id="39990-196">单击 **+** 该按钮， **选择"新建服务号码**"，然后转到 **"添加新服务号码"** 页。</span><span class="sxs-lookup"><span data-stu-id="39990-196">Click the **+** button, select **New Service Numbers**, and go to the **Add new service numbers** page.</span></span>
4. <span data-ttu-id="39990-197">选择 **"国家/地区\*\*\*\*"、"省/地区**"、"**城市**"和"输入 **数量**"，然后单击 **"添加**"进行搜索。</span><span class="sxs-lookup"><span data-stu-id="39990-197">Select **Country/Region**, **State/Region**, **City**, input **Quantity**, and click **add** to search.</span></span> <span data-ttu-id="39990-198">单击 **获取号码**。</span><span class="sxs-lookup"><span data-stu-id="39990-198">Click **acquire numbers**.</span></span> <span data-ttu-id="39990-199">新获取的号码会显示在 **电话号码选项卡** 上。</span><span class="sxs-lookup"><span data-stu-id="39990-199">The newly acquired number will show on  the **phone numbers** tab.</span></span>
#### <a name="step-4-assign-pstn-number-to-application-instance"></a><span data-ttu-id="39990-200">步骤 4：将 PSTN 号码分配给应用程序实例</span><span class="sxs-lookup"><span data-stu-id="39990-200">Step 4: Assign PSTN number to application instance</span></span>
<span data-ttu-id="39990-201">使用租户管理员凭据，在租户远程 PowerShell 上调用以下 cmdlet，将 PSTN 号码分配给应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="39990-201">With tenant admin credentials, call the following cmdlets on the tenant remote PowerShell to assign the PSTN number to the application instance.</span></span> <span data-ttu-id="39990-202">有关详细信息，请参阅 [Set-CsOnlineVoiceApplicationInstance](https://docs.microsoft.com/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) 和 [Sync-CsOnlineApplicationInstance](https://docs.microsoft.com/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true)。</span><span class="sxs-lookup"><span data-stu-id="39990-202">For more information, see [Set-CsOnlineVoiceApplicationInstance](https://docs.microsoft.com/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](https://docs.microsoft.com/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>
```
PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <UPN> -TelephoneNumber <TelephoneNumber>
PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <ObjectId>
```
> <span data-ttu-id="39990-203">**注意：** 如果租户具有分配给任何应用程序实例的澳大利亚 PSTN 号码，则此呼叫可能会失败。</span><span class="sxs-lookup"><span data-stu-id="39990-203">**Note:** If a tenant has Australian PSTN numbers assigned to any application instances, this call might fail.</span></span> <span data-ttu-id="39990-204">如果租户是新创建的，可能需要几天时间，此功能可用。</span><span class="sxs-lookup"><span data-stu-id="39990-204">If a tenant is newly created, it might take several days for this feature to be available.</span></span>

#### <a name="notification---incoming"></a><span data-ttu-id="39990-205">通知 - 传入</span><span class="sxs-lookup"><span data-stu-id="39990-205">Notification - incoming</span></span>
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
              "id": "8d1e6ab6-26c5-4e22-a1bc-06ea7343958e",
              "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f"
            }
          },
          "region": "amer",
        },
        "targets": [
          {
            "@odata.type": "#microsoft.graph.invitationParticipantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "applicationInstance": {
                "@odata.type": "#microsoft.graph.identity",
                "displayName": "PstnAppInstance",
                "id": "7629bdce-046c-4903-86b4-a8f718277e1a",
                "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f"
              }
            },
            "endpointType": "default",
            "id": "c339cede-4bd6-4f20-ab9f-3a13e65f6d00",
            "region": "amer",
            "languageId": null
          }
        ],
        "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f",
        "myParticipantId": "c339cede-4bd6-4f20-ab9f-3a13e65f6d00",
        "id": "491f0b00-ffff-4bc9-a43e-b226498ec22a"
      }
    }
  ]
}
```

#### <a name="request"></a><span data-ttu-id="39990-206">请求</span><span class="sxs-lookup"><span data-stu-id="39990-206">Request</span></span>

<!-- {
  "blockType": "request", 
  "name": "call-redirect"
} -->
``` http
POST https://graph.microsoft.com/beta/communications/calls/491f0b00-ffff-4bc9-a43e-b226498ec22a/redirect
Content-Type: application/json

{
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "phone": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "+12345678901"
        }
      }
    }
  ],
  "callbackUri": "https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039"
}
```
#### <a name="response"></a><span data-ttu-id="39990-207">响应</span><span class="sxs-lookup"><span data-stu-id="39990-207">Response</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="notification---terminated"></a><span data-ttu-id="39990-208">Notification - 已终止</span><span class="sxs-lookup"><span data-stu-id="39990-208">Notification - terminated</span></span>

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
              "id": "8d1e6ab6-26c5-4e22-a1bc-06ea7343958e",
              "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f"
            }
          },
          "region": "amer",
        },
        "targets": [
          {
            "@odata.type": "#microsoft.graph.invitationParticipantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "applicationInstance": {
                "@odata.type": "#microsoft.graph.identity",
                "displayName": "PstnAppInstance",
                "id": "7629bdce-046c-4903-86b4-a8f718277e1a",
                "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f"
              }
            },
            "endpointType": "default",
            "id": "c339cede-4bd6-4f20-ab9f-3a13e65f6d00",
            "region": "amer",
            "languageId": null
          }
        ],
        "answeredBy": {
          "@odata.type": "#microsoft.graph.participantInfo",
          "identity": {
            "@odata.type": "#microsoft.graph.identitySet",
            "encrypted": {
              "@odata.type": "#microsoft.graph.identity",
              "id": "1xt4uextl99sdzwdxuvdxrvgrv8gehcq7jdgf9yhzeto"
            }
          },
          "endpointType": "default"
        },
        "tenantId": "632899f8-2ea1-4604-8413-27bd2892079f",
        "myParticipantId": "c339cede-4bd6-4f20-ab9f-3a13e65f6d00",
        "id": "491f0b00-ffff-4bc9-a43e-b226498ec22a"
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


