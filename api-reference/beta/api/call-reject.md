---
title: '呼叫: 拒绝'
description: 拒绝传入呼叫。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 5b42ebee208431cd0a02be291d07f580d98c87a1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461302"
---
# <a name="call-reject"></a><span data-ttu-id="acd6a-103">呼叫: 拒绝</span><span class="sxs-lookup"><span data-stu-id="acd6a-103">call: reject</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="acd6a-104">拒绝传入呼叫。</span><span class="sxs-lookup"><span data-stu-id="acd6a-104">Reject an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="acd6a-105">权限</span><span class="sxs-lookup"><span data-stu-id="acd6a-105">Permissions</span></span>
<span data-ttu-id="acd6a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="acd6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="acd6a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="acd6a-108">Permission type</span></span> | <span data-ttu-id="acd6a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="acd6a-109">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="acd6a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="acd6a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="acd6a-111">不支持</span><span class="sxs-lookup"><span data-stu-id="acd6a-111">Not Supported</span></span>                       |
| <span data-ttu-id="acd6a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="acd6a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="acd6a-113">不支持</span><span class="sxs-lookup"><span data-stu-id="acd6a-113">Not Supported</span></span>                       |
| <span data-ttu-id="acd6a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="acd6a-114">Application</span></span>     | <span data-ttu-id="acd6a-115">无</span><span class="sxs-lookup"><span data-stu-id="acd6a-115">None</span></span>                                                       |

## <a name="http-request"></a><span data-ttu-id="acd6a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="acd6a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/reject
POST /applications/{id}/calls/{id}/reject
```

## <a name="request-headers"></a><span data-ttu-id="acd6a-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="acd6a-117">Request headers</span></span>
| <span data-ttu-id="acd6a-118">名称</span><span class="sxs-lookup"><span data-stu-id="acd6a-118">Name</span></span>          | <span data-ttu-id="acd6a-119">说明</span><span class="sxs-lookup"><span data-stu-id="acd6a-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="acd6a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="acd6a-120">Authorization</span></span> | <span data-ttu-id="acd6a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="acd6a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="acd6a-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="acd6a-123">Request body</span></span>
<span data-ttu-id="acd6a-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="acd6a-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="acd6a-125">参数</span><span class="sxs-lookup"><span data-stu-id="acd6a-125">Parameter</span></span>      | <span data-ttu-id="acd6a-126">类型</span><span class="sxs-lookup"><span data-stu-id="acd6a-126">Type</span></span>    |<span data-ttu-id="acd6a-127">说明</span><span class="sxs-lookup"><span data-stu-id="acd6a-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="acd6a-128">在于</span><span class="sxs-lookup"><span data-stu-id="acd6a-128">reason</span></span>|<span data-ttu-id="acd6a-129">字符串</span><span class="sxs-lookup"><span data-stu-id="acd6a-129">String</span></span>|<span data-ttu-id="acd6a-130">拒绝原因。</span><span class="sxs-lookup"><span data-stu-id="acd6a-130">The rejection reason.</span></span>|

## <a name="response"></a><span data-ttu-id="acd6a-131">响应</span><span class="sxs-lookup"><span data-stu-id="acd6a-131">Response</span></span>
<span data-ttu-id="acd6a-p103">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="acd6a-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

```http
Returns `202 Accepted` response code
```

## <a name="example"></a><span data-ttu-id="acd6a-134">示例</span><span class="sxs-lookup"><span data-stu-id="acd6a-134">Example</span></span>
<span data-ttu-id="acd6a-135">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="acd6a-135">The following example shows how to call this API.</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="acd6a-136">通知传入</span><span class="sxs-lookup"><span data-stu-id="acd6a-136">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="acd6a-137">请求</span><span class="sxs-lookup"><span data-stu-id="acd6a-137">Request</span></span>
<span data-ttu-id="acd6a-138">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="acd6a-138">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="acd6a-139">响应</span><span class="sxs-lookup"><span data-stu-id="acd6a-139">Response</span></span>
<span data-ttu-id="acd6a-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="acd6a-140">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---deleted"></a><span data-ttu-id="acd6a-141">通知-已删除</span><span class="sxs-lookup"><span data-stu-id="acd6a-141">Notification - deleted</span></span>

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
    "Error: /api-reference/beta/api/call-reject.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
