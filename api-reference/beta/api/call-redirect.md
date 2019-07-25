---
title: '呼叫: 重定向'
description: 重定向传入呼叫。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 261d84ce8643d274b81d23284944bd047fc678cc
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864665"
---
# <a name="call-redirect"></a><span data-ttu-id="73092-103">呼叫: 重定向</span><span class="sxs-lookup"><span data-stu-id="73092-103">call: redirect</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73092-104">重定向传入呼叫。</span><span class="sxs-lookup"><span data-stu-id="73092-104">Redirect an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="73092-105">权限</span><span class="sxs-lookup"><span data-stu-id="73092-105">Permissions</span></span>
<span data-ttu-id="73092-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73092-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="73092-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="73092-108">Permission type</span></span> | <span data-ttu-id="73092-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="73092-109">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="73092-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73092-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="73092-111">不支持</span><span class="sxs-lookup"><span data-stu-id="73092-111">Not Supported</span></span>                |
| <span data-ttu-id="73092-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73092-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73092-113">不支持</span><span class="sxs-lookup"><span data-stu-id="73092-113">Not Supported</span></span>                |
| <span data-ttu-id="73092-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="73092-114">Application</span></span>     | <span data-ttu-id="73092-115">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="73092-115">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="73092-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73092-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/redirect
POST /applications/{id}/calls/{id}/redirect
```

## <a name="request-headers"></a><span data-ttu-id="73092-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="73092-117">Request headers</span></span>
| <span data-ttu-id="73092-118">名称</span><span class="sxs-lookup"><span data-stu-id="73092-118">Name</span></span>          | <span data-ttu-id="73092-119">说明</span><span class="sxs-lookup"><span data-stu-id="73092-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="73092-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="73092-120">Authorization</span></span> | <span data-ttu-id="73092-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="73092-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73092-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="73092-123">Request body</span></span>
<span data-ttu-id="73092-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="73092-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="73092-125">参数</span><span class="sxs-lookup"><span data-stu-id="73092-125">Parameter</span></span>      | <span data-ttu-id="73092-126">类型</span><span class="sxs-lookup"><span data-stu-id="73092-126">Type</span></span>    |<span data-ttu-id="73092-127">说明</span><span class="sxs-lookup"><span data-stu-id="73092-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73092-128">targets</span><span class="sxs-lookup"><span data-stu-id="73092-128">targets</span></span>|<span data-ttu-id="73092-129">[invitationParticipantInfo](../resources/invitationparticipantinfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="73092-129">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>|<span data-ttu-id="73092-130">重定向操作的目标参与者。</span><span class="sxs-lookup"><span data-stu-id="73092-130">The target participants of the redirect operation.</span></span>|
|<span data-ttu-id="73092-131">targetDisposition</span><span class="sxs-lookup"><span data-stu-id="73092-131">targetDisposition</span></span>|<span data-ttu-id="73092-132">String</span><span class="sxs-lookup"><span data-stu-id="73092-132">String</span></span>|<span data-ttu-id="73092-133">可能的值为:`default`</span><span class="sxs-lookup"><span data-stu-id="73092-133">The possible value is: `default`</span></span>|
|<span data-ttu-id="73092-134">timeout</span><span class="sxs-lookup"><span data-stu-id="73092-134">timeout</span></span>|<span data-ttu-id="73092-135">Int32</span><span class="sxs-lookup"><span data-stu-id="73092-135">Int32</span></span>|<span data-ttu-id="73092-136">重定向操作的超时时间 (秒)。</span><span class="sxs-lookup"><span data-stu-id="73092-136">The timeout in seconds for the redirect operation.</span></span>|
|<span data-ttu-id="73092-137">maskCallee</span><span class="sxs-lookup"><span data-stu-id="73092-137">maskCallee</span></span>|<span data-ttu-id="73092-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="73092-138">Boolean</span></span>|<span data-ttu-id="73092-139">指示是否屏蔽被叫方。</span><span class="sxs-lookup"><span data-stu-id="73092-139">Indicates whether to mask the callee.</span></span>|
|<span data-ttu-id="73092-140">maskCaller</span><span class="sxs-lookup"><span data-stu-id="73092-140">maskCaller</span></span>|<span data-ttu-id="73092-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="73092-141">Boolean</span></span>|<span data-ttu-id="73092-142">指示是否屏蔽调用方。</span><span class="sxs-lookup"><span data-stu-id="73092-142">Indicates whether to mask the caller.</span></span>|

## <a name="response"></a><span data-ttu-id="73092-143">响应</span><span class="sxs-lookup"><span data-stu-id="73092-143">Response</span></span>
<span data-ttu-id="73092-144">返回`202 Accepted`响应代码</span><span class="sxs-lookup"><span data-stu-id="73092-144">Returns `202 Accepted` response code</span></span>

## <a name="examples"></a><span data-ttu-id="73092-145">示例</span><span class="sxs-lookup"><span data-stu-id="73092-145">Examples</span></span>

### <a name="redirect-a-call"></a><span data-ttu-id="73092-146">重定向呼叫</span><span class="sxs-lookup"><span data-stu-id="73092-146">Redirect a call</span></span>

##### <a name="request"></a><span data-ttu-id="73092-147">请求</span><span class="sxs-lookup"><span data-stu-id="73092-147">Request</span></span>
<span data-ttu-id="73092-148">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="73092-148">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="73092-149">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="73092-149">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="73092-150">C#</span><span class="sxs-lookup"><span data-stu-id="73092-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-redirect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="73092-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="73092-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-redirect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="73092-152">目标-C</span><span class="sxs-lookup"><span data-stu-id="73092-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-redirect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="73092-153">Java</span><span class="sxs-lookup"><span data-stu-id="73092-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-redirect-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="73092-154">响应</span><span class="sxs-lookup"><span data-stu-id="73092-154">Response</span></span>

> <span data-ttu-id="73092-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="73092-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="forward-a-call"></a><span data-ttu-id="73092-157">转接呼叫</span><span class="sxs-lookup"><span data-stu-id="73092-157">Forward a call</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="73092-158">通知传入</span><span class="sxs-lookup"><span data-stu-id="73092-158">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="73092-159">请求</span><span class="sxs-lookup"><span data-stu-id="73092-159">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="73092-160">响应</span><span class="sxs-lookup"><span data-stu-id="73092-160">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---redirecting"></a><span data-ttu-id="73092-161">通知-重定向</span><span class="sxs-lookup"><span data-stu-id="73092-161">Notification - redirecting</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="73092-162">通知终止</span><span class="sxs-lookup"><span data-stu-id="73092-162">Notification - terminated</span></span>

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
