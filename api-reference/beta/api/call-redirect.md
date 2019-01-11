---
title: 呼叫： 重定向
description: 重定向传入呼叫。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: f581a5ce95368e7d852a5b1435ef05bf940f607c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809469"
---
# <a name="call-redirect"></a><span data-ttu-id="dcfc0-103">呼叫： 重定向</span><span class="sxs-lookup"><span data-stu-id="dcfc0-103">call: redirect</span></span>

> <span data-ttu-id="dcfc0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="dcfc0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dcfc0-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="dcfc0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dcfc0-106">重定向传入呼叫。</span><span class="sxs-lookup"><span data-stu-id="dcfc0-106">Redirect an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="dcfc0-107">权限</span><span class="sxs-lookup"><span data-stu-id="dcfc0-107">Permissions</span></span>
<span data-ttu-id="dcfc0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dcfc0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dcfc0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="dcfc0-110">Permission type</span></span> | <span data-ttu-id="dcfc0-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dcfc0-111">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="dcfc0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dcfc0-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="dcfc0-113">不支持</span><span class="sxs-lookup"><span data-stu-id="dcfc0-113">Not Supported</span></span>                |
| <span data-ttu-id="dcfc0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dcfc0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcfc0-115">不支持</span><span class="sxs-lookup"><span data-stu-id="dcfc0-115">Not Supported</span></span>                |
| <span data-ttu-id="dcfc0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="dcfc0-116">Application</span></span>     | <span data-ttu-id="dcfc0-117">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="dcfc0-117">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="dcfc0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dcfc0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/redirect
POST /applications/{id}/calls/{id}/redirect
```

## <a name="request-headers"></a><span data-ttu-id="dcfc0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="dcfc0-119">Request headers</span></span>
| <span data-ttu-id="dcfc0-120">名称</span><span class="sxs-lookup"><span data-stu-id="dcfc0-120">Name</span></span>          | <span data-ttu-id="dcfc0-121">说明</span><span class="sxs-lookup"><span data-stu-id="dcfc0-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="dcfc0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dcfc0-122">Authorization</span></span> | <span data-ttu-id="dcfc0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dcfc0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dcfc0-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="dcfc0-125">Request body</span></span>
<span data-ttu-id="dcfc0-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="dcfc0-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dcfc0-127">参数</span><span class="sxs-lookup"><span data-stu-id="dcfc0-127">Parameter</span></span>      | <span data-ttu-id="dcfc0-128">类型</span><span class="sxs-lookup"><span data-stu-id="dcfc0-128">Type</span></span>    |<span data-ttu-id="dcfc0-129">Description</span><span class="sxs-lookup"><span data-stu-id="dcfc0-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dcfc0-130">目标</span><span class="sxs-lookup"><span data-stu-id="dcfc0-130">targets</span></span>|<span data-ttu-id="dcfc0-131">[invitationParticipantInfo](../resources/invitationparticipantinfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="dcfc0-131">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>|<span data-ttu-id="dcfc0-132">重定向操作的目标参与者。</span><span class="sxs-lookup"><span data-stu-id="dcfc0-132">The target participants of the redirect operation.</span></span>|
|<span data-ttu-id="dcfc0-133">targetDisposition</span><span class="sxs-lookup"><span data-stu-id="dcfc0-133">targetDisposition</span></span>|<span data-ttu-id="dcfc0-134">字符串</span><span class="sxs-lookup"><span data-stu-id="dcfc0-134">String</span></span>|<span data-ttu-id="dcfc0-135">可能的值是：`default`</span><span class="sxs-lookup"><span data-stu-id="dcfc0-135">The possible value is: `default`</span></span>|
|<span data-ttu-id="dcfc0-136">timeout</span><span class="sxs-lookup"><span data-stu-id="dcfc0-136">timeout</span></span>|<span data-ttu-id="dcfc0-137">Int32</span><span class="sxs-lookup"><span data-stu-id="dcfc0-137">Int32</span></span>|<span data-ttu-id="dcfc0-138">超时的重定向操作的秒数。</span><span class="sxs-lookup"><span data-stu-id="dcfc0-138">The timeout in seconds for the redirect operation.</span></span>|
|<span data-ttu-id="dcfc0-139">maskCallee</span><span class="sxs-lookup"><span data-stu-id="dcfc0-139">maskCallee</span></span>|<span data-ttu-id="dcfc0-140">布尔</span><span class="sxs-lookup"><span data-stu-id="dcfc0-140">Boolean</span></span>|<span data-ttu-id="dcfc0-141">指示是否屏蔽被叫方。</span><span class="sxs-lookup"><span data-stu-id="dcfc0-141">Indicates whether to mask the callee.</span></span>|
|<span data-ttu-id="dcfc0-142">maskCaller</span><span class="sxs-lookup"><span data-stu-id="dcfc0-142">maskCaller</span></span>|<span data-ttu-id="dcfc0-143">布尔</span><span class="sxs-lookup"><span data-stu-id="dcfc0-143">Boolean</span></span>|<span data-ttu-id="dcfc0-144">指示是否屏蔽呼叫者。</span><span class="sxs-lookup"><span data-stu-id="dcfc0-144">Indicates whether to mask the caller.</span></span>|

## <a name="response"></a><span data-ttu-id="dcfc0-145">响应</span><span class="sxs-lookup"><span data-stu-id="dcfc0-145">Response</span></span>
<span data-ttu-id="dcfc0-146">返回`202 Accepted`响应代码</span><span class="sxs-lookup"><span data-stu-id="dcfc0-146">Returns `202 Accepted` response code</span></span>

## <a name="examples"></a><span data-ttu-id="dcfc0-147">示例</span><span class="sxs-lookup"><span data-stu-id="dcfc0-147">Examples</span></span>

### <a name="redirect-a-call"></a><span data-ttu-id="dcfc0-148">将呼叫重定向</span><span class="sxs-lookup"><span data-stu-id="dcfc0-148">Redirect a call</span></span>

##### <a name="request"></a><span data-ttu-id="dcfc0-149">请求</span><span class="sxs-lookup"><span data-stu-id="dcfc0-149">Request</span></span>
<span data-ttu-id="dcfc0-150">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="dcfc0-150">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="dcfc0-151">响应</span><span class="sxs-lookup"><span data-stu-id="dcfc0-151">Response</span></span>

> <span data-ttu-id="dcfc0-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="dcfc0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="forward-a-call"></a><span data-ttu-id="dcfc0-154">转移呼叫</span><span class="sxs-lookup"><span data-stu-id="dcfc0-154">Forward a call</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="dcfc0-155">通知-传入</span><span class="sxs-lookup"><span data-stu-id="dcfc0-155">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="dcfc0-156">请求</span><span class="sxs-lookup"><span data-stu-id="dcfc0-156">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="dcfc0-157">响应</span><span class="sxs-lookup"><span data-stu-id="dcfc0-157">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---redirecting"></a><span data-ttu-id="dcfc0-158">通知-重定向</span><span class="sxs-lookup"><span data-stu-id="dcfc0-158">Notification - redirecting</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="dcfc0-159">通知-终止</span><span class="sxs-lookup"><span data-stu-id="dcfc0-159">Notification - terminated</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "call: redirect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
