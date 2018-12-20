---
title: 呼叫： subscribeToTone
description: 订阅 DTMF （双音多频信号）。 这使您用户按键在电话上按下键时收到通知。
author: VinodRavichandran
ms.openlocfilehash: 82f7632736dc187fae1313224a6cb6f4807e0dd1
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380434"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="ad997-104">呼叫： subscribeToTone</span><span class="sxs-lookup"><span data-stu-id="ad997-104">call: subscribeToTone</span></span>

> <span data-ttu-id="ad997-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ad997-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad997-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ad997-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ad997-107">订阅 DTMF （双音多频信号）。</span><span class="sxs-lookup"><span data-stu-id="ad997-107">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="ad997-108">这使您的用户"按键"在电话上按下键时收到通知。</span><span class="sxs-lookup"><span data-stu-id="ad997-108">This allows you to be notified when the user presses keys on a "touchtone" phone.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad997-109">权限</span><span class="sxs-lookup"><span data-stu-id="ad997-109">Permissions</span></span>
<span data-ttu-id="ad997-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ad997-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ad997-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="ad997-112">Permission type</span></span> | <span data-ttu-id="ad997-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ad997-113">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="ad997-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ad997-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="ad997-115">不支持</span><span class="sxs-lookup"><span data-stu-id="ad997-115">Not Supported</span></span>        |
| <span data-ttu-id="ad997-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ad997-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad997-117">不支持</span><span class="sxs-lookup"><span data-stu-id="ad997-117">Not Supported</span></span>        |
| <span data-ttu-id="ad997-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="ad997-118">Application</span></span>     | <span data-ttu-id="ad997-119">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="ad997-119">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="ad997-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ad997-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/subscribeToTone
POST /applications/{id}/calls/{id}/subscribeToTone
```

## <a name="request-headers"></a><span data-ttu-id="ad997-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ad997-121">Request headers</span></span>
| <span data-ttu-id="ad997-122">名称</span><span class="sxs-lookup"><span data-stu-id="ad997-122">Name</span></span>          | <span data-ttu-id="ad997-123">说明</span><span class="sxs-lookup"><span data-stu-id="ad997-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="ad997-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad997-124">Authorization</span></span> | <span data-ttu-id="ad997-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ad997-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad997-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ad997-127">Request body</span></span>
<span data-ttu-id="ad997-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="ad997-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ad997-129">参数</span><span class="sxs-lookup"><span data-stu-id="ad997-129">Parameter</span></span>      | <span data-ttu-id="ad997-130">类型</span><span class="sxs-lookup"><span data-stu-id="ad997-130">Type</span></span>    | <span data-ttu-id="ad997-131">说明</span><span class="sxs-lookup"><span data-stu-id="ad997-131">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="ad997-132">clientContext</span><span class="sxs-lookup"><span data-stu-id="ad997-132">clientContext</span></span>  | <span data-ttu-id="ad997-133">字符串</span><span class="sxs-lookup"><span data-stu-id="ad997-133">String</span></span>  | <span data-ttu-id="ad997-134">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="ad997-134">The client context.</span></span> |

## <a name="response"></a><span data-ttu-id="ad997-135">响应</span><span class="sxs-lookup"><span data-stu-id="ad997-135">Response</span></span>
<span data-ttu-id="ad997-136">返回`202 Accepted`响应代码和具有[commsOperation](../resources/commsoperation.md)创建的此请求 uri 中的位置标头。</span><span class="sxs-lookup"><span data-stu-id="ad997-136">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="ad997-137">示例</span><span class="sxs-lookup"><span data-stu-id="ad997-137">Example</span></span>
<span data-ttu-id="ad997-138">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="ad997-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="ad997-139">请求</span><span class="sxs-lookup"><span data-stu-id="ad997-139">Request</span></span>
<span data-ttu-id="ad997-140">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="ad997-140">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-subscribeToTone"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/subscribeToTone
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="response"></a><span data-ttu-id="ad997-141">响应</span><span class="sxs-lookup"><span data-stu-id="ad997-141">Response</span></span>

> <span data-ttu-id="ad997-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ad997-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="ad997-144">通知-完成的操作</span><span class="sxs-lookup"><span data-stu-id="ad997-144">Notification - operation completed</span></span>

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
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "status": "completed"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call: subscribeToTone",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
