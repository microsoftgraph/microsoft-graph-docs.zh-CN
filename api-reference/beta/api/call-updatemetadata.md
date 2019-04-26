---
title: '调用: updateMetadata'
description: 更新与调用相关联的 appliation 的元数据。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 73d75c671bd8e80e35e68f239d24a1a99736ae54
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328111"
---
# <a name="call-updatemetadata"></a><span data-ttu-id="fffe5-103">调用: updateMetadata</span><span class="sxs-lookup"><span data-stu-id="fffe5-103">call: updateMetadata</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fffe5-104">更新与调用相关联的 appliation 的元数据。</span><span class="sxs-lookup"><span data-stu-id="fffe5-104">Update the appliation's metadata associated with a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="fffe5-105">权限</span><span class="sxs-lookup"><span data-stu-id="fffe5-105">Permissions</span></span>
<span data-ttu-id="fffe5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fffe5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fffe5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="fffe5-108">Permission type</span></span>                        | <span data-ttu-id="fffe5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fffe5-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fffe5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fffe5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="fffe5-111">不支持</span><span class="sxs-lookup"><span data-stu-id="fffe5-111">Not Supported</span></span>                               |
| <span data-ttu-id="fffe5-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fffe5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fffe5-113">不支持</span><span class="sxs-lookup"><span data-stu-id="fffe5-113">Not Supported</span></span>                               |
| <span data-ttu-id="fffe5-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="fffe5-114">Application</span></span>     | <span data-ttu-id="fffe5-115">JoinGroupCallsasGuest、JoinGroupCalls、InitiateGroupCalls 和。 all</span><span class="sxs-lookup"><span data-stu-id="fffe5-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fffe5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fffe5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/updateMetadata
POST /applications/{id}/calls/{id}/updateMetadata
```

## <a name="request-headers"></a><span data-ttu-id="fffe5-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="fffe5-117">Request headers</span></span>
| <span data-ttu-id="fffe5-118">名称</span><span class="sxs-lookup"><span data-stu-id="fffe5-118">Name</span></span>          | <span data-ttu-id="fffe5-119">说明</span><span class="sxs-lookup"><span data-stu-id="fffe5-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="fffe5-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="fffe5-120">Authorization</span></span> | <span data-ttu-id="fffe5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fffe5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fffe5-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="fffe5-123">Request body</span></span>
<span data-ttu-id="fffe5-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="fffe5-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fffe5-125">参数</span><span class="sxs-lookup"><span data-stu-id="fffe5-125">Parameter</span></span>      | <span data-ttu-id="fffe5-126">类型</span><span class="sxs-lookup"><span data-stu-id="fffe5-126">Type</span></span>    |<span data-ttu-id="fffe5-127">说明</span><span class="sxs-lookup"><span data-stu-id="fffe5-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fffe5-128">metadata</span><span class="sxs-lookup"><span data-stu-id="fffe5-128">metadata</span></span>|<span data-ttu-id="fffe5-129">String</span><span class="sxs-lookup"><span data-stu-id="fffe5-129">String</span></span>|<span data-ttu-id="fffe5-130">名单中参与者提供的数据的 blob。</span><span class="sxs-lookup"><span data-stu-id="fffe5-130">A blob of data provided by the participant in the roster.</span></span>|
|<span data-ttu-id="fffe5-131">适用</span><span class="sxs-lookup"><span data-stu-id="fffe5-131">clientContext</span></span>|<span data-ttu-id="fffe5-132">String</span><span class="sxs-lookup"><span data-stu-id="fffe5-132">String</span></span>|<span data-ttu-id="fffe5-133">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="fffe5-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="fffe5-134">响应</span><span class="sxs-lookup"><span data-stu-id="fffe5-134">Response</span></span>
<span data-ttu-id="fffe5-135">返回`202 Accepted`响应代码和位置标头, 其中包含为此请求创建的[commsOperation](../resources/commsoperation.md)的 uri。</span><span class="sxs-lookup"><span data-stu-id="fffe5-135">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="fffe5-136">示例</span><span class="sxs-lookup"><span data-stu-id="fffe5-136">Example</span></span>
<span data-ttu-id="fffe5-137">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="fffe5-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="fffe5-138">请求</span><span class="sxs-lookup"><span data-stu-id="fffe5-138">Request</span></span>
<span data-ttu-id="fffe5-139">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="fffe5-139">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-updateMetadata"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/updateMetadata
Content-Type: application/json
Content-Length: 79

{
  "metadata": "metadata-value",
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="fffe5-140">响应</span><span class="sxs-lookup"><span data-stu-id="fffe5-140">Response</span></span>

> <span data-ttu-id="fffe5-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fffe5-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: updateMetadata",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
