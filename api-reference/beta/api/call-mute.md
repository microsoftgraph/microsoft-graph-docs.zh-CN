---
title: '呼叫: 静音'
description: 允许应用程序将其本身设为静音。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2f619cdc42ff914999ad8826ff31452ff82ea6a1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461246"
---
# <a name="call-mute"></a><span data-ttu-id="59d3e-103">呼叫: 静音</span><span class="sxs-lookup"><span data-stu-id="59d3e-103">call: mute</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59d3e-104">允许应用程序将其本身设为静音。</span><span class="sxs-lookup"><span data-stu-id="59d3e-104">Allows the application to mute itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="59d3e-105">权限</span><span class="sxs-lookup"><span data-stu-id="59d3e-105">Permissions</span></span>
<span data-ttu-id="59d3e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="59d3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="59d3e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="59d3e-108">Permission type</span></span>                        | <span data-ttu-id="59d3e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="59d3e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="59d3e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59d3e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="59d3e-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="59d3e-111">Not Supported.</span></span>                               |
| <span data-ttu-id="59d3e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59d3e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59d3e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="59d3e-113">Not Supported.</span></span>                               |
| <span data-ttu-id="59d3e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="59d3e-114">Application</span></span>                            | <span data-ttu-id="59d3e-115">无。</span><span class="sxs-lookup"><span data-stu-id="59d3e-115">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="59d3e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="59d3e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/mute
POST /applications/{id}/calls/{id}/mute
```

## <a name="request-headers"></a><span data-ttu-id="59d3e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="59d3e-117">Request headers</span></span>
| <span data-ttu-id="59d3e-118">名称</span><span class="sxs-lookup"><span data-stu-id="59d3e-118">Name</span></span>          | <span data-ttu-id="59d3e-119">说明</span><span class="sxs-lookup"><span data-stu-id="59d3e-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="59d3e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="59d3e-120">Authorization</span></span> | <span data-ttu-id="59d3e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="59d3e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59d3e-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="59d3e-123">Request body</span></span>
<span data-ttu-id="59d3e-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="59d3e-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="59d3e-125">参数</span><span class="sxs-lookup"><span data-stu-id="59d3e-125">Parameter</span></span>      | <span data-ttu-id="59d3e-126">类型</span><span class="sxs-lookup"><span data-stu-id="59d3e-126">Type</span></span>    |<span data-ttu-id="59d3e-127">说明</span><span class="sxs-lookup"><span data-stu-id="59d3e-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59d3e-128">适用</span><span class="sxs-lookup"><span data-stu-id="59d3e-128">clientContext</span></span>|<span data-ttu-id="59d3e-129">字符串</span><span class="sxs-lookup"><span data-stu-id="59d3e-129">String</span></span>|<span data-ttu-id="59d3e-130">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="59d3e-130">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="59d3e-131">响应</span><span class="sxs-lookup"><span data-stu-id="59d3e-131">Response</span></span>
<span data-ttu-id="59d3e-132">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[commsOperation](../resources/commsoperation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="59d3e-132">If successful, this method returns `200 OK` response code and a [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59d3e-133">示例</span><span class="sxs-lookup"><span data-stu-id="59d3e-133">Example</span></span>
<span data-ttu-id="59d3e-134">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="59d3e-134">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="59d3e-135">请求</span><span class="sxs-lookup"><span data-stu-id="59d3e-135">Request</span></span>
<span data-ttu-id="59d3e-136">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="59d3e-136">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-mute"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/mute
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="59d3e-137">响应</span><span class="sxs-lookup"><span data-stu-id="59d3e-137">Response</span></span>

> <span data-ttu-id="59d3e-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="59d3e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: mute",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-mute.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
