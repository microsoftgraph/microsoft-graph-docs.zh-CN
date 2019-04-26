---
title: '参与者: muteAll'
description: 将呼叫中的所有参与者设为静音。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7ae154e0a9e211620d9761c9051e73d5b35ec020
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33332743"
---
# <a name="participant-muteall"></a><span data-ttu-id="d2b83-103">参与者: muteAll</span><span class="sxs-lookup"><span data-stu-id="d2b83-103">participant: muteAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2b83-104">将呼叫中的所有参与者设为静音。</span><span class="sxs-lookup"><span data-stu-id="d2b83-104">Mute all participants in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2b83-105">权限</span><span class="sxs-lookup"><span data-stu-id="d2b83-105">Permissions</span></span>
<span data-ttu-id="d2b83-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d2b83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d2b83-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d2b83-108">Permission type</span></span>                        | <span data-ttu-id="d2b83-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d2b83-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d2b83-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d2b83-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d2b83-111">不支持</span><span class="sxs-lookup"><span data-stu-id="d2b83-111">Not Supported</span></span>                               |
| <span data-ttu-id="d2b83-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d2b83-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2b83-113">不支持</span><span class="sxs-lookup"><span data-stu-id="d2b83-113">Not Supported</span></span>                               |
| <span data-ttu-id="d2b83-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d2b83-114">Application</span></span>                            | <span data-ttu-id="d2b83-115">无</span><span class="sxs-lookup"><span data-stu-id="d2b83-115">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="d2b83-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d2b83-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/muteAll
POST /applications/{id}/calls/{id}/participants/muteAll
```

## <a name="request-headers"></a><span data-ttu-id="d2b83-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="d2b83-117">Request headers</span></span>
| <span data-ttu-id="d2b83-118">名称</span><span class="sxs-lookup"><span data-stu-id="d2b83-118">Name</span></span>          | <span data-ttu-id="d2b83-119">说明</span><span class="sxs-lookup"><span data-stu-id="d2b83-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d2b83-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2b83-120">Authorization</span></span> | <span data-ttu-id="d2b83-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d2b83-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2b83-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="d2b83-123">Request body</span></span>
<span data-ttu-id="d2b83-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d2b83-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d2b83-125">参数</span><span class="sxs-lookup"><span data-stu-id="d2b83-125">Parameter</span></span>      | <span data-ttu-id="d2b83-126">类型</span><span class="sxs-lookup"><span data-stu-id="d2b83-126">Type</span></span>    |<span data-ttu-id="d2b83-127">说明</span><span class="sxs-lookup"><span data-stu-id="d2b83-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2b83-128">participants</span><span class="sxs-lookup"><span data-stu-id="d2b83-128">participants</span></span>|<span data-ttu-id="d2b83-129">String 集合</span><span class="sxs-lookup"><span data-stu-id="d2b83-129">String collection</span></span>|<span data-ttu-id="d2b83-130">要静音的参与者。</span><span class="sxs-lookup"><span data-stu-id="d2b83-130">The participants to be muted.</span></span>|
|<span data-ttu-id="d2b83-131">适用</span><span class="sxs-lookup"><span data-stu-id="d2b83-131">clientContext</span></span>|<span data-ttu-id="d2b83-132">String</span><span class="sxs-lookup"><span data-stu-id="d2b83-132">String</span></span>|<span data-ttu-id="d2b83-133">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="d2b83-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="d2b83-134">响应</span><span class="sxs-lookup"><span data-stu-id="d2b83-134">Response</span></span>
<span data-ttu-id="d2b83-135">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[commsOperation](../resources/commsoperation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d2b83-135">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2b83-136">示例</span><span class="sxs-lookup"><span data-stu-id="d2b83-136">Example</span></span>
<span data-ttu-id="d2b83-137">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="d2b83-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="d2b83-138">请求</span><span class="sxs-lookup"><span data-stu-id="d2b83-138">Request</span></span>
<span data-ttu-id="d2b83-139">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="d2b83-139">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "participant-muteAll"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/participants/muteAll
Content-Type: application/json
Content-Length: 81

{
  "participants": [
    ""
  ],
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="d2b83-140">响应</span><span class="sxs-lookup"><span data-stu-id="d2b83-140">Response</span></span>

> <span data-ttu-id="d2b83-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d2b83-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "participant: muteAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
