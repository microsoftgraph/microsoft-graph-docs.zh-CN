---
title: 呼叫：重定向
description: 重定向传入呼叫。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7ea4e128f6cbbdd8184afdcb7113271fa32510df
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792263"
---
# <a name="call-redirect"></a><span data-ttu-id="65daf-103">呼叫：重定向</span><span class="sxs-lookup"><span data-stu-id="65daf-103">call: redirect</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65daf-104">重定向传入呼叫。</span><span class="sxs-lookup"><span data-stu-id="65daf-104">Redirect an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="65daf-105">权限</span><span class="sxs-lookup"><span data-stu-id="65daf-105">Permissions</span></span>
<span data-ttu-id="65daf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="65daf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="65daf-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="65daf-108">Permission type</span></span> | <span data-ttu-id="65daf-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="65daf-109">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="65daf-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="65daf-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="65daf-111">不支持</span><span class="sxs-lookup"><span data-stu-id="65daf-111">Not Supported</span></span>                |
| <span data-ttu-id="65daf-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="65daf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65daf-113">不支持</span><span class="sxs-lookup"><span data-stu-id="65daf-113">Not Supported</span></span>                |
| <span data-ttu-id="65daf-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="65daf-114">Application</span></span>     | <span data-ttu-id="65daf-115">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="65daf-115">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="65daf-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65daf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/redirect
POST /applications/{id}/calls/{id}/redirect
```

## <a name="request-headers"></a><span data-ttu-id="65daf-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="65daf-117">Request headers</span></span>
| <span data-ttu-id="65daf-118">名称</span><span class="sxs-lookup"><span data-stu-id="65daf-118">Name</span></span>          | <span data-ttu-id="65daf-119">说明</span><span class="sxs-lookup"><span data-stu-id="65daf-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="65daf-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="65daf-120">Authorization</span></span> | <span data-ttu-id="65daf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="65daf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="65daf-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="65daf-123">Request body</span></span>
<span data-ttu-id="65daf-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="65daf-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="65daf-125">参数</span><span class="sxs-lookup"><span data-stu-id="65daf-125">Parameter</span></span>      | <span data-ttu-id="65daf-126">类型</span><span class="sxs-lookup"><span data-stu-id="65daf-126">Type</span></span>    |<span data-ttu-id="65daf-127">说明</span><span class="sxs-lookup"><span data-stu-id="65daf-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65daf-128">targets</span><span class="sxs-lookup"><span data-stu-id="65daf-128">targets</span></span>|<span data-ttu-id="65daf-129">[invitationParticipantInfo](../resources/invitationparticipantinfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="65daf-129">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>|<span data-ttu-id="65daf-130">重定向操作的目标参与者。</span><span class="sxs-lookup"><span data-stu-id="65daf-130">The target participants of the redirect operation.</span></span>|
|<span data-ttu-id="65daf-131">targetDisposition</span><span class="sxs-lookup"><span data-stu-id="65daf-131">targetDisposition</span></span>|<span data-ttu-id="65daf-132">String</span><span class="sxs-lookup"><span data-stu-id="65daf-132">String</span></span>|<span data-ttu-id="65daf-133">可能的值为：`default`</span><span class="sxs-lookup"><span data-stu-id="65daf-133">The possible value is: `default`</span></span>|
|<span data-ttu-id="65daf-134">timeout</span><span class="sxs-lookup"><span data-stu-id="65daf-134">timeout</span></span>|<span data-ttu-id="65daf-135">Int32</span><span class="sxs-lookup"><span data-stu-id="65daf-135">Int32</span></span>|<span data-ttu-id="65daf-136">重定向操作的超时时间（秒）。</span><span class="sxs-lookup"><span data-stu-id="65daf-136">The timeout in seconds for the redirect operation.</span></span>|
|<span data-ttu-id="65daf-137">maskCallee</span><span class="sxs-lookup"><span data-stu-id="65daf-137">maskCallee</span></span>|<span data-ttu-id="65daf-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="65daf-138">Boolean</span></span>|<span data-ttu-id="65daf-139">指示是否屏蔽被叫方。</span><span class="sxs-lookup"><span data-stu-id="65daf-139">Indicates whether to mask the callee.</span></span>|
|<span data-ttu-id="65daf-140">maskCaller</span><span class="sxs-lookup"><span data-stu-id="65daf-140">maskCaller</span></span>|<span data-ttu-id="65daf-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="65daf-141">Boolean</span></span>|<span data-ttu-id="65daf-142">指示是否屏蔽调用方。</span><span class="sxs-lookup"><span data-stu-id="65daf-142">Indicates whether to mask the caller.</span></span>|
|<span data-ttu-id="65daf-143">callbackUri</span><span class="sxs-lookup"><span data-stu-id="65daf-143">callbackUri</span></span>|<span data-ttu-id="65daf-144">String</span><span class="sxs-lookup"><span data-stu-id="65daf-144">String</span></span>|<span data-ttu-id="65daf-145">允许 bot 提供特定的回调 URI，在此 URI 中，重定向操作的结果将被发布。</span><span class="sxs-lookup"><span data-stu-id="65daf-145">Allows bots to provide a specific callback URI where the result of the Redirect action will be posted.</span></span> <span data-ttu-id="65daf-146">这允许将结果发送到触发重定向操作的相同特定 bot 实例。</span><span class="sxs-lookup"><span data-stu-id="65daf-146">This allows sending the result to the same specific bot instance that triggered the Redirect action.</span></span> <span data-ttu-id="65daf-147">如果未提供，则将使用 bot 的全局回调 URI。</span><span class="sxs-lookup"><span data-stu-id="65daf-147">If none is provided, the bot's global callback URI will be used.</span></span>|

## <a name="response"></a><span data-ttu-id="65daf-148">响应</span><span class="sxs-lookup"><span data-stu-id="65daf-148">Response</span></span>
<span data-ttu-id="65daf-149">返回`202 Accepted`响应代码</span><span class="sxs-lookup"><span data-stu-id="65daf-149">Returns `202 Accepted` response code</span></span>

## <a name="examples"></a><span data-ttu-id="65daf-150">示例</span><span class="sxs-lookup"><span data-stu-id="65daf-150">Examples</span></span>

### <a name="redirect-a-call"></a><span data-ttu-id="65daf-151">重定向呼叫</span><span class="sxs-lookup"><span data-stu-id="65daf-151">Redirect a call</span></span>

##### <a name="request"></a><span data-ttu-id="65daf-152">请求</span><span class="sxs-lookup"><span data-stu-id="65daf-152">Request</span></span>
<span data-ttu-id="65daf-153">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="65daf-153">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="65daf-154">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="65daf-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-redirect"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/redirect
Content-Type: application/json
Content-Length: 515

{
  "targets": [
    {
      "endpointType": "default",
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "languageId": "en-US",
      "region": "westus"
    }
  ],
  "targetDisposition": "default",
  "timeout": 99,
  "maskCallee": false,
  "maskCaller": false
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="65daf-155">C#</span><span class="sxs-lookup"><span data-stu-id="65daf-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-redirect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="65daf-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65daf-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-redirect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="65daf-157">目标-C</span><span class="sxs-lookup"><span data-stu-id="65daf-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-redirect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="65daf-158">响应</span><span class="sxs-lookup"><span data-stu-id="65daf-158">Response</span></span>

> <span data-ttu-id="65daf-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="65daf-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="forward-a-call"></a><span data-ttu-id="65daf-161">转接呼叫</span><span class="sxs-lookup"><span data-stu-id="65daf-161">Forward a call</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="65daf-162">通知传入</span><span class="sxs-lookup"><span data-stu-id="65daf-162">Notification - incoming</span></span>

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
            "region": "westus",
            "languageId": "en-US"
          }
        ],
        "requestedModalities": [ "audio", "video" ]
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="65daf-163">请求</span><span class="sxs-lookup"><span data-stu-id="65daf-163">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls/57DAB8B1894C409AB240BD8BEAE78896/redirect
Authorization: Bearer <TOKEN>
Content-Type: application/json

{
  "targets": [
    {
      "endpointType": "default",
      "identity": {
        "user": {
          "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572699"
        }
      },
      "languageId": "en-US",
      "region": "westus"
    }
  ],
  "targetDisposition": "default",
  "timeout": 60,
  "maskCallee": false,
  "maskCaller": false
}
```

##### <a name="response"></a><span data-ttu-id="65daf-164">响应</span><span class="sxs-lookup"><span data-stu-id="65daf-164">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---redirecting"></a><span data-ttu-id="65daf-165">通知-重定向</span><span class="sxs-lookup"><span data-stu-id="65daf-165">Notification - redirecting</span></span>

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
        "state": "redirecting"
      }
    }
  ]
}
```

##### <a name="notification---terminated"></a><span data-ttu-id="65daf-166">通知终止</span><span class="sxs-lookup"><span data-stu-id="65daf-166">Notification - terminated</span></span>

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
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "terminated",
        "answeredBy": {
          "identity": {
            "user": {
              "displayName": "Test User 2",
              "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572699"
            }
          }
        },
        "terminationReason": "AppRedirected"
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
