---
title: '调用: cancelMediaProcessing'
description: 取消所有正在进行的任何 PlayPrompt 或记录操作的媒体处理。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 77c35cb0cfeaea6ebb2e623b32b1fa3c70f65777
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461306"
---
# <a name="call-cancelmediaprocessing"></a><span data-ttu-id="3ed44-103">调用: cancelMediaProcessing</span><span class="sxs-lookup"><span data-stu-id="3ed44-103">call: cancelMediaProcessing</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ed44-104">取消所有正在进行的任何 PlayPrompt 或记录操作的媒体处理。</span><span class="sxs-lookup"><span data-stu-id="3ed44-104">Cancels media processing for all in-progress any PlayPrompt or Record operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ed44-105">权限</span><span class="sxs-lookup"><span data-stu-id="3ed44-105">Permissions</span></span>
<span data-ttu-id="3ed44-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3ed44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3ed44-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3ed44-108">Permission type</span></span>                        | <span data-ttu-id="3ed44-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3ed44-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3ed44-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3ed44-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3ed44-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ed44-111">Not Supported.</span></span>                              |
| <span data-ttu-id="3ed44-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3ed44-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ed44-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ed44-113">Not Supported.</span></span>                              |
| <span data-ttu-id="3ed44-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3ed44-114">Application</span></span>                            | <span data-ttu-id="3ed44-115">无。</span><span class="sxs-lookup"><span data-stu-id="3ed44-115">None.</span></span>                                       |

## <a name="http-request"></a><span data-ttu-id="3ed44-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3ed44-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/cancelMediaProcessing
POST /applications/{id}/calls/{id}/cancelMediaProcessing
```

## <a name="request-headers"></a><span data-ttu-id="3ed44-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="3ed44-117">Request headers</span></span>
| <span data-ttu-id="3ed44-118">名称</span><span class="sxs-lookup"><span data-stu-id="3ed44-118">Name</span></span>          | <span data-ttu-id="3ed44-119">说明</span><span class="sxs-lookup"><span data-stu-id="3ed44-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="3ed44-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ed44-120">Authorization</span></span> | <span data-ttu-id="3ed44-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3ed44-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ed44-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="3ed44-123">Request body</span></span>
<span data-ttu-id="3ed44-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="3ed44-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3ed44-125">参数</span><span class="sxs-lookup"><span data-stu-id="3ed44-125">Parameter</span></span>      | <span data-ttu-id="3ed44-126">类型</span><span class="sxs-lookup"><span data-stu-id="3ed44-126">Type</span></span>    | <span data-ttu-id="3ed44-127">说明</span><span class="sxs-lookup"><span data-stu-id="3ed44-127">Description</span></span>                                                    |
|:---------------|:--------|:---------------------------------------------------------------|
| <span data-ttu-id="3ed44-128">各种</span><span class="sxs-lookup"><span data-stu-id="3ed44-128">all</span></span>            | <span data-ttu-id="3ed44-129">布尔</span><span class="sxs-lookup"><span data-stu-id="3ed44-129">Boolean</span></span> | <span data-ttu-id="3ed44-130">指示是否停止所有操作或当前操作的标志。</span><span class="sxs-lookup"><span data-stu-id="3ed44-130">The flag indicating whether to stop all operations or current.</span></span> |
| <span data-ttu-id="3ed44-131">适用</span><span class="sxs-lookup"><span data-stu-id="3ed44-131">clientContext</span></span>  | <span data-ttu-id="3ed44-132">字符串</span><span class="sxs-lookup"><span data-stu-id="3ed44-132">String</span></span>  | <span data-ttu-id="3ed44-133">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="3ed44-133">The client context.</span></span>                                            |

## <a name="response"></a><span data-ttu-id="3ed44-134">响应</span><span class="sxs-lookup"><span data-stu-id="3ed44-134">Response</span></span>
<span data-ttu-id="3ed44-135">返回`202 Accepted`响应代码和位置标头, 其中包含为此请求创建的[commsOperation](../resources/commsoperation.md)的 uri。</span><span class="sxs-lookup"><span data-stu-id="3ed44-135">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="3ed44-136">示例</span><span class="sxs-lookup"><span data-stu-id="3ed44-136">Example</span></span>
<span data-ttu-id="3ed44-137">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="3ed44-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="3ed44-138">请求</span><span class="sxs-lookup"><span data-stu-id="3ed44-138">Request</span></span>
<span data-ttu-id="3ed44-139">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="3ed44-139">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-cancelMediaProcessing"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/cancelMediaProcessing
Content-Type: application/json
Content-Length: 62

{
  "all": true,
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="3ed44-140">响应</span><span class="sxs-lookup"><span data-stu-id="3ed44-140">Response</span></span>

> <span data-ttu-id="3ed44-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3ed44-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="3ed44-143">通知-操作已完成</span><span class="sxs-lookup"><span data-stu-id="3ed44-143">Notification - operation completed</span></span>

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
  "description": "call: cancelMediaProcessing",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-cancelmediaprocessing.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
