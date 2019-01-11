---
title: 呼叫： 设为静音
description: 允许应用程序本身设为静音。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 603c0d49f47291ec5050cd08dfbb0cc0faa2bc0e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813438"
---
# <a name="call-mute"></a><span data-ttu-id="2d541-103">呼叫： 设为静音</span><span class="sxs-lookup"><span data-stu-id="2d541-103">call: mute</span></span>

> <span data-ttu-id="2d541-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2d541-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2d541-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2d541-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2d541-106">允许应用程序本身设为静音。</span><span class="sxs-lookup"><span data-stu-id="2d541-106">Allows the application to mute itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d541-107">权限</span><span class="sxs-lookup"><span data-stu-id="2d541-107">Permissions</span></span>
<span data-ttu-id="2d541-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2d541-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2d541-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2d541-110">Permission type</span></span>                        | <span data-ttu-id="2d541-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2d541-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2d541-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2d541-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="2d541-113">不受支持。</span><span class="sxs-lookup"><span data-stu-id="2d541-113">Not Supported.</span></span>                               |
| <span data-ttu-id="2d541-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2d541-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d541-115">不受支持。</span><span class="sxs-lookup"><span data-stu-id="2d541-115">Not Supported.</span></span>                               |
| <span data-ttu-id="2d541-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2d541-116">Application</span></span>                            | <span data-ttu-id="2d541-117">无。</span><span class="sxs-lookup"><span data-stu-id="2d541-117">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="2d541-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2d541-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/mute
POST /applications/{id}/calls/{id}/mute
```

## <a name="request-headers"></a><span data-ttu-id="2d541-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2d541-119">Request headers</span></span>
| <span data-ttu-id="2d541-120">名称</span><span class="sxs-lookup"><span data-stu-id="2d541-120">Name</span></span>          | <span data-ttu-id="2d541-121">说明</span><span class="sxs-lookup"><span data-stu-id="2d541-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="2d541-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d541-122">Authorization</span></span> | <span data-ttu-id="2d541-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2d541-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2d541-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="2d541-125">Request body</span></span>
<span data-ttu-id="2d541-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="2d541-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2d541-127">参数</span><span class="sxs-lookup"><span data-stu-id="2d541-127">Parameter</span></span>      | <span data-ttu-id="2d541-128">类型</span><span class="sxs-lookup"><span data-stu-id="2d541-128">Type</span></span>    |<span data-ttu-id="2d541-129">Description</span><span class="sxs-lookup"><span data-stu-id="2d541-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d541-130">clientContext</span><span class="sxs-lookup"><span data-stu-id="2d541-130">clientContext</span></span>|<span data-ttu-id="2d541-131">字符串</span><span class="sxs-lookup"><span data-stu-id="2d541-131">String</span></span>|<span data-ttu-id="2d541-132">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="2d541-132">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="2d541-133">响应</span><span class="sxs-lookup"><span data-stu-id="2d541-133">Response</span></span>
<span data-ttu-id="2d541-134">如果成功，此方法返回`200 OK`响应代码和响应正文中的[commsOperation](../resources/commsoperation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2d541-134">If successful, this method returns `200 OK` response code and a [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d541-135">示例</span><span class="sxs-lookup"><span data-stu-id="2d541-135">Example</span></span>
<span data-ttu-id="2d541-136">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="2d541-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="2d541-137">请求</span><span class="sxs-lookup"><span data-stu-id="2d541-137">Request</span></span>
<span data-ttu-id="2d541-138">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="2d541-138">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="2d541-139">响应</span><span class="sxs-lookup"><span data-stu-id="2d541-139">Response</span></span>

> <span data-ttu-id="2d541-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2d541-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "call: mute",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
