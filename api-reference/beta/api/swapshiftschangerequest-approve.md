---
title: swapShiftsChangeRequest：批准
description: 批准交换转换请求。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f952444e374d7db808dc708bf75dd9e6617d2e19
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952200"
---
# <a name="swapshiftschangerequest-approve"></a><span data-ttu-id="74452-103">swapShiftsChangeRequest：批准</span><span class="sxs-lookup"><span data-stu-id="74452-103">swapShiftsChangeRequest: approve</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74452-104">批准[swapShiftsChangeRequest](../resources/swapshiftschangerequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="74452-104">Approve a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="74452-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="74452-105">Permissions</span></span>

<span data-ttu-id="74452-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="74452-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="74452-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="74452-108">Permission type</span></span>                        | <span data-ttu-id="74452-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="74452-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="74452-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="74452-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="74452-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74452-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="74452-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="74452-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74452-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="74452-113">Not supported.</span></span> |
| <span data-ttu-id="74452-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="74452-114">Application</span></span>                            | <span data-ttu-id="74452-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="74452-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="74452-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="74452-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/swapShiftsChangeRequests/approve
```

## <a name="request-headers"></a><span data-ttu-id="74452-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="74452-117">Request headers</span></span>

| <span data-ttu-id="74452-118">名称</span><span class="sxs-lookup"><span data-stu-id="74452-118">Name</span></span>          | <span data-ttu-id="74452-119">说明</span><span class="sxs-lookup"><span data-stu-id="74452-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="74452-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="74452-120">Authorization</span></span> | <span data-ttu-id="74452-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="74452-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="74452-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="74452-123">Content-type</span></span> | <span data-ttu-id="74452-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="74452-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="74452-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="74452-126">Request body</span></span>

<span data-ttu-id="74452-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="74452-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="74452-128">参数</span><span class="sxs-lookup"><span data-stu-id="74452-128">Parameter</span></span>    | <span data-ttu-id="74452-129">类型</span><span class="sxs-lookup"><span data-stu-id="74452-129">Type</span></span>        | <span data-ttu-id="74452-130">描述</span><span class="sxs-lookup"><span data-stu-id="74452-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="74452-131">message</span><span class="sxs-lookup"><span data-stu-id="74452-131">message</span></span>|<span data-ttu-id="74452-132">String</span><span class="sxs-lookup"><span data-stu-id="74452-132">String</span></span>|<span data-ttu-id="74452-133">自定义审批邮件。</span><span class="sxs-lookup"><span data-stu-id="74452-133">A custom approval message.</span></span>|

## <a name="response"></a><span data-ttu-id="74452-134">响应</span><span class="sxs-lookup"><span data-stu-id="74452-134">Response</span></span>

<span data-ttu-id="74452-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="74452-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="74452-137">示例</span><span class="sxs-lookup"><span data-stu-id="74452-137">Examples</span></span>

<span data-ttu-id="74452-138">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="74452-138">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="74452-139">请求</span><span class="sxs-lookup"><span data-stu-id="74452-139">Request</span></span>

<span data-ttu-id="74452-140">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="74452-140">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "openshiftchangerequest_approve"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/schedule/openShiftsChangeRequests/approve
Content-type: application/json

{
  "message": "message-value"
}
```

### <a name="response"></a><span data-ttu-id="74452-141">响应</span><span class="sxs-lookup"><span data-stu-id="74452-141">Response</span></span>

<span data-ttu-id="74452-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="74452-142">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openShiftChangeRequest: approve",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
