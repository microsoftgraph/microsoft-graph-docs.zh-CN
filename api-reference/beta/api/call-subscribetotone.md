---
title: '调用: subscribeToTone'
description: 订阅 DTMF (双音多频信号)。 这样, 当用户在 "按键电话" 上按下按键时, 您就会收到通知。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 33ce1e97c104a8dcbeff75e249493f19bc530781
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35438578"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="a15b9-104">调用: subscribeToTone</span><span class="sxs-lookup"><span data-stu-id="a15b9-104">call: subscribeToTone</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a15b9-105">订阅 DTMF (双音多频信号)。</span><span class="sxs-lookup"><span data-stu-id="a15b9-105">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="a15b9-106">这样, 你就可以在用户按 "按键时" 电话上的键时收到通知。</span><span class="sxs-lookup"><span data-stu-id="a15b9-106">This allows you to be notified when the user presses keys on a "touchtone" phone.</span></span>

## <a name="permissions"></a><span data-ttu-id="a15b9-107">权限</span><span class="sxs-lookup"><span data-stu-id="a15b9-107">Permissions</span></span>
<span data-ttu-id="a15b9-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a15b9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a15b9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a15b9-110">Permission type</span></span> | <span data-ttu-id="a15b9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a15b9-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="a15b9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a15b9-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a15b9-113">不支持</span><span class="sxs-lookup"><span data-stu-id="a15b9-113">Not Supported</span></span>        |
| <span data-ttu-id="a15b9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a15b9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a15b9-115">不支持</span><span class="sxs-lookup"><span data-stu-id="a15b9-115">Not Supported</span></span>        |
| <span data-ttu-id="a15b9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a15b9-116">Application</span></span>     | <span data-ttu-id="a15b9-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="a15b9-117">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="a15b9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a15b9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/subscribeToTone
POST /applications/{id}/calls/{id}/subscribeToTone
```

## <a name="request-headers"></a><span data-ttu-id="a15b9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a15b9-119">Request headers</span></span>
| <span data-ttu-id="a15b9-120">名称</span><span class="sxs-lookup"><span data-stu-id="a15b9-120">Name</span></span>          | <span data-ttu-id="a15b9-121">说明</span><span class="sxs-lookup"><span data-stu-id="a15b9-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="a15b9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a15b9-122">Authorization</span></span> | <span data-ttu-id="a15b9-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a15b9-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a15b9-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a15b9-125">Request body</span></span>
<span data-ttu-id="a15b9-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a15b9-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a15b9-127">参数</span><span class="sxs-lookup"><span data-stu-id="a15b9-127">Parameter</span></span>      | <span data-ttu-id="a15b9-128">类型</span><span class="sxs-lookup"><span data-stu-id="a15b9-128">Type</span></span>    | <span data-ttu-id="a15b9-129">说明</span><span class="sxs-lookup"><span data-stu-id="a15b9-129">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="a15b9-130">适用</span><span class="sxs-lookup"><span data-stu-id="a15b9-130">clientContext</span></span>  | <span data-ttu-id="a15b9-131">String</span><span class="sxs-lookup"><span data-stu-id="a15b9-131">String</span></span>  | <span data-ttu-id="a15b9-132">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="a15b9-132">The client context.</span></span> |

## <a name="response"></a><span data-ttu-id="a15b9-133">响应</span><span class="sxs-lookup"><span data-stu-id="a15b9-133">Response</span></span>
<span data-ttu-id="a15b9-134">返回`202 Accepted`响应代码和位置标头, 其中包含为此请求创建的[commsOperation](../resources/commsoperation.md)的 uri。</span><span class="sxs-lookup"><span data-stu-id="a15b9-134">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="a15b9-135">示例</span><span class="sxs-lookup"><span data-stu-id="a15b9-135">Example</span></span>
<span data-ttu-id="a15b9-136">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="a15b9-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="a15b9-137">请求</span><span class="sxs-lookup"><span data-stu-id="a15b9-137">Request</span></span>
<span data-ttu-id="a15b9-138">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="a15b9-138">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a15b9-139">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="a15b9-139">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="a15b9-140">C#</span><span class="sxs-lookup"><span data-stu-id="a15b9-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-subscribetotone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a15b9-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="a15b9-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-subscribetotone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a15b9-142">目标-C</span><span class="sxs-lookup"><span data-stu-id="a15b9-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-subscribetotone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a15b9-143">响应</span><span class="sxs-lookup"><span data-stu-id="a15b9-143">Response</span></span>

> <span data-ttu-id="a15b9-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a15b9-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="a15b9-146">通知-操作已完成</span><span class="sxs-lookup"><span data-stu-id="a15b9-146">Notification - operation completed</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "call: subscribeToTone",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
