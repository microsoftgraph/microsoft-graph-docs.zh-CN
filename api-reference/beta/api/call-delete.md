---
title: 删除呼叫
description: 删除或挂断活动呼叫。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 6eb30d8e92fe99e06467c01104d8742d090a8a18
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328043"
---
# <a name="delete-call"></a><span data-ttu-id="23356-103">删除呼叫</span><span class="sxs-lookup"><span data-stu-id="23356-103">Delete call</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23356-104">删除或挂断活动呼叫。</span><span class="sxs-lookup"><span data-stu-id="23356-104">Delete or hang up an active call.</span></span>

## <a name="permissions"></a><span data-ttu-id="23356-105">权限</span><span class="sxs-lookup"><span data-stu-id="23356-105">Permissions</span></span>

<span data-ttu-id="23356-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="23356-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="23356-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="23356-108">Permission type</span></span> | <span data-ttu-id="23356-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="23356-109">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="23356-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="23356-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="23356-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="23356-111">Not Supported.</span></span>                         |
| <span data-ttu-id="23356-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="23356-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23356-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="23356-113">Not Supported.</span></span>                         |
| <span data-ttu-id="23356-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="23356-114">Application</span></span>                            | <span data-ttu-id="23356-115">无。</span><span class="sxs-lookup"><span data-stu-id="23356-115">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="23356-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="23356-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}
DELETE /applications/{id}/calls/{id}
```

## <a name="request-headers"></a><span data-ttu-id="23356-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="23356-117">Request headers</span></span>
| <span data-ttu-id="23356-118">名称</span><span class="sxs-lookup"><span data-stu-id="23356-118">Name</span></span>          | <span data-ttu-id="23356-119">说明</span><span class="sxs-lookup"><span data-stu-id="23356-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="23356-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="23356-120">Authorization</span></span> | <span data-ttu-id="23356-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="23356-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="23356-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="23356-123">Request body</span></span>
<span data-ttu-id="23356-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="23356-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23356-125">响应</span><span class="sxs-lookup"><span data-stu-id="23356-125">Response</span></span>
<span data-ttu-id="23356-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="23356-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23356-128">示例</span><span class="sxs-lookup"><span data-stu-id="23356-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="23356-129">请求</span><span class="sxs-lookup"><span data-stu-id="23356-129">Request</span></span>
<span data-ttu-id="23356-130">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="23356-130">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete-call"
}-->
```http
DELETE https://graph.microsoft.com/beta/app/calls/{id}
```

##### <a name="response"></a><span data-ttu-id="23356-131">响应</span><span class="sxs-lookup"><span data-stu-id="23356-131">Response</span></span>

> <span data-ttu-id="23356-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="23356-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="notification---terminating"></a><span data-ttu-id="23356-134">通知终止</span><span class="sxs-lookup"><span data-stu-id="23356-134">Notification - terminating</span></span>

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
        "state": "terminating"
      }
    }
  ]
}
```

##### <a name="notification---terminated"></a><span data-ttu-id="23356-135">通知终止</span><span class="sxs-lookup"><span data-stu-id="23356-135">Notification - terminated</span></span>

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
        "terminationReason": "AppInitiated"
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
  "description": "Delete call",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
