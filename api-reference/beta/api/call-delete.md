---
title: 删除呼叫
description: 删除或挂断活动呼叫。
author: VinodRavichandran
ms.openlocfilehash: 07183b4837e6107f347947b901d4efea76b7da98
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350965"
---
# <a name="delete-call"></a><span data-ttu-id="0f44a-103">删除呼叫</span><span class="sxs-lookup"><span data-stu-id="0f44a-103">Delete call</span></span>

> <span data-ttu-id="0f44a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0f44a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f44a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0f44a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0f44a-106">删除或挂断活动呼叫。</span><span class="sxs-lookup"><span data-stu-id="0f44a-106">Delete or hang up an active call.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f44a-107">权限</span><span class="sxs-lookup"><span data-stu-id="0f44a-107">Permissions</span></span>

<span data-ttu-id="0f44a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0f44a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0f44a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0f44a-110">Permission type</span></span> | <span data-ttu-id="0f44a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0f44a-111">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="0f44a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0f44a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="0f44a-113">不受支持。</span><span class="sxs-lookup"><span data-stu-id="0f44a-113">Not Supported.</span></span>                         |
| <span data-ttu-id="0f44a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0f44a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f44a-115">不受支持。</span><span class="sxs-lookup"><span data-stu-id="0f44a-115">Not Supported.</span></span>                         |
| <span data-ttu-id="0f44a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0f44a-116">Application</span></span>                            | <span data-ttu-id="0f44a-117">无。</span><span class="sxs-lookup"><span data-stu-id="0f44a-117">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="0f44a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0f44a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}
DELETE /applications/{id}/calls/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0f44a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0f44a-119">Request headers</span></span>
| <span data-ttu-id="0f44a-120">Name</span><span class="sxs-lookup"><span data-stu-id="0f44a-120">Name</span></span>          | <span data-ttu-id="0f44a-121">说明</span><span class="sxs-lookup"><span data-stu-id="0f44a-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="0f44a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f44a-122">Authorization</span></span> | <span data-ttu-id="0f44a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0f44a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f44a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="0f44a-125">Request body</span></span>
<span data-ttu-id="0f44a-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0f44a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f44a-127">响应</span><span class="sxs-lookup"><span data-stu-id="0f44a-127">Response</span></span>
<span data-ttu-id="0f44a-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0f44a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f44a-130">示例</span><span class="sxs-lookup"><span data-stu-id="0f44a-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0f44a-131">请求</span><span class="sxs-lookup"><span data-stu-id="0f44a-131">Request</span></span>
<span data-ttu-id="0f44a-132">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="0f44a-132">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_call"
}-->
```http
DELETE https://graph.microsoft.com/beta/app/calls/{id}
```

##### <a name="response"></a><span data-ttu-id="0f44a-133">响应</span><span class="sxs-lookup"><span data-stu-id="0f44a-133">Response</span></span>

> <span data-ttu-id="0f44a-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0f44a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="notification---terminating"></a><span data-ttu-id="0f44a-136">通知-终止</span><span class="sxs-lookup"><span data-stu-id="0f44a-136">Notification - terminating</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="0f44a-137">通知-终止</span><span class="sxs-lookup"><span data-stu-id="0f44a-137">Notification - terminated</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Delete call",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
