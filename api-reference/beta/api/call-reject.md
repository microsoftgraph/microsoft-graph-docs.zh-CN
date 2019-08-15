---
title: '呼叫: 拒绝'
description: 拒绝传入呼叫。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 61a7b417d2688539d705e1718813ea54c538bddf
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36418878"
---
# <a name="call-reject"></a><span data-ttu-id="6708e-103">呼叫: 拒绝</span><span class="sxs-lookup"><span data-stu-id="6708e-103">call: reject</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6708e-104">拒绝传入呼叫。</span><span class="sxs-lookup"><span data-stu-id="6708e-104">Reject an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="6708e-105">权限</span><span class="sxs-lookup"><span data-stu-id="6708e-105">Permissions</span></span>
<span data-ttu-id="6708e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6708e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6708e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6708e-108">Permission type</span></span> | <span data-ttu-id="6708e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6708e-109">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="6708e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6708e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6708e-111">不支持</span><span class="sxs-lookup"><span data-stu-id="6708e-111">Not Supported</span></span>                       |
| <span data-ttu-id="6708e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6708e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6708e-113">不支持</span><span class="sxs-lookup"><span data-stu-id="6708e-113">Not Supported</span></span>                       |
| <span data-ttu-id="6708e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6708e-114">Application</span></span>     | <span data-ttu-id="6708e-115">无</span><span class="sxs-lookup"><span data-stu-id="6708e-115">None</span></span>                                                       |

## <a name="http-request"></a><span data-ttu-id="6708e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6708e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/reject
POST /applications/{id}/calls/{id}/reject
```

## <a name="request-headers"></a><span data-ttu-id="6708e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="6708e-117">Request headers</span></span>
| <span data-ttu-id="6708e-118">名称</span><span class="sxs-lookup"><span data-stu-id="6708e-118">Name</span></span>          | <span data-ttu-id="6708e-119">说明</span><span class="sxs-lookup"><span data-stu-id="6708e-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="6708e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6708e-120">Authorization</span></span> | <span data-ttu-id="6708e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6708e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6708e-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="6708e-123">Request body</span></span>
<span data-ttu-id="6708e-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="6708e-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6708e-125">参数</span><span class="sxs-lookup"><span data-stu-id="6708e-125">Parameter</span></span>      | <span data-ttu-id="6708e-126">类型</span><span class="sxs-lookup"><span data-stu-id="6708e-126">Type</span></span>    |<span data-ttu-id="6708e-127">说明</span><span class="sxs-lookup"><span data-stu-id="6708e-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6708e-128">在于</span><span class="sxs-lookup"><span data-stu-id="6708e-128">reason</span></span>|<span data-ttu-id="6708e-129">String</span><span class="sxs-lookup"><span data-stu-id="6708e-129">String</span></span>|<span data-ttu-id="6708e-130">拒绝原因。</span><span class="sxs-lookup"><span data-stu-id="6708e-130">The rejection reason.</span></span>|

## <a name="response"></a><span data-ttu-id="6708e-131">响应</span><span class="sxs-lookup"><span data-stu-id="6708e-131">Response</span></span>
<span data-ttu-id="6708e-p103">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6708e-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

```http
Returns `202 Accepted` response code
```

## <a name="example"></a><span data-ttu-id="6708e-134">示例</span><span class="sxs-lookup"><span data-stu-id="6708e-134">Example</span></span>
<span data-ttu-id="6708e-135">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="6708e-135">The following example shows how to call this API.</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="6708e-136">通知传入</span><span class="sxs-lookup"><span data-stu-id="6708e-136">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="6708e-137">请求</span><span class="sxs-lookup"><span data-stu-id="6708e-137">Request</span></span>
<span data-ttu-id="6708e-138">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="6708e-138">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6708e-139">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="6708e-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-reject"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/reject
Content-Type: application/json
Content-Length: 24

{
  "reason": "none"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6708e-140">C#</span><span class="sxs-lookup"><span data-stu-id="6708e-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6708e-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6708e-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6708e-142">目标-C</span><span class="sxs-lookup"><span data-stu-id="6708e-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6708e-143">响应</span><span class="sxs-lookup"><span data-stu-id="6708e-143">Response</span></span>
<span data-ttu-id="6708e-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6708e-144">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---deleted"></a><span data-ttu-id="6708e-145">通知-已删除</span><span class="sxs-lookup"><span data-stu-id="6708e-145">Notification - deleted</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "call: reject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
