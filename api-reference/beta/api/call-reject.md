---
title: 呼叫： 拒绝
description: 拒绝传入的呼叫。
author: VinodRavichandran
ms.openlocfilehash: 2516ead8d9fa158192a0d9c7c02ac8adb44f764a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343454"
---
# <a name="call-reject"></a><span data-ttu-id="49abf-103">呼叫： 拒绝</span><span class="sxs-lookup"><span data-stu-id="49abf-103">call: reject</span></span>

> <span data-ttu-id="49abf-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="49abf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49abf-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="49abf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="49abf-106">拒绝传入的呼叫。</span><span class="sxs-lookup"><span data-stu-id="49abf-106">Reject an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="49abf-107">权限</span><span class="sxs-lookup"><span data-stu-id="49abf-107">Permissions</span></span>
<span data-ttu-id="49abf-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="49abf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="49abf-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="49abf-110">Permission type</span></span> | <span data-ttu-id="49abf-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="49abf-111">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="49abf-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="49abf-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="49abf-113">不支持</span><span class="sxs-lookup"><span data-stu-id="49abf-113">Not Supported</span></span>                       |
| <span data-ttu-id="49abf-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="49abf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49abf-115">不支持</span><span class="sxs-lookup"><span data-stu-id="49abf-115">Not Supported</span></span>                       |
| <span data-ttu-id="49abf-116">Application</span><span class="sxs-lookup"><span data-stu-id="49abf-116">Application</span></span>     | <span data-ttu-id="49abf-117">无</span><span class="sxs-lookup"><span data-stu-id="49abf-117">None</span></span>                                                       |

## <a name="http-request"></a><span data-ttu-id="49abf-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="49abf-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/reject
POST /applications/{id}/calls/{id}/reject
```

## <a name="request-headers"></a><span data-ttu-id="49abf-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="49abf-119">Request headers</span></span>
| <span data-ttu-id="49abf-120">Name</span><span class="sxs-lookup"><span data-stu-id="49abf-120">Name</span></span>          | <span data-ttu-id="49abf-121">说明</span><span class="sxs-lookup"><span data-stu-id="49abf-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="49abf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="49abf-122">Authorization</span></span> | <span data-ttu-id="49abf-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="49abf-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="49abf-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="49abf-125">Request body</span></span>
<span data-ttu-id="49abf-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="49abf-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="49abf-127">参数</span><span class="sxs-lookup"><span data-stu-id="49abf-127">Parameter</span></span>      | <span data-ttu-id="49abf-128">Type</span><span class="sxs-lookup"><span data-stu-id="49abf-128">Type</span></span>    |<span data-ttu-id="49abf-129">说明</span><span class="sxs-lookup"><span data-stu-id="49abf-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49abf-130">原因</span><span class="sxs-lookup"><span data-stu-id="49abf-130">reason</span></span>|<span data-ttu-id="49abf-131">字符串</span><span class="sxs-lookup"><span data-stu-id="49abf-131">String</span></span>|<span data-ttu-id="49abf-132">拒绝原因。</span><span class="sxs-lookup"><span data-stu-id="49abf-132">The rejection reason.</span></span>|

## <a name="response"></a><span data-ttu-id="49abf-133">响应</span><span class="sxs-lookup"><span data-stu-id="49abf-133">Response</span></span>
<span data-ttu-id="49abf-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="49abf-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

```http
Returns `202 Accepted` response code
```

## <a name="example"></a><span data-ttu-id="49abf-136">示例</span><span class="sxs-lookup"><span data-stu-id="49abf-136">Example</span></span>
<span data-ttu-id="49abf-137">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="49abf-137">The following example shows how to call this API.</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="49abf-138">通知-传入</span><span class="sxs-lookup"><span data-stu-id="49abf-138">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="49abf-139">请求</span><span class="sxs-lookup"><span data-stu-id="49abf-139">Request</span></span>
<span data-ttu-id="49abf-140">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="49abf-140">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call_reject"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/reject
Content-Type: application/json
Content-Length: 24

{
  "reason": "none"
}
```

##### <a name="response"></a><span data-ttu-id="49abf-141">响应</span><span class="sxs-lookup"><span data-stu-id="49abf-141">Response</span></span>
<span data-ttu-id="49abf-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="49abf-142">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---deleted"></a><span data-ttu-id="49abf-143">删除通知</span><span class="sxs-lookup"><span data-stu-id="49abf-143">Notification - deleted</span></span>

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
        "@odata.etag": "W/\"5445\""
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call: reject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
