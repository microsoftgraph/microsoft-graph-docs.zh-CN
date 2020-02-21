---
title: swapShiftsChangeRequest：拒绝
description: 拒绝交换转换请求。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 35d7d9d83dc32d7598815ed8d98e7f6f828d8b1f
ms.sourcegitcommit: 31a9b4cb3d0f905f123475a4c1a86f5b1e59b935
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2020
ms.locfileid: "42219789"
---
# <a name="swapshiftschangerequest-decline"></a><span data-ttu-id="9a15d-103">swapShiftsChangeRequest：拒绝</span><span class="sxs-lookup"><span data-stu-id="9a15d-103">swapShiftsChangeRequest: decline</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a15d-104">拒绝[swapShiftsChangeRequest](../resources/swapshiftschangerequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9a15d-104">Decline a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a15d-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="9a15d-105">Permissions</span></span>

<span data-ttu-id="9a15d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9a15d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9a15d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9a15d-108">Permission type</span></span>                        | <span data-ttu-id="9a15d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9a15d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9a15d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9a15d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9a15d-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a15d-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="9a15d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9a15d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a15d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a15d-113">Not supported.</span></span> |
| <span data-ttu-id="9a15d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9a15d-114">Application</span></span>                            | <span data-ttu-id="9a15d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a15d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a15d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9a15d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="9a15d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="9a15d-117">Request headers</span></span>

| <span data-ttu-id="9a15d-118">名称</span><span class="sxs-lookup"><span data-stu-id="9a15d-118">Name</span></span>          | <span data-ttu-id="9a15d-119">说明</span><span class="sxs-lookup"><span data-stu-id="9a15d-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9a15d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a15d-120">Authorization</span></span> | <span data-ttu-id="9a15d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9a15d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9a15d-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="9a15d-123">Content-type</span></span> | <span data-ttu-id="9a15d-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="9a15d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a15d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9a15d-126">Request body</span></span>

<span data-ttu-id="9a15d-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="9a15d-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9a15d-128">参数</span><span class="sxs-lookup"><span data-stu-id="9a15d-128">Parameter</span></span>    | <span data-ttu-id="9a15d-129">类型</span><span class="sxs-lookup"><span data-stu-id="9a15d-129">Type</span></span>        | <span data-ttu-id="9a15d-130">描述</span><span class="sxs-lookup"><span data-stu-id="9a15d-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9a15d-131">message</span><span class="sxs-lookup"><span data-stu-id="9a15d-131">message</span></span>|<span data-ttu-id="9a15d-132">String</span><span class="sxs-lookup"><span data-stu-id="9a15d-132">String</span></span>|<span data-ttu-id="9a15d-133">自定义拒绝邮件。</span><span class="sxs-lookup"><span data-stu-id="9a15d-133">A custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="9a15d-134">响应</span><span class="sxs-lookup"><span data-stu-id="9a15d-134">Response</span></span>

<span data-ttu-id="9a15d-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9a15d-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9a15d-137">示例</span><span class="sxs-lookup"><span data-stu-id="9a15d-137">Examples</span></span>

<span data-ttu-id="9a15d-138">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="9a15d-138">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="9a15d-139">请求</span><span class="sxs-lookup"><span data-stu-id="9a15d-139">Request</span></span>

<span data-ttu-id="9a15d-140">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="9a15d-140">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "swapshiftchangerequest_decline"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/decline
Content-type: application/json

{
  "message": "message-value"
}
```

### <a name="response"></a><span data-ttu-id="9a15d-141">响应</span><span class="sxs-lookup"><span data-stu-id="9a15d-141">Response</span></span>

<span data-ttu-id="9a15d-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9a15d-142">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 NO CONTENT
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "swapShiftChangeRequest: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
